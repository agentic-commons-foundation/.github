# Licensing Policy

This is the canonical licensing policy for the [`@agentic-commons-foundation`](https://github.com/agentic-commons-foundation) organization. It applies to every repository in the org. The protocol, registry, and brand are held in trust by Obiwan Co., Limited and are intended to transfer to the independent Agentic Commons Foundation as the network matures.

Status: **FROZEN** (2026-06-09). Changes to this policy follow the process in [§5](#5-changing-this-policy).

## 1. The license trio

Project output is split by **what it is**, and each class uses the license that best fits its purpose.

| Asset class | License | Why this one |
|------------|---------|--------------|
| **Documentation** — tutorials, mission copy, public website prose, blog posts | [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) | Copyleft (Share-Alike) keeps derived content open — the same license Wikipedia uses. Attribution required. |
| **Source code** — SDKs, CLI, validators, bots, website code | [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0) | Permissive, to maximize adoption across any runtime. Includes an explicit patent grant and a patent-retaliation clause — important for protocol/agent code. |
| **Protocol specification** — marker format, identifier spec, verification rules | [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/) | Public-domain dedication, so the spec can become a truly neutral standard anyone — including upstream platforms and competitors — can implement with zero license friction. |

## 2. The `.github` exception

Community-health files in the [`.github`](https://github.com/agentic-commons-foundation/.github) repository — Code of Conduct, issue templates, PR template — are licensed [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) (no Share-Alike), matching the upstream [Contributor Covenant](https://www.contributor-covenant.org/). This lets anyone fork and reuse these community files without copyleft propagation. The "documentation = CC BY-SA 4.0" rule above refers to substantive content and tutorials, not boilerplate community files.

## 3. Contributor License Agreement (CLA)

Contributions require signing a **Contributor License Agreement** — an Individual CLA (ICLA) for individuals and a Corporate CLA (CCLA) for contributions made on behalf of an employer. Sign-off is automated via [CLA Assistant](https://github.com/cla-assistant/cla-assistant) on every pull request.

We chose a CLA over a [DCO](https://developercertificate.org/) because the project is on a path to becoming a 501(c)(3) foundation: a CLA concentrates the inbound grant in the holding entity, which makes the eventual transfer to the Agentic Commons Foundation clean and lets the foundation relicense on the community's behalf if ever necessary.

Until the CLA bot is live, the [GitHub Terms of Service §D.6 inbound=outbound rule](https://docs.github.com/en/site-policy/github-terms/github-terms-of-service#6-contributions-under-repository-license) governs.

## 4. Current per-repository status

| Repository | Class | License | Status |
|-----------|-------|---------|--------|
| [`spec`](https://github.com/agentic-commons-foundation/spec) | Protocol | CC0 1.0 | ✅ Aligned |
| [`guides`](https://github.com/agentic-commons-foundation/guides) | Documentation | CC BY-SA 4.0 | ✅ Aligned |
| [`.github`](https://github.com/agentic-commons-foundation/.github) | Community files | CC BY 4.0 | ✅ Aligned (§2 exception) |
| [`musicbrainz-bot`](https://github.com/agentic-commons-foundation/musicbrainz-bot) | Source code | MIT → Apache 2.0 | 🔄 Migrating |
| [`openlibrary-bots`](https://github.com/agentic-commons-foundation/openlibrary-bots) | Source code (fork) | AGPL-3.0 (upstream) | ✅ Documented exception (see below) |

**New repositories** adopt the trio default for their class from creation: code → Apache 2.0, documentation → CC BY-SA 4.0, protocol → CC0 1.0. Forks inherit upstream license constraints and are evaluated case by case before any relicensing.

### Fork exception: `openlibrary-bots`

[`openlibrary-bots`](https://github.com/agentic-commons-foundation/openlibrary-bots) is a fork of [`internetarchive/openlibrary-bots`](https://github.com/internetarchive/openlibrary-bots), which is licensed **GNU AGPL-3.0**. AGPL-3.0 is a strong (network) copyleft license, so the fork **must remain AGPL-3.0** — it cannot be relicensed to Apache 2.0 without the consent of every upstream copyright holder. Any modifications we publish on top of it are likewise AGPL-3.0. This is the intended behavior of the policy's "forks inherit upstream constraints" rule, not a violation of the code = Apache 2.0 default, which applies to original work.

## 5. Changing this policy

This policy is FROZEN. Material changes (adding/removing an asset class, changing a default license, changing the CLA terms) go through the org's RFC process in [`spec`](https://github.com/agentic-commons-foundation/spec): public proposal, ≥14 days discussion, maintainer majority. The rationale for the current trio, the `.github` exception, and the CLA-over-DCO choice is recorded in the brand Decision Log.
