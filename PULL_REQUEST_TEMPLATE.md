<!--
Thank you for contributing. Filling this out fully speeds up review.
See CONTRIBUTING.md §1.3 for branch / commit / PR conventions.
-->

## What this PR does

<!-- 1–3 sentences. State the change, not the motivation (motivation belongs in the linked issue). -->

## Linked issue

Closes #

<!-- If this PR does not close an issue, explain why an issue isn't needed (typo, doc fix, mechanical refactor). For non-trivial changes, open an issue first. -->

## Type of change

- [ ] Bug fix (non-breaking)
- [ ] New feature (non-breaking)
- [ ] Breaking change (requires version bump and migration note)
- [ ] Documentation only
- [ ] Build / CI / tooling

## Cross-repo impact

This change requires a corresponding update in:

- [ ] `spec` — protocol-level change (PR linked: )
- [ ] `guides` — user-facing behavior changed (PR linked: )
- [ ] `agentic-commons` — public website affected (PR linked: )
- [ ] None of the above

## Testing

- [ ] Existing tests pass locally (`uv run pytest` / `pnpm test`)
- [ ] Added tests for new behavior, if applicable
- [ ] Manually verified the change end-to-end (describe below)

<!-- For agent-node / SDK changes, describe what end-to-end run you did and the result. -->

## Quality checklist

- [ ] CI is green
- [ ] Linter passes (`ruff` / `eslint`)
- [ ] PR title follows Conventional Commits (`type(scope): subject`)
- [ ] No secrets, API keys, or private data in the diff
- [ ] If touching public website / docs / blog: voice and tone follow [`marketing/brand/voice-and-tone.md`](https://github.com/heydoraai/agentic-commons/blob/main/marketing/brand/voice-and-tone.md) (no AI marketing words, no AI-tells)

## Code of Conduct

- [ ] I have read and agree to follow the [Code of Conduct](./CODE_OF_CONDUCT.md).
