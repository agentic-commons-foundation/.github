---
name: RFC proposal (protocol change)
about: Propose a change to the ACG protocol or a related specification
title: "[RFC] "
labels: rfc
assignees: ''
---

> RFCs go through a structured discussion process. See [`CONTRIBUTING.md` §3](../CONTRIBUTING.md) for the full lifecycle. The minimum is: 14-day discussion window, simple majority of active maintainers, no remaining blocking concerns, decision recorded as an ADR in `governance/adrs/`.
>
> If your proposal is not a protocol change, use the Feature Request template instead.

## Summary

<!-- One paragraph: what change to the protocol, and why. -->

## Motivation

<!-- What problem does this solve? Who has the problem (agent runtime authors, project maintainers, funders, registry operators)? Concrete examples beat abstract claims. -->

## Detailed proposal

<!-- The actual change. Be specific about wire format, marker syntax, registry behavior, etc. If the change is to spec/X.md, paste the proposed diff or link to a draft branch. -->

## Migration path

How do existing implementations move to the new behavior?

- Backwards-compatible? (yes / no — and if no, what breaks)
- Versioning strategy (new field with default? new spec version? deprecation period?)
- Required changes in: `sdk-python` / `sdk-typescript` / `marker-validator` / `cli` / `guides`

## Alternatives considered

<!-- Other designs and why this one is preferable. Acceptable answers include "we considered doing nothing — that means X stays broken". -->

## Out of scope

<!-- What this RFC is *not* doing, to keep the discussion bounded. -->

## Security and privacy

<!-- Any signing, identity, or data-leak implications? -->

## Open questions

<!-- Things you don't know yet and want input on. -->

---

By submitting this RFC I agree to follow the [Code of Conduct](../CODE_OF_CONDUCT.md). Final discussion happens in the [`spec` Discussions, RFC category](https://github.com/agentic-commons-foundation/spec/discussions/categories/rfc) — this issue exists to track lifecycle state (draft → discussion → accepted/rejected → ADR recorded).
