# Contributor License Agreement (CLA)

This directory holds the org's Contributor License Agreements and the runbook for
enforcing them. The decision to use a CLA (over a DCO) and the rationale are in
[`../LICENSING.md`](../LICENSING.md) §3.

| File | Purpose |
|------|---------|
| [`individual-cla.md`](./individual-cla.md) | Individual CLA (ICLA) — signed by each individual contributor |
| [`corporate-cla.md`](./corporate-cla.md) | Corporate CLA (CCLA) — signed by an employer for its designated employees |

> **Both texts are DRAFT and must be reviewed by legal counsel before
> enforcement.** They are adapted from the Apache Software Foundation ICLA v2.2 /
> CCLA v2.0. Until enforcement is announced, the
> [GitHub ToS inbound=outbound rule](https://docs.github.com/en/site-policy/github-terms/github-terms-of-service#6-contributions-under-repository-license)
> governs.

## Enforcement: CLA Assistant

Signatures are collected automatically when a contributor opens their first pull
request. There are two ways to run CLA Assistant; pick one before enabling.

### Recommended — CLA Assistant Lite (GitHub Action)

[`cla-assistant/github-action`](https://github.com/cla-assistant/github-action)
runs as a workflow inside our own org and **stores signatures in a file in one of
our own repositories** — no third-party service holds contributor data, which fits
the project's data-ownership stance. Tradeoff: the workflow must be added to each
repo that gates on the CLA (or distributed via an org workflow template).

**Manual setup steps (require org/repo admin — cannot be automated here):**

1. Create a fine-grained Personal Access Token (or a GitHub App token) with
   `contents: write` on the repo chosen to store signatures, and add it as the
   `PERSONAL_ACCESS_TOKEN` Actions secret in each repo that uses the workflow.
2. Decide the signatures storage location (e.g. a `signatures` branch, or a
   `cla/signatures.json` file in this `.github` repo).
3. Add a workflow like the following to each gated repo as
   `.github/workflows/cla.yml`:

   ```yaml
   name: CLA Assistant
   on:
     issue_comment:
       types: [created]
     pull_request_target:
       types: [opened, closed, synchronize]
   permissions:
     actions: write
     contents: write
     pull-requests: write
     statuses: write
   jobs:
     cla:
       runs-on: ubuntu-latest
       steps:
         - uses: cla-assistant/github-action@v2.6.1
           env:
             GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
             PERSONAL_ACCESS_TOKEN: ${{ secrets.PERSONAL_ACCESS_TOKEN }}
           with:
             path-to-signatures: 'cla/signatures.json'
             path-to-document: 'https://github.com/agentic-commons-foundation/.github/blob/main/legal/individual-cla.md'
             branch: 'cla-signatures'
             allowlist: 'dependabot[bot],pre-commit-ci[bot],*[bot]'
   ```

4. Confirm the bot comments on a test PR and records the signature.

### Alternative — hosted CLA Assistant (GitHub App)

[cla-assistant.io](https://cla-assistant.io) is a one-click GitHub App: authorize
it on the org, paste the CLA text, and it gates PRs org-wide from a central
dashboard. Easier to operate, but a third party stores the signature records —
which is why Lite is recommended here.

## After enforcement is live

- Add the `path-to-document` link to the in-force ICLA/CCLA (this directory).
- Update [`../CONTRIBUTING.md`](../CONTRIBUTING.md) §0.2 to state the CLA is now
  enforced (it currently says "until the CLA bot is live...").
- Note the go-live date in the brand Decision Log.
