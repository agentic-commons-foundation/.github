# Code of Conduct

> **Status**: DRAFT — pending team review before first public repository in `@agentic-commons-foundation` (later renamed `@agentic-commons`) is opened. Once a single repository under this organization is public, this document MUST be in place at `.github/CODE_OF_CONDUCT.md`.
>
> **Publish gate** — this document MUST NOT be published until all of the following are true:
> 1. `coc@agentic-commons.org` routes to a monitored inbox.
> 2. `security@agentic-commons.org` routes to a monitored inbox.
> 3. `hello@agentic-commons.org` routes to a monitored inbox.
> 4. The Trust & Safety lead role (per §7) is filled by a named individual at Obiwan Co., Limited (the founding contributor entity currently holding the project in trust).
>
> **Scope**: This Code of Conduct (the "Code") applies to every space the Agentic Commons project operates in — see §3.
>
> **Source basis**: This document adapts the [Contributor Covenant 2.1](https://www.contributor-covenant.org/version/2/1/code_of_conduct/) (CC BY 4.0). Specific modifications from the upstream version are listed in §9.

---

## §0 Preamble

Agentic Commons is a public-good network where AI agents contribute to open-source, scientific, and public-interest projects with verifiable provenance. Our community spans contributors who write code, contributors who run agent nodes, and contributors who maintain upstream public-good projects.

Funders, sponsors, and Foundation stewards — distinct from but adjacent to this contributor community — are governed by the same standards under §4.4.

Every participant operates under the same expectations of conduct. There is no separate standard for "core team" versus "external contributor", for "human contributor" versus "agent operator", or for "ClawGrid commercial users" versus "Agentic Commons public-good contributors".

---

## §1 Our Pledge

We as members, contributors, and leaders pledge to make participation in the Agentic Commons community a harassment-free experience for everyone, regardless of age, body size, visible or invisible disability, ethnicity, sex characteristics, gender identity and expression, level of experience, education, socio-economic status, nationality, personal appearance, race, caste, color, religion, or sexual identity and orientation.

We pledge to act and interact in ways that contribute to an open, welcoming, diverse, inclusive, and healthy community.

---

## §2 Our Standards

Examples of behavior that contributes to a positive environment for the Agentic Commons community include:

- Demonstrating empathy and kindness toward other people
- Being respectful of differing opinions, viewpoints, and experiences
- Giving and gracefully accepting constructive feedback
- Accepting responsibility and apologizing to those affected by our mistakes, and learning from the experience
- Focusing on what is best not just for us as individuals, but for the overall community

Examples of unacceptable behavior include:

- The use of sexualized language or imagery, and sexual attention or advances of any kind
- Trolling, insulting or derogatory comments, and personal or political attacks
- Public or private harassment
- Publishing others' private information, such as a physical or email address, without their explicit permission
- Other conduct which could reasonably be considered inappropriate in a professional setting

---

## §3 Scope

This Code applies within all Agentic Commons community spaces, and also applies when an individual is officially representing the community in public spaces — including on personal accounts when the post is presented in a community-representative capacity.

Specifically:

| Space | Operator | Where this Code is enforced |
|-------|----------|---------------------------|
| GitHub Organization (`@agentic-commons-foundation`, later `@agentic-commons`) | Project maintainers (transferring to the Agentic Commons Foundation once incorporated) | All repositories, issues, PRs, Discussions, releases, wiki |
| Discord (`https://discord.gg/kp6fTb4eFZ`) | Project maintainers + appointed moderators | All channels including voice, threads, and direct messages between members where the contact originated through a community space |
| Public social platforms and community sites | Project maintainers | Replies, quote-posts, comments under posts from any **official Agentic Commons account**, plus personal accounts when the holder is acting in a community-representative capacity. The authoritative list of official accounts (and their status) is maintained at [`agentic-commons-foundation/official-accounts`](https://github.com/agentic-commons-foundation/official-accounts) — that repository, not this Code, is the source of truth for which accounts exist. |
| Wikipedia, OpenStreetMap, GitHub OSS, HuggingFace, OpenStax, scientific literature platforms | Each upstream project's own governance | Agent contributions made under Agentic Commons identifiers — see §4.3 |
| Newsletter (`newsletter.agentic-commons.org`) | Project maintainers | Replies to project email addresses |
| Live events, conference talks, meetups, hackathons | Event organizers + project speakers | Any session, booth, or social gathering presented as Agentic Commons |
| Direct project email (`hello@`, `coc@`, `security@`) | Project maintainers (transferring to the Agentic Commons Foundation once incorporated) | All correspondence |

Representing the community includes using an official project email address, posting via an official social media account, or acting as an appointed representative at an online or offline event.

**Impersonation**: Accounts on any platform that are not on the [official-accounts list](https://github.com/agentic-commons-foundation/official-accounts) are not Agentic Commons accounts, regardless of similarity to project naming. Reports of impersonation may be sent to `coc@agentic-commons.org`; we will pursue platform-level takedown but cannot enforce this Code against an account we do not operate.

**Pre-launch / silent reservations**: A platform handle that has been registered defensively (to prevent squatting) but on which the project has not yet posted official content is governed by this Code only from the date of first official post or interaction. Until then, the handle is a defensive registration with no community presence to govern. Reservation status is tracked in the official-accounts list.

---

## §4 Project-Specific Provisions

The following additions are specific to Agentic Commons because of the project's nature — agent-driven contributions across multiple platforms, and the project's structural relationship to the upstream public-good projects we contribute to.

### §4.1 Agent-Generated Conduct

Agents (Claude Code, Codex, GitHub Copilot, Cursor, OpenClaw, or any other runtime) acting under an Agentic Commons identifier are subject to this Code. The fact that a comment, edit, pull request, or message was produced by an AI agent does not exempt it from §2.

Specifically:

- **The operator of an agent node is responsible for the conduct of the agent running on it.** "I didn't write that, my agent did" is not a defense.
- **Operators are responsible for ensuring their agents comply** with the contribution policies, bot policies, and Codes of Conduct of any upstream public-good project the agent submits to.
- **High-volume agent posting in conversational spaces** (Discord text channels, GitHub Discussions, Reddit threads) is treated as spam under §5, regardless of intent. Agents belong in upstream contribution channels (Wikipedia edits, OSS PRs, dataset commits) — not in community discussion spaces.
- **Agent-generated content must be identifiable as such**:
  - In community spaces (Discord, GitHub Discussions, Reddit), prefix the post with `[agent:<your-id>]` or an equivalent explicit declaration.
  - In upstream contribution channels (Wikipedia edits, GitHub PRs, OSM changesets, dataset commits), include the `[ACG #id]` provenance marker per the [`marker-spec`](https://github.com/agentic-commons-foundation/spec).
  - Concealing agent authorship in either context is a violation.
- **Prompt injection attempts directed at other contributors' agents** — for example, embedding instructions in a Discord message intended to manipulate another operator's agent — are treated as harassment under §2.

### §4.2 Cross-Platform Enforcement

A single Code applies across every space in §3. A contributor sanctioned under §8.3 or §8.4 in one space (e.g., Discord) is sanctioned identically across the other spaces (GitHub Org membership, social channels, future events). §8.1–§8.2 sanctions are scoped to the space where the violation occurred unless the Trust & Safety contact in §7 documents a reason to extend.

Coordination of cross-platform enforcement is handled by the Trust & Safety contact. Decisions and the reasoning behind them are recorded in a non-public moderator log. An aggregate transparency report (counts by category, no identifying details) is published periodically at `@agentic-commons-foundation/transparency` once that repository is established.

### §4.3 Our Community's Commitments to Upstream Projects

Agentic Commons routes contributions to upstream public-good projects (Wikipedia, OpenStreetMap, GitHub-hosted OSS, HuggingFace, OpenStax, and others across six domains: climate, public health, education, accessibility, science, and the digital commons).

The commitments below are *self-imposed* — this Code does not attempt to govern upstream projects we have no formal relationship with.

#### §4.3.1 Two operational modes

Most agent contributions to upstream projects do not involve a formal relationship between Agentic Commons and the upstream project. The CoC distinguishes two modes to be honest about this:

**Mode A — individual-contributor mode** (default; the majority of contributions):

The agent submits an edit, PR, or commit through the same channel any individual contributor would use. The contribution is bound by the upstream project's general contributor policies (Wikipedia editing guidelines, GitHub PR conventions, OSM mapping standards), not by any institutional agreement. There is no formal relationship between Agentic Commons and the upstream project in this mode, and we do not claim one.

**Mode B — institutional-cooperation mode** (smaller subset; required when applicable):

The agent operates under a project-level relationship: the upstream project has completed our formal partner-onboarding process (documented in the project's governance repository), or the contribution would cross a threshold the upstream project's bot or automation policy treats as institutional (notably: Wikipedia edits at any volume that triggers the [BAG BRFA](https://en.wikipedia.org/wiki/Wikipedia:Bots/Requests_for_approval) requirement; npm package publishing at non-personal scale; high-frequency OSM imports). In this mode there is an addressable institutional relationship.

Determining which mode applies is the operator's responsibility before starting a task class at scale. When in doubt, treat the activity as Mode B and seek the upstream institutional process before scaling.

#### §4.3.2 Operator commitments (apply in either mode)

- Every agent contribution carries a verifiable provenance marker.
- Operators ensure their agents follow whichever level of upstream policy applies — individual-contributor guidelines for Mode A, bot / institutional policies for Mode B.
- When operating in Mode B, the relevant institutional process (e.g., a granted BRFA, a published npm-publishing arrangement) must be completed *before* the high-volume activity begins. Retroactive approval is not assumed.

#### §4.3.3 Project-level commitments (Mode B only)

- When an upstream project in Mode B asks Agentic Commons to pause, slow, or change a class of contribution, we comply within the timeline they specify, through the contact established at onboarding or BRFA.
- For Mode A contributions, upstream feedback flows through standard channels — reverts, PR rejections, talk-page mentions, issue comments. Aggregate signals are captured in the coordinator's quality-scoring system and used to throttle or retire task classes; we do not claim addressable-entity status for Mode A and therefore do not promise individual response to addressed requests.

#### §4.3.4 Toward our own community members who participate in upstream review

- When members of our community also serve as reviewers in upstream public-good projects, we expect them to evaluate each agent contribution on its merits using the same standard they apply to human contributors.
- Reflexively rejecting an agent contribution solely because it was produced by an agent — without engaging with the substance of the change — is conduct we discourage from our own community.
- This expectation does not extend to upstream reviewers who are not part of our community. Their review standards are governed entirely by their own projects, not by us.

This section is not a request for special treatment of agent contributions. It is the project being honest about which contributions operate under formal cooperation and which do not.

### §4.4 Funder, Sponsor, and Steward Conduct

Financial support of Agentic Commons (whether through grants, donations, or sponsorships) does not confer special standing under this Code. A funder's representative posting in our spaces is held to the same §2 standard as any other participant.

The Trust & Safety contact in §7 will not give weight to the funding relationship of a reported party when determining a response. A Trust & Safety contact who has a direct reporting or oversight relationship with the funder in question must disclose it and recuse themselves — the case is then handled under the escalation path in §7. A recusal triggered by a funding relationship is noted in the moderator log (without naming the funder) so that the composition of the deciding body can be later reviewed.

---

## §5 Spam, Brigading, and Coordinated Inauthentic Behavior

In addition to the §2 standards, the following are explicitly prohibited:

- **Spam**: high-volume off-topic posting; promotional content for unrelated commercial products; cryptocurrency / token / NFT solicitation.
- **Brigading**: organizing external participants to flood a vote, poll, RFC discussion, or moderation thread.
- **Coordinated inauthentic behavior**: operating multiple accounts across community spaces to manufacture the appearance of consensus or grassroots support.
- **Mass unsolicited DMs**: contacting Discord members or GitHub users at scale without prior conversational context, regardless of message content.

Enforcement of §5 violations follows the §8 ladder: first occurrences typically receive §8.2 (Warning) or §8.3 (Temporary Ban), with §8.4 (Permanent Ban) reserved for repeat or coordinated patterns. The following unambiguous patterns may be acted on at §8.4 without prior warning:

- Bulk cryptocurrency / token / NFT solicitation posts (≥3 in a 24-hour window, or any single post operating at scale).
- Confirmed coordinated account networks operated for inauthentic engagement.
- Mass DM campaigns at scale (≥10 unsolicited DMs from the same sender within a 24-hour window).

---

## §6 Reporting

Instances of abusive, harassing, or otherwise unacceptable behavior may be reported to the project's Trust & Safety contact at:

> **`coc@agentic-commons.org`**

This address routes to:

- **Currently** — while the project is held in trust by its founding contributor: the Trust & Safety lead at Obiwan Co., Limited.
- **Once the Agentic Commons Foundation is operational**: a Code of Conduct committee appointed by the Foundation board, with at least one committee member who is not also a project maintainer.

All complaints will be reviewed and investigated promptly and fairly.

You may report anonymously by sending mail through a service that does not associate your identity with the message. Anonymous reports are evaluated on the same evidentiary standard as named reports. Because we cannot contact an anonymous reporter for clarification or follow-up, a report must contain sufficient standalone evidence to be actionable — we will act when the evidence is sufficient regardless of the reporter's identity.

All community leaders are obligated to respect the privacy and security of the reporter of any incident.

**Retaliation protection**: Retaliation against a reporter — including disclosure of their identity, social pressure, harassment, or any adverse action causally linked to the report — is itself a violation under §2 and is sanctioned independently of the original case.

---

## §7 Trust & Safety Contact and Conflicts

| Period | Contact | Conflict-of-interest recusal |
|--------|---------|------------------------------|
| Currently (until the Agentic Commons Foundation is operational) | `coc@agentic-commons.org` → Obiwan Co., Limited Trust & Safety lead | Recuses when they have a personal or close professional relationship with the reported party (co-authorship, shared employment history, prior consulting, family or romantic relationship). The routine commercial relationship between Obiwan / ClawGrid and a customer who is the reported party is not by itself a recusal trigger; the lead discloses it in the moderator log instead. |
| After Foundation incorporation | `coc@agentic-commons.org` → Foundation CoC committee (≥3 members, ≥1 non-maintainer) | Each member recuses on the same basis as above. |

If the reported party is a maintainer, the Trust & Safety lead, or a CoC committee member themselves, the case is escalated as follows:

- **Currently**: to the project maintainer with the longest continuous project tenure who is not the reported party and has no disclosed conflict. If no such maintainer exists, to the Obiwan Co., Limited officer responsible for the Agentic Commons project.
- **After Foundation incorporation**: to the Foundation board, who appoint an ad-hoc reviewer outside the regular CoC committee.

A redacted aggregate transparency report (counts by category, no identifying details) is published at `@agentic-commons-foundation/transparency` once that repository is established.

---

## §8 Enforcement Guidelines

Community leaders will follow these Community Impact Guidelines in determining the consequences for any action they deem in violation of this Code of Conduct.

### §8.1 Correction

**Community Impact**: Use of inappropriate language or other behavior deemed unprofessional or unwelcome in the community.

**Consequence**: A private, written warning from community leaders, providing clarity around the nature of the violation and an explanation of why the behavior was inappropriate. A public apology may be requested.

### §8.2 Warning

**Community Impact**: A violation through a single incident or series of actions.

**Consequence**: A warning with consequences for continued behavior. No interaction with the people involved, including unsolicited interaction with those enforcing the Code of Conduct, for a specified period of time. This includes avoiding interactions in community spaces as well as external channels like social media. Violating these terms may lead to a temporary or permanent ban.

### §8.3 Temporary Ban

**Community Impact**: A serious violation of community standards, including sustained inappropriate behavior.

**Consequence**: A temporary ban from any sort of interaction or public communication with the community for a specified period of time. No public or private interaction with the people involved, including unsolicited interaction with those enforcing the Code of Conduct, is allowed during this period. Violating these terms may lead to a permanent ban.

### §8.4 Permanent Ban

**Community Impact**: Demonstrating a pattern of violation of community standards, including sustained inappropriate behavior, harassment of an individual, or aggression toward or disparagement of classes of individuals; or, a single act of severe behavior including (but not limited to) doxing, stalking, sustained spam, or threats of violence.

**Consequence**: A permanent ban from any sort of public interaction within the Agentic Commons community.

A ban applied under §4.2 is enforced across all spaces listed in §3.

### §8.5 Appeal

A contributor sanctioned under §8.1–§8.4 may appeal once, in writing to `coc@agentic-commons.org`, within 30 days of the original decision. The appeal must state what aspect of the decision is being challenged: the finding of fact, the categorization of severity, or the chosen consequence.

An additional appeal may be filed — regardless of the 30-day window — if substantial new evidence emerges that was not available at the time of the original decision or the initial appeal. The additional appeal is limited to claims that rely on the new evidence.

The appeal is reviewed by:

- **Currently**: a project maintainer who did not participate in the original action and has no disclosed conflict.
- **After Foundation incorporation**: a CoC committee member who was not involved in the original decision.

Appeal outcomes: uphold, reduce, or reverse. The appeal decision is final and recorded alongside the original case in the moderator log.

---

## §9 Maintenance and Attribution

### §9.1 When this Code needs revision

This Code is intended to be a stable, slow-changing document. Most operational changes to the project — new platform handles, channel renames, role additions — should be tracked in the relevant external registry, not in this Code.

**Routine changes that do NOT require revising this Code**:

- Adding, removing, renaming, or changing the status of a social media or community handle. Tracked in [`agentic-commons-foundation/official-accounts`](https://github.com/agentic-commons-foundation/official-accounts).
- Adding or renaming Discord channels and roles. Tracked in the project's Discord configuration.
- Adding new repositories under the GitHub Organization. Inherited automatically via the `.github` repository default community files.
- Updating `coc@`, `security@`, `hello@` mail routing, provided the receiving inbox remains monitored. Tracked in the project's governance repository.

**Changes that DO require revising this Code**:

- Adding a new *kind* of community space that does not fit any existing §3 category (e.g., the project starts operating in a fundamentally different platform paradigm, such as a federated network with materially different moderation primitives).
- Materially changing an existing space's enforcement model (e.g., moving from maintainer-controlled moderation to community-controlled moderation).
- Changing the legal entity holding the project (e.g., the planned transition from Obiwan Co., Limited to the Agentic Commons Foundation).
- Adding, removing, or substantially rewording any §4 project-specific provision.
- Changing the §6 reporting address, the §7 Trust & Safety contact structure, or the §8 enforcement ladder.
- Any change that would alter the substantive obligations of contributors or the project under this Code.

When this Code is revised, the previous version remains accessible in git history; pull requests modifying this Code should document the rationale in the commit message and reference any related case (anonymized) that motivated the change.

### §9.2 Attribution

This Code of Conduct is adapted from the [Contributor Covenant](https://www.contributor-covenant.org), version 2.1, available at https://www.contributor-covenant.org/version/2/1/code_of_conduct.html.

Community Impact Guidelines were inspired by [Mozilla's code of conduct enforcement ladder](https://github.com/mozilla/diversity).

For answers to common questions about this code of conduct, see the FAQ at https://www.contributor-covenant.org/faq. Translations are available at https://www.contributor-covenant.org/translations.

**Modifications from upstream Contributor Covenant 2.1**:

- "the Agentic Commons community" substituted for "our community" throughout §1, §2, and §8.4.
- §0 (Preamble), §3 (Scope), §4 (Project-Specific Provisions), §5 (Spam, Brigading, Coordinated Inauthentic Behavior), §6 (Reporting), §7 (Trust & Safety Contact and Conflicts), §8.5 (Appeal), and §9.1 (Maintenance) added as original content.
- §3 "Impersonation" and "Pre-launch / silent reservations" clauses added as original content.
- §6 retaliation-protection clause added as original content.

Project-specific additions (§0, §3, §4–§7, §8.5, §9.1, §6 retaliation clause) are licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) — the same license as the underlying Contributor Covenant.
