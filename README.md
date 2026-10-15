# Delivery and Implementation · `[ORG]AIOC-DI`

> **Delivery and Implementation in one page**
>
> Delivery and Implementation (DI) takes an organisation's decided design into a running organisation, and stays to run and improve it with the organisation. It is the last stage of the design chain, after Process and Position Design.
>
> **What goes in:** the decided Process and Position Design release with the operating model it was designed from (mode A), or a design made elsewhere, filed in Source Lifecycle (mode B). Mode C, no design yet, comes in a later slice.
>
> **What comes out in slice 1, the gap audit and the launch essentials:** the gap report in two tiers (what blocks launch; what is incomplete); the organisation health check; the procedures under each process; briefs for counsel and finance; the transition plan and the go-live criteria; and answers to any position's questions, grounded in the decided design with verified citations, or "I do not know". The organisation decides each element. The launch package is filed in Source Lifecycle.
>
> **It decides nothing.** In this version it reads and proposes only; a draft enters a record only when a position inserts it; the go or no-go is the deciding position's; any accountable position can stop it at once. It works at the level of processes and units, never persons.

The writing repository of **`[ORG]AIOC-DI`, Delivery and Implementation**: the mother text of the 49GAION Library part of the same name (49GAION Standard §3.1, item 5, and its Protocol section, both proposed on 15 October 2026). In each organisation this repository is named `<org>aioc-di` (Naming Standard R9). It is written for any organisation and holds no organisation data.

**Status: draft `v0.1.1`, slice 1 of 4, 16 October 2026 (`decisions/DR-0002`). Nothing here has run; every fixed test reads `NOT_RUN`.**

## Where to read

| File | What it is |
|---|---|
| [`blueprint/DI-BLUEPRINT.md`](blueprint/DI-BLUEPRINT.md) | the blueprint, on the 49GAION AIOC Blueprint Template at `e89ed1d`: identity, card, placement, positions, the five stages with their inputs, outputs and done-tests (§5.0), every capability, the human decisions (§13), Cells and Pods (§17), the package parts (Annex A), the gap checks (Annex F) |
| [`tests/TEST-DI.md`](tests/TEST-DI.md) | the fixed test, written before use: 48 cases and the Delivery Lead's seat test |
| [`cards/`](cards/) | the unit cards of its four Pods and thirteen Cells, and the bot identity cards of its twelve AI Cells, generated from the blueprint |
| [`docs/HISTORY.md`](docs/HISTORY.md) | why this stage exists |
| [`upstream/PROPOSALS.md`](upstream/PROPOSALS.md) | the changes this AIOC needs from Process and Position Design, the target operating model and Source Lifecycle |
| [`decisions/`](decisions/) | the decision records of this repository |

Returns follow the Library's design return contract, `library/contracts/design-return.schema.json` of `49GAION-protocol`.

## Checks

```
python3 tools/make_cards.py <49GAION-protocol>/spec/schemas
```

It must report 0 errors.

## How a change is made

A change is a pull request, reviewed by someone other than its writer. A decided text is never edited; a change is a new version that names what it supersedes.

*Powered by 49GAION*
