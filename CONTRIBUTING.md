# Contributing

**`[ORG]AIOC-DI` v0.1.0 · 15 October 2026.**

1. **One change, one pull request**, reviewed by someone other than its writer.
2. **Positions, never people.** No person's name in any file. Who occupies a position is top management's own mechanism, never here (49GAION Standard §1.1, item 9).
3. **No organisation data.** This repository is written for any organisation. An organisation's values, sources and run records live in its own records repository.
4. **Cite every rule** to its source: a 49GAION text by section and version, a carried rule by the TOM blueprint section and version (blueprint Annex E), a requirement by its ID in `PRD-[ORG]AIOC-DI-001`. Never invent a fact, a version or a score. `NOT_RUN` is never PASS.
5. **The blueprint governs the cards.** Edit the card data block of blueprint §17 only, then run `python3 tools/make_cards.py <49GAION-protocol/spec/schemas>`. It must report 0 errors.
6. **Returns use the Library contract** (`library/contracts/design-return.schema.json` of `49GAION-protocol`); this repository keeps no copy of it.
7. **Decided texts are never edited.** A change is a new version that names what it supersedes.
8. **English only, plain and short.**

*Powered by 49GAION*
