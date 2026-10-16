```yaml
# ── Blueprint metadata (machine-readable; the panel generator and the back-office builder read this block) ──
blueprint:
  aioc: "[ORG]AIOC-DI"
  parent: "[ORG]AIOC-CH"                  # example code of the Charter; each organisation writes its own Charter's code (Standard §1.7, item 13)
  full_name: "Delivery and Implementation"
  organisation: "<organisation>"          # filled in each organisation's own copy
  type: "specialised"
  org_aion: "[ORG]AION"
  blueprint_version: "v0.1.2"
  status: "draft"
  template:
    name: "49GAION AIOC Blueprint Template"
    version: "v1.5.0, with the unreleased v1.6.0 additions on main"
    source: "github.com/49g-holding/49GAION-aioc, template/AIOC-BLUEPRINT-TEMPLATE.md @ e89ed1d"
  mother:
    name: "49GAION Delivery and Implementation"
    version: "part card v1 (DRAFT)"
    source: "github.com/49g-holding/49GAION-protocol, library/cards/delivery-and-implementation.part-card.json and the Protocol section Delivery and Implementation (pull request #36); Standard §3.1, item 5 (49GAION pull request #68, DR-0017)"
  writing_repository: "<org>aioc-di"
  code_project: "<org>aioc-di, on the organisation's code platform"
  panel_register_id: "none yet"
  slice: "1 of 4: gap audit and launch essentials"
  capabilities:
    standard: ["Chief of Staff", "Office", "Input socket", "Panel"]
    functional: ["Intake and Design Map", "Needs Requests", "Gap Audit", "Health Check", "Procedure Writing", "Briefs", "Transition and Go-live Criteria", "Answers", "Independent Review", "Decision Package and Filing"]
```

# Blueprint · `[ORG]AIOC-DI` · Delivery and Implementation · `v0.1.2`

**Draft, 15 October 2026; v0.1.1, 16 October 2026, receives the answers to its returns and the release notices of `[ORG]AIOC-PPD` under their contracts, now that both stages before it are connected (`decisions/DR-0002`). v0.1.2, 16 October 2026, carries the value case of the TOM Release and the priority of each element, unchanged, and orders the transition waves by priority (`decisions/DR-0003`; TOM blueprint `v0.6.0`, Annex H).** Written by `[ORG]AIOC-OCO` on the directions recorded in `decisions/DR-0001` to `decisions/DR-0003`. This is the first blueprint of Delivery and Implementation, written for any organisation as the mother text of the Library part 49GAION Delivery and Implementation. It covers **slice 1 of 4, the gap audit and the launch essentials**, which the governing seat started first. The later slices are named in §5.0 and come as later versions. Every rule rests on a 49GAION text, on the blueprints of `[ORG]AIOC-PPD` or `[ORG]AIOC-TOM` (cited by section and version), or on the product requirements of this part (`PRD-[ORG]AIOC-DI-001` v0.4, in its code project), or is new here and marked **New**. Nothing here has run. Every fixed test reads `NOT_RUN`.

> **Delivery and Implementation in one page**
>
> Delivery and Implementation (DI) takes an organisation's decided design into a running organisation, and stays to run and improve it with the organisation. It is the last stage of the design chain, after Process and Position Design (PPD).
>
> **What goes in (this version)**
> 1. **Mode A:** the decided PPD release, handed over directly by `[ORG]AIOC-PPD`, by reference and hash, with the decided TOM release it was designed from.
> 2. **Mode B:** a design made elsewhere, filed as a source in Source Lifecycle.
> 3. The organisation's other sources, only from Source Lifecycle, and answers to what they do not say, asked only through its Chief of Staff.
>
> Mode C (no design yet) comes in slice 4.
>
> **What DI does in slice 1, in five stages**
> 1. **Admit:** check the request, the design, the connections and the deciding positions.
> 2. **Map:** in mode A, account for every element of the release; in mode B, map the outside design onto the structure of a PPD release, showing what mapped, what did not and why. Defects of a release go back to the stage that made it.
> 3. **Diagnose:** the gap audit, in two tiers (what blocks launch; what is incomplete), each gap with its consequence, evidence and proposed fix; and the organisation health check at entry.
> 4. **Prepare:** the procedures under each process, critical processes first; briefs for counsel and finance (policies, pay structure, contracts, authority instruments, obligations, controls, systems and suppliers); the transition plan and the go-live criteria.
> 5. **Decide and file:** the organisation decides each element; the launch package is filed in Source Lifecycle.
>
> All the while, any position may ask DI how the organisation works. DI answers only from the decided design, citing the element, its version and a quoted span, and a second engine checks every citation. Where the design is silent, DI says it does not know.
>
> **Who decides.** DI decides nothing for the organisation. In this version it reads and proposes only: a draft enters a record only when a position inserts it. The go or no-go is always the deciding position's. Any accountable position can stop DI at once.
>
> **Processes, not persons.** DI addresses positions only, never ranks, scores or watches the occupant of a position, and shows no measure for a single position.

**Where this blueprint stands.** First draft, slice 1. The stages, their inputs, outputs and done-tests are set (§5.0). The review rule it shares with `[ORG]AIOC-PPD` and `[ORG]AIOC-TOM` is carried by section (§5.9; Annex E). The decisions only a human seat can take are listed once, in §13.

---

## 0. Identity and lineage

| Field | Value |
|---|---|
| Code | `[ORG]AIOC-DI`. Collision check (Naming Standard §5 and R6): the initials do not recreate `AIOC`, `AION` or `49GAION`, and do not read as a version suffix. The code is the one the Library part's Protocol section gives it in an `[ORG]AION`. Each organisation records it in its register before the repository is created (Naming Standard R9) |
| Full name | Delivery and Implementation |
| Description | "`[ORG]AIOC-DI` is `<organisation>`'s Delivery and Implementation core, built from 49GAION Delivery and Implementation" |
| Kind | AIOC |
| Parent | `<code of the Charter of this [ORG]AION>`; the cards use the example code `[ORG]AIOC-CH`. A top-level AIOC (Standard §1.7, item 13) |
| Inner units | `[ORG]CELL-DDL`, `[ORG]CELL-DCS`, `[ORG]POD-DD`, `[ORG]POD-DP`, `[ORG]POD-DA`, `[ORG]POD-DR`: four Pods with their eleven Cells, and two Cells directly under the AIOC (§17). No inner AIOC |
| HOAC label | `[ORG]HOAC-ACS`, held by its top Cell, the DI Delivery Lead `[ORG]CELL-DDL` (`label_holder`) |
| Accountable to | `<code of the Cell carrying [ORG]HOAC-TM>`; the cards use the example code `[ORG]CELL-TMS` (Naming Standard R15) |
| Type | Specialised: the organisation needs its decided design taken into a running organisation (§16) |
| `[ORG]AION` | `[ORG]AION`, based on 49GAION Standard `v1.5.0`, with the unreleased `v1.6.0` texts on main |
| Versioned Definition | this file; the Panel and the Back office are built from it |
| Organisation | `<organisation>` |
| Made from | the Library part 49GAION Delivery and Implementation, part card `v1` (DRAFT), and its Protocol section, both merged on 15 October 2026 (`decisions/DR-0001`) |
| Template | 49GAION AIOC Blueprint Template `v1.5.0` at `e89ed1d` (with the `v1.6.0` additions) |
| Mother | 49GAION Delivery and Implementation, part card `v1`. This text is its mother blueprint |
| Product requirements | `PRD-[ORG]AIOC-DI-001` v0.4, approved by the governing seat on 15 October 2026; its requirement IDs (`FR-n`, `NFR-n`) are cited here |
| Blueprint version and status | `v0.1.2` · draft · slice 1 |
| Accountable seat (`[ORG]HOAC-ACS`) | the DI Delivery Lead, `[ORG]CELL-DDL`, a HOAC position. Who occupies it is top management's own mechanism; this AIOC never sees it (Standard §1.1, items 9 and 10) |
| Reports to | the Cell carrying `[ORG]HOAC-TM` |
| Writing repository | `<org>aioc-di`, plus `-records` for an organisation's runs and `-records-restricted` for run records that touch a Strictly confidential source (Naming Standard R9). The mother text lives in a public repository and holds no organisation data |
| Code project | `<org>aioc-di`, on the organisation's code platform; it holds the product requirements and the code |
| Panel | not yet built |
| Back office | not yet built |
| Attribution | Powered by 49GAION |

**Lineage.** A review of what an organisation still needs, after its processes and positions are designed, to start working without AI found that the decided design is not yet a working organisation: procedures, policy and pay drafts, authority instruments, controls, the transition plan and the go-live criteria are still missing, and the organisation needs someone beside it through launch and after. The governing seat directed a stage of its own for that, with an assistant that stays (`decisions/DR-0001`; `49GAION/DR-0017`). A study of fifteen products that design, launch or run organisations then placed each useful feature in the stage where it truly belongs. Both are summarised in `docs/HISTORY.md`. No earlier code or result is carried here.

---

## 1. Card (49GAION Operating Protocol §3)

```yaml
card:
  unit_kind: "AIOC"
  code: "[ORG]AIOC-DI"
  parent: "[ORG]AIOC-CH"                  # example code of the Charter, the root AIOC; only it has parent none (Standard §1.7, item 13)
  inner_units: ["[ORG]CELL-DDL", "[ORG]CELL-DCS", "[ORG]POD-DD", "[ORG]POD-DP", "[ORG]POD-DA", "[ORG]POD-DR"]
  type: "specialised"
  org_aion: "[ORG]AION"
  card_version: "v0.1.2"
  input_door: "Chief of Staff"
  wake: { method: "queue", verified: false }
  receives:
    - kind: "run request"                 # a Work Item from the Requesting Authority's Cell, through the HU input port; references only
      format: "Work Item (Protocol §4.1) whose sources field holds the mode (A or B), and either one PPD Release reference or the reference of a design filed in Source Lifecycle"
      acceptance_test: "TEST-DI v1, cases 1, 18, 19"
      decision_needed: false
    - kind: "release notice"              # from [ORG]AIOC-PPD, directly, through the tool gateway
      format: "release notice of [ORG]AIOC-PPD (its contracts/release-notice.schema.json, urn:49gaion:library:ppd:release-notice:v0.4): the PPD Release ID, version and manifest hash, the TOM Release it rests on, its filed reference, and the returns it answers"
      acceptance_test: "TEST-DI v1, cases 1, 20, 48"
      decision_needed: false
    - kind: "return answer"               # from [ORG]AIOC-PPD or [ORG]AIOC-TOM: the end, or the next round, of a return this AIOC sent
      format: "the return at its next version (49GAION-protocol library/contracts/design-return.schema.json)"
      acceptance_test: "TEST-DI v1, case 48"
      decision_needed: false
    - kind: "source reference"            # the outside design (mode B) and the organisation's other sources, from the output socket of [ORG]AIOC-SL
      format: "source reference (ID + version + hash; held or not held)"
      acceptance_test: "TEST-DI v1, cases 2, 21"
      decision_needed: false
    - kind: "needs answer"
      format: "needs answer, by reference only"
      acceptance_test: "TEST-DI v1, case 22"
      decision_needed: false
    - kind: "needs status"
      format: "needs status"
      acceptance_test: "TEST-DI v1, case 22"
      decision_needed: false
    - kind: "question"                    # from any position of the organisation, through the HU input port; never a source
      format: "question from a position (its position code), text only"
      acceptance_test: "TEST-DI v1, cases 7, 36, 37"
      decision_needed: false
  delivers:
    - kind: "return"                      # to the stage that made the release; also filed into [ORG]AIOC-SL as a design report
      format: "design return (49GAION-protocol library/contracts/design-return.schema.json), prefix DIR"
      usual_receivers: ["[ORG]AIOC-PPD", "[ORG]AIOC-TOM", "[ORG]AIOC-SL"]
    - kind: "needs request"
      format: "needs request, as a sub-item of the run Work Item"
      usual_receivers: ["[ORG]AIOC-SL"]
    - kind: "missing report"
      format: "Missing Report, one per pass"
      usual_receivers: ["[ORG]AIOC-SL"]
    - kind: "launch package filing"
      format: "launch package manifest and its parts (Annex A), filed as a source of origin kind delivery and implementation; filing receipt"
      usual_receivers: ["[ORG]AIOC-SL"]
    - kind: "answer"
      format: "answer with its citations (Annex A.7), or 'I do not know'; to the asking position only"
      usual_receivers: ["the asking position"]
  anatomy:
    panel: { health: { tests: true, metrics: ["stuck", "returned", "late", "run state", "returns open", "returns answered", "needs open", "needs past deadline", "gaps by tier", "gaps by state", "procedures by state", "briefs by state", "go-live criteria by state", "answers given", "answers 'I do not know'", "citations refused by the verifier", "reviews held", "review budget used"] } }
    back_office: { converses_with_humans: true, hosts: ["Chief of Staff", "Office"], protocol_traffic: true }
    definition: { location: "<org>aioc-di, blueprint/DI-BLUEPRINT.md", version: "v0.1.2" }
    delivery: { rollback: "one-click" }
    connectors:
      - { role: "design source", connector: "[ORG]AIOC-PPD release port", access_managed_in: "panel" }   # the grant is signed at the tool gateway as connect-external-port
      - { role: "returns to the operating model", connector: "[ORG]AIOC-TOM return port", access_managed_in: "panel" }
      - { role: "source of record", connector: "[ORG]AIOC-SL output socket", access_managed_in: "panel" }      # as above (Protocol §13, item 5)
    gateway: { metering_id: "<per-AIOC metering id>" }
  full_name: "Delivery and Implementation"
  version: "0.1.2"
  lineage: { id: "[ORG]AIOC-DI", version: "0.1.2", relation: "original" }
  lifecycle_state: "designed"
  blueprint_version: "v0.1.2"
  template_version: "v1.5.0"
  accountable_to: "[ORG]CELL-TMS"         # example code of the Cell carrying [ORG]HOAC-TM (Naming Standard R15); never a Cell inside this AIOC
  top_cell: "[ORG]CELL-DDL"
  hoac: "[ORG]HOAC-ACS"
  label_holder: "[ORG]CELL-DDL"
  fixed_test: { id: "TEST-DI", version: "v1", owner: "[ORG]CELL-TMS" }
  skills:
    - { id: "di-design-map", name: "Reading a decided design, or mapping a design made elsewhere", tags: ["delivery", "intake"] }
    - { id: "di-gap-audit", name: "The gap audit in two tiers, and the organisation health check", tags: ["delivery", "diagnosis"] }
    - { id: "di-procedures", name: "Procedures under each process", tags: ["delivery"] }
    - { id: "di-briefs", name: "Briefs for counsel and finance", tags: ["delivery"] }
    - { id: "di-transition", name: "Transition plan and go-live criteria", tags: ["delivery"] }
    - { id: "di-answers", name: "Answers grounded in the decided design, with verified citations", tags: ["delivery", "assurance"] }
  ports:
    - { unit: "[ORG]AIOC-DI", port: "ai-in", direction: "input", type: "AI", identification: "technical-key", accepted_content: ["release notice", "return answer", "source reference", "needs answer", "needs status"], authority_limit: "read only, within the scopes signed for the PPD and Source Lifecycle connections; return answers on the PPD and TOM connections", audit_trail: "unit register; the serve logs of [ORG]AIOC-PPD and [ORG]AIOC-SL", required_tests: ["TEST-DI v1"], enforcement: "shared-gateway-outside-unit" }
    - { unit: "[ORG]AIOC-DI", port: "ai-out", direction: "output", type: "AI", identification: "technical-key", accepted_content: ["return", "needs request", "missing report", "needs status", "launch package filing"], authority_limit: "returns, requests, reports and filings only; files only its own packages and design reports; never an instruction to a person", audit_trail: "Work Item record and the unit register", required_tests: ["TEST-DI v1"], enforcement: "shared-gateway-outside-unit" }
    - { unit: "[ORG]AIOC-DI", port: "hu-in", direction: "input", type: "HU", identification: "live-human-sign-in-at-gateway", accepted_content: ["run request from the Requesting Authority's Cell (references only)", "a question from a position about how the organisation works (never a source)", "a decision of a deciding position on a row of the Decision Package", "run control and configuration from the DI Delivery Lead (never a source)"], authority_limit: "the signer's authority_scope; nothing received here is a source", audit_trail: "Office record", required_tests: ["TEST-DI v1"], enforcement: "shared-gateway-outside-unit" }
    - { unit: "[ORG]AIOC-DI", port: "hu-out", direction: "output", type: "HU", identification: "live-human-sign-in-at-gateway", accepted_content: ["answer to the asking position", "run brief to the DI Delivery Lead", "ruling sheets to the DI Delivery Lead", "Decision Package rows to the deciding positions", "filing notice to the Requesting Authority's Cell"], authority_limit: "information and proposals only; never a decision, an instruction or a question about a person", audit_trail: "Office record", required_tests: ["TEST-DI v1"], enforcement: "shared-gateway-outside-unit" }
    - { unit: "[ORG]AIOC-DI", port: "stop", direction: "input", type: "HU", identification: "live-human-sign-in-at-gateway", accepted_content: ["stop"], authority_limit: "stop only; open to every accountable position of the organisation (FR-34)", audit_trail: "unit register", required_tests: ["TEST-DI v1"], enforcement: "shared-gateway-outside-unit", stop_door: true }
  configuration:                          # every slot is set by the organisation (§15); an empty slot fails the joining test
    office_accountable_human: { value: "<set by the organisation>", set_by: "<position>", date: "<date>", version: "<vN>" }
    central_head: { value: "<the OCO of this [ORG]AION>", set_by: "<position>", date: "<date>", version: "<vN>" }
    discussion_limits: { value: "<set by the organisation>", set_by: "<position>", date: "<date>", version: "<vN>" }
    waiting_deadlines: { value: "<per status>", set_by: "<Cell carrying [ORG]HOAC-TM>", date: "<date>", version: "<vN>" }
    bounce_limit: { value: "<number>", set_by: "<position>", date: "<date>", version: "<vN>" }
    chain_depth: { value: "<number, at least 1>", set_by: "<position>", date: "<date>", version: "<vN>" }
    halt_request_priority: { value: "immediate", set_by: "<position>", date: "<date>", version: "<vN>" }
    budget_cap: { value: "<amount per period>", set_by: "<Cell carrying [ORG]HOAC-TM>", date: "<date>", version: "<vN>" }
    unattended_action: "read-record-triage"
    requesting_authority_cell: { value: "<set by the organisation>", set_by: "<Cell carrying [ORG]HOAC-GOV>", date: "<date>", version: "<vN>" }
    modes_enabled: { value: ["A", "B"], set_by: "<Cell carrying [ORG]HOAC-TM>", date: "<date>", version: "<vN>" }
    rows_per_pass: { value: 12, set_by: "<position>", date: "<date>", version: "<vN>" }
    non_response_passes: { value: "<set by the organisation>", set_by: "<Cell carrying [ORG]HOAC-TM>", date: "<date>", version: "<vN>" }
    return_round_deadline: { value: "<set by the organisation>", set_by: "<Cell carrying [ORG]HOAC-TM>", date: "<date>", version: "<vN>" }
    return_rounds_max: { value: "<set by the organisation>", set_by: "<Cell carrying [ORG]HOAC-TM>", date: "<date>", version: "<vN>" }
    review_engines: { value: 3, set_by: "<position>", date: "<date>", version: "<vN>" }
    review_families_min: { value: 2, set_by: "<position>", date: "<date>", version: "<vN>" }
    reduced_review_permitted: { value: "no", set_by: "<Cell carrying [ORG]HOAC-TM>", date: "<date>", version: "<vN>" }
    review_budget_per_run: { value: "<set by the organisation>", set_by: "<Cell carrying [ORG]HOAC-TM>", date: "<date>", version: "<vN>" }
    gap_bars: { value: "<blocking gaps found, at or above; false gaps, at or below>", set_by: "<Cell carrying [ORG]HOAC-TM>", date: "<date>", version: "<vN>" }
    answer_bars: { value: "<grounded answers, at or above; 'I do not know' on unanswerable questions, at or above>", set_by: "<Cell carrying [ORG]HOAC-TM>", date: "<date>", version: "<vN>" }
    deciding_positions: { value: "<position codes: go or no-go; counsel per jurisdiction; finance>", set_by: "<Requesting Authority Cell>", date: "<date>", version: "<vN>" }
    ladder: { value: "every class at level 1 at most in this version", set_by: "<owner position>", date: "<date>", version: "<vN>" }
```

**Joining the protocol.** This AIOC joins only after every input and output on this card passes fixed samples (the joining test, Protocol §11, item 1; Standard §3.2, item 4). It also needs `[ORG]AIOC-PPD` to send it release notices and accept its returns, `[ORG]AIOC-TOM` to accept its returns, and Source Lifecycle to accept filings of origin kind `delivery and implementation` (`upstream/PROPOSALS.md`, items 1 to 3). Until then its `lifecycle_state` stays `designed` and no Work Item is routed to it. The cards of its Pods and Cells are set in §17 and generated into `cards/`.

---

## 2. Organisation table and placement

### 2.1 Organisation table

The blueprint writes `[ORG]` for the organisation's prefix (Naming Standard R13). Positions only; who occupies each one is top management's own mechanism (Standard §1.1, items 9 and 10).

| Term in the blueprint | In `<organisation>` |
|---|---|
| The Top Office (decisions are signed by human Cells carrying HOAC labels) | `<filled by the organisation>` |
| `[ORG]AIOC-OCO` | `<filled>` |
| The Charter of this `[ORG]AION` | `<code>` |
| The Cell carrying `[ORG]HOAC-TM` | `<code>` |
| The Library blueprint this core is made from | 49GAION Delivery and Implementation, part card `v1`; its Protocol section (§20); this text is its mother blueprint |
| **The Requesting Authority**: the position that asks for the delivery work and decides the launch package | `<code of the human Cell carrying [ORG]HOAC-GOV>`, or of a human Cell carrying a HOAC label whose `authority_scope`, delegated by that Cell under `delegate-authority`, covers these decisions (Standard §4.2, items 5 and 8; §4.4, item 8). It is a position, never this AIOC's Delivery Lead |
| **The deciding positions** | position codes set by the Requesting Authority (`deciding_positions`): the position that decides go or no-go; the counsel position for each jurisdiction; the finance position. Each is a position of the organisation's decided design, never of this AIOC |
| **The DI Delivery Lead position** | a HOAC position (`[ORG]HOAC-ACS`), a legal persona. Who occupies it is top management's own mechanism; this AIOC never sees it |
| **The design source** | `[ORG]AIOC-PPD`: it hands over its decided release directly, and receives this AIOC's returns on it |
| **The operating model** | `[ORG]AIOC-TOM`: its decided release is read by reference from Source Lifecycle; it receives this AIOC's returns on it |
| **The source of record** | `[ORG]AIOC-SL`: every other source, every question to the organisation, and every filing |
| **The engine register** | held at the tool gateway, in the Charter (Standard §4.4, item 11); read as `[ORG]AIOC-TOM` reads it (TOM blueprint `v0.5.0`, Annex E.12) |

### 2.2 Placement

- **Where it sits.** A top-level AIOC under the Charter, beside `[ORG]AIOC-SL`, `[ORG]AIOC-TOM` and `[ORG]AIOC-PPD`. It is the last stage of the design chain.
- **Its role.** It takes the decided design into a running organisation and stays with it. In this version (slice 1) it does the gap audit and prepares the launch essentials.
- **Scope in this version.**
  - **It does:** admit a decided PPD release (mode A) or a design made elsewhere (mode B); map it; return every defect of a release to the stage that made it; audit the gaps in two tiers; run the organisation health check at entry; write the procedures under each process; write briefs for counsel and finance; draft the transition plan and the go-live criteria; answer positions' questions from the decided design, with verified citations; trace every artefact both ways; prepare the decision; file the launch package.
  - **It does not:** decide anything for the organisation, the go or no-go included; give legal, tax, employment or pay advice; set an amount; ask any person anything about the organisation; name a person, or read who occupies a position; rank, score or watch the occupant of a position; change a design release; read records of work (slice 3); apply any change (ladder level 2 is not in this version); start from no design (mode C, slice 4).
- **Shapes it serves.** Any shape the design covers: one owner's work, a single entity, a group of entities, or a group with independent institutions inside it. Where a design covers several entities or jurisdictions, every brief and every go-live criterion records its entity and jurisdiction.
- **Boundaries with other AIOCs.**
  - **`[ORG]AIOC-PPD`** designs processes, positions and units. This AIOC reads its decided release and returns defects; it never redesigns. A return is a request, never a change (§5.1; Annex B).
  - **`[ORG]AIOC-TOM`** designs the operating model. A defect this AIOC finds in a TOM element goes back to TOM by return.
  - **`[ORG]AIOC-SL`** holds every source and every contact with a person. This AIOC holds only references and its own records, and files its package and its returns there.
  - **`[ORG]AIOC-OCO`** installs, fixes and upgrades this AIOC; it never grades it (Standard §2.3, item 9).
- **Overlap.** None known. Where an organisation already holds procedures, policies or plans, they are sources, read through Source Lifecycle and mapped (§5.1).

---

## 3. Positions

| Position (standard title) | Purpose | Reports to | Run today by | Deputy |
|---|---|---|---|---|
| DI Delivery Lead | the accountable position of this AIOC and the owner of its path: owns the fixed tests of its parts; rules on contested review findings; accepts a reduced review level within the TM Cell's permission; attests the method. Answers for the method, never for the organisation's choices | the Cell carrying `[ORG]HOAC-TM` | a HOAC position (`[ORG]HOAC-ACS`); who occupies it is top management's own mechanism, never seen by this AIOC | as top management arranges (`appoint-acting-filler`, Standard §4.1, item 12) |
| Chief of Staff | keep each run moving, honest and traced; the only door to PPD, TOM and Source Lifecycle | DI Delivery Lead | an agent (`[ORG]CELL-DCS`) | none; the run halts |
| Design Mapper | read a decided release, or map a design made elsewhere, and draft returns | Chief of Staff | an agent (`[ORG]CELL-DDM`) | none; the step halts |
| Gap Auditor | run the gap checks in two tiers | Chief of Staff | an agent (`[ORG]CELL-DGA`) | none; the step halts |
| Health Checker | run the organisation health check at entry | Chief of Staff | an agent (`[ORG]CELL-DHC`) | none; the step halts |
| Procedure Writer | write the procedure under each process | Chief of Staff | an agent (`[ORG]CELL-DPW`) | none; the step halts |
| Brief Writer | write the briefs for counsel and finance | Chief of Staff | an agent (`[ORG]CELL-DBW`) | none; the step halts |
| Transition Planner | draft the transition plan and the go-live criteria | Chief of Staff | an agent (`[ORG]CELL-DTP`) | none; the step halts |
| Answer Guide | draft each answer from the decided design | Chief of Staff | an agent (`[ORG]CELL-DAG`) | none; the question waits |
| Citation Verifier | check that each citation of an answer or a draft resolves and supports it | Chief of Staff | an agent (`[ORG]CELL-DCV`), on an engine of another family than the writer's | none; the answer waits |
| Blind Reviewer, seats A–C | review a locked output, alone first, then in debate | Chief of Staff | agents (`[ORG]CELL-DBRA` to `[ORG]CELL-DBRC`) | none; any seat covers another |

- **Every human position is a HOAC position.** This AIOC has one, the DI Delivery Lead. The organisation may add more in this AIOC's own design (§17).
- **Present as positions** (Standard §1.1, items 9 and 10). Every human this AIOC deals with, its own Lead and the organisation's positions, is present as a position. It addresses positions only, through their HU ports.
- The **Requesting Authority** and the **deciding positions** are not positions of this AIOC (§2.1). They decide; this AIOC prepares the decision.
- No AI Cell signs anything (Protocol §10, item 3). Each AI Cell's bot has its own identity card (§17).
- The trace query, the package manifest and the checks of §5 are code steps of the Chief of Staff, never a Cell. Code is a tool, never a seat.

---

## 4. Standard capabilities

Defaults are in `docs/STANDARD-CAPABILITIES.md` of `49GAION-aioc` at `e89ed1d` (`v1.5.0`, with the `v1.6.0` additions). The differences are listed in §11.

### 4.1 Office
#### Definition
Default · form: **single Chief of Staff**. An Office forms only if the Delivery Lead needs more than one Chief of Staff; it is proposed to the Delivery Lead, never self-created.
#### Process (SOP)
Default.
#### Role card
None while the form is a single Chief of Staff.
#### Fixed test
TEST-DI-DCS v1 (TEST-DI v1, case 44) · result `NOT_RUN`

### 4.2 Chief of Staff
#### Definition
Default, **managing** kind, with these additions:
- **The only door.** It is the only Cell of this AIOC that sends anything outside it: returns to `[ORG]AIOC-PPD` and `[ORG]AIOC-TOM`; needs requests, Missing Reports and filings to `[ORG]AIOC-SL`; answers and Decision Package rows to positions, through the HU output port. The external ports sit on its card (§17).
- **No question about a person, and none to a person about the organisation.** Every question for the organisation goes to the Chief of Staff of `[ORG]AIOC-SL` as a needs request (§5.2). It sends a position only an answer it was asked for, a Decision Package row, or a notice.
- **An orchestrator that never judges itself.** It runs the gates (Annex C), dispatches the Cells, locks outputs, runs the code steps, draws the reviewers and writes the run record. It never rules on a finding, never dismisses or downgrades one, never lowers a review, and never decides for a deciding position.
#### Process (SOP)
Default, plus:
1. **Admission (S0).** On a run request: open the run record; check that the request carries references only and names an enabled mode; receive or fetch the release notice (mode A) or the design's source reference (mode B); have the Input socket build Input Pack P0 (§4.3); check gate T0 (Annex C.2) → *P0 and the T0 record* (evidence: the T0 record, with P0's ID).
2. **One run at a time per organisation.** A second run in parallel needs the Delivery Lead's approval, recorded in the run record.
3. **Returns.** Collect the return drafts; have each reviewed; send each to the stage that made the release, under the design return contract, and file it into `[ORG]AIOC-SL` with the same hash; mark the elements it touches `held: return open`; count its rounds; past `return_round_deadline` or `return_rounds_max`, put it to the Requesting Authority, who answers it or sets it aside on a stated basis → *return sent; return ended* (evidence: the return, its filing receipt and its end).
4. **Passes.** Batch needs candidates into passes of at most `rows_per_pass` rows, one decision per row, each with its Missing Report.
5. **Questions.** On a question from a position, dispatch the Answer Guide, then the Citation Verifier; send the verified answer, or "I do not know", to the asking position only; record the question by ID, never as a source (§5.8).
6. **Code steps.** Run the checks of §5.1 to §5.7, the trace query (§5.10) and the package manifest → *generated parts* (evidence: re-generated byte-identical).
7. **Stops and revocation.** A stop from any accountable position takes effect at the gateway on every part, and on any draft in flight; the Chief of Staff is itself stopped. A revoked connection holds the run as `held: connection revoked`.
#### Role card
| Field | Content |
|---|---|
| Name | Chief of Staff |
| Position and seat | the position Chief of Staff; accountable seat: the DI Delivery Lead (`[ORG]HOAC-ACS`) |
| Performed by | an agent (`[ORG]CELL-DCS`, full name DI Chief of Staff) |
| Purpose | keep each run moving, honest and traced; be this AIOC's voice to the Delivery Lead and its only door to PPD, TOM, Source Lifecycle and the asking positions |
| Authority limits | alone: dispatch, lock, record, run code steps, send reviewed returns and needs requests, send verified answers, file a package whose elements are decided; needs the Delivery Lead: a second run in parallel, a budget above the cap, any change to configuration, a ruling on a finding, a reduced review level; never: ask a person anything about the organisation, change a design release, decide for a deciding position, insert a draft into a record, rule on or dismiss a finding, sign, close a Work Item this AIOC performed |
| Write location | the run record and this AIOC's Work Items |
| Reports to | the DI Delivery Lead |
| Escalation | to the Delivery Lead in one line, with evidence linked; a stop goes to the stop door, never through this Cell |
| Tools and access | the PPD, TOM and Source Lifecycle connections through the tool gateway, within their signed scopes; the code steps of the code project; no credential in any instruction |
| Deputy and cover | none; on failure the run halts and the Delivery Lead is told |
| Fixed test and score | TEST-DI-DCS v1 (§9), plus the default Chief of Staff test |
| Card version and status | v0.1.0 · draft |
#### Fixed test
TEST-DI-DCS v1 · result `NOT_RUN`

### 4.3 Input socket
#### Definition
Default, with this AIOC's standard format, the **Input Pack**, as in the TOM blueprint `v0.5.0` §4.3, parts 1 to 3 and 6 to 8, read with these changes:
1. **Three kinds of input.** The **releases** (mode A): the decided PPD Release, by manifest and parts, from the release notice, and the decided TOM Release it names, read by reference from Source Lifecycle. The **outside design** (mode B): a source in Source Lifecycle, cut into atoms and labelled once (TOM Annex B, carried). The **other sources**: by reference from Source Lifecycle's output socket.
2. **A release is read, never atomised as a source.** Its elements keep their own IDs. Every element of this AIOC's output traces to a release element or a source atom.
3. **The release check.** A release is admitted only when its manifest validates, its final status is decided, and its hash equals the copy filed in Source Lifecycle; the PPD Release must name the TOM Release it was designed from, and that release must pass the same check. Otherwise nothing of it is used, and a return goes back with the failed condition.
4. **A new release** makes a new pack version. The elements that changed re-open the work that cites them; decided work that cites nothing changed is kept by hash.
5. **Nothing that arrives through a human port is a source.** A run request is admitted only if it carries references. A question from a position is never a source and never changes the design.
6. The pack's ID is `DII-` followed by the SHA-256 of its body.
#### Process (SOP)
Default (receive, identify, normalise, check, deliver), run by the Chief of Staff through the socket's code steps. A refused item comes back with its reason and never enters.
#### Role card
Default; performed by the Chief of Staff (`[ORG]CELL-DCS`) through the socket's code steps.
#### Fixed test
TEST-DI v1, cases 1, 2, 18 to 22 · result `NOT_RUN`

### 4.4 Panel
#### Definition
Default. The Panel also shows, for each run: the run state and its flags with their ages; the mode; the releases or the design in use, and any newer release; every return, with its round, state and age; every needs request; each gate with its result; the gaps by tier and state; each procedure, brief and go-live criterion with its decision state; the questions answered and those answered "I do not know"; per review, its point, verdict and findings. It shows no measure for a single position.
#### Process (SOP)
Default.
#### Role card
Default.
#### Fixed test
Default Panel test · result `NOT_RUN`

---

## 5. Functional capabilities

Five stages (§5.0) are performed by the Input socket (§4.3: S0) and these capabilities: Intake and Design Map (S1); Gap Audit and Health Check (S2); Procedure Writing, Briefs, and Transition and Go-live Criteria (S3); Decision Package and Filing (S4). Needs Requests (§5.2) and Answers (§5.8) are services. Independent Review (§5.9) closes every stage. Each capability is written in the four-part form (Annex A of the template), with one added row, **Done when**. Each step reads: **position**: action → *output* (evidence). Annexes: A (package parts), B (returns), C (run states and gates), D (what this AIOC never does), E (rules carried), F (the gap checks).

**One word per meaning.**
- **Release**: a decided design release this run reads (PPD or TOM). **Outside design**: a design made elsewhere, read as a source (mode B). **Design**: either.
- **Launch package**: this AIOC's output in this version (Annex A).
- **Gap** (`GAP-n`): a check of Annex F that the design fails. **Brief** (`BRF-n`): a draft for counsel or finance. **Criterion** (`GLC-n`): a go-live criterion.
- **Deciding position**: the position that decides a row (§2.1). **Return** (`DIR-n`): this AIOC's notice to the stage that made a release (Annex B).

### 5.0 The stages: input, output, done-test

| ID | Plain name | Run state | Gate | Exact input | Exact output | Done-test | Human decision |
|---|---|---|---|---|---|---|---|
| S0 | **Admit** | `admitting` | T0 | The run Work Item (references only). Mode A: the release notice of `[ORG]AIOC-PPD`. Mode B: the outside design's reference in Source Lifecycle. The connection grants. The engine register. | Input Pack `P0`; the run record, opened. | **T0** (Annex C.2): references only; an enabled mode; the release check (§4.3, part 3) or the source check passes; the connections are signed and in scope; `requesting_authority_cell` and `deciding_positions` are set; RP0 settled. | Requesting Authority: opens the run; names the deciding positions. |
| S1 | **Map** | `mapping` | T1 | P0. | The **design map** (Annex A.1); return drafts (Annex B). | **T1**: mode A: every process, position, unit, decision, control and forum in scope is `used`, `returned` or `out of scope` with a reason; mode B: every element of the outside design is `mapped`, `not mapped` (with the reason) or `out of scope`, and none is rewritten; every return draft passed RP1 and was sent. | Requesting Authority: the scope, if the request did not name it; mode B rows `not mapped`. |
| S2 | **Diagnose** | `diagnosing` | T2 | The design map; P0. | The **gap report** (Annex A.2); the **health check** (Annex A.3). | **T2**: every check of Annex F has a result (`met`, `gap`, `unknown`) with evidence; every gap has its tier, consequence, evidence, proposed fix and route; every item of the health check has a result with evidence; RP2 settled with no unresolved `MATERIAL` finding. | Requesting Authority: the route of each gap (return, decision, or prepare). |
| S3 | **Prepare** | `preparing` | T3 | The design map; the decided gap routes; P0. | The **procedures** (Annex A.4), critical processes first; the **briefs** (Annex A.5); the **transition plan** and the **go-live criteria** (Annex A.6). | **T3**: every procedure step traces to a process step; every brief carries its entity, jurisdiction, draft mark and addressee position; every go-live criterion has its measure, evidence source and a threshold that is a decision row; the go or no-go deciding position is named; every citation passed the Citation Verifier; RP3 settled with no unresolved `MATERIAL` finding. | Requesting Authority: assumptions; contradictions with the design. |
| S4 | **Decide and file** | `deciding`; end states `filed` | T4, then T5 | Every reviewed part of S1 to S3, by hash; the settled review records. | The **Decision Package** (Annex A.8); then the **launch package** manifest and its parts; the filing receipt; the notice to the deciding positions. | **T4**: every element decided (`ACCEPT`, `CORRECT`, `REJECT`) by its deciding position; silence decided nothing. **T5**: the manifest is content-addressed; every element traces to a design element or a source atom; the package lint passes; the package is filed and reads back by hash. | The deciding positions: each element. The Delivery Lead: the attestation. |

**Services and rules used by every stage.**

| Name | What it is | Output | Done-test |
|---|---|---|---|
| **Returns** (§5.1) | A stage that finds a defect in a release drafts a return; the Chief of Staff sends it after review | a return (Annex B) | Annex B, Done when |
| **Asking** (§5.2) | Every stage raises needs candidates; the Chief of Staff asks the Chief of Staff of `[ORG]AIOC-SL` | needs requests; one Missing Report per pass | each request ends answered by reference or with another outcome of the needs-answer contract |
| **Answers** (§5.8) | Any position may ask how the organisation works, at any time | an answer with verified citations, or "I do not know" | §5.8, Done when |
| **Review** (§5.9) | The rule that closes every stage | a review record and a verdict | §5.9, Done when |

**Run states.** `admitting` (S0) → `mapping` (S1) → `diagnosing` (S2) → `preparing` (S3) → `deciding` (S4) → `filed`. Endings, flags and holds: Annex C.1.

**Not in this version (later slices, `PRD-[ORG]AIOC-DI-001` v0.4).** Each comes as a later version of this blueprint, with its own stages, Cells and test cases.
- **Slice 2, Accompany with a thin Operate:** the implementation plan, problem records and the issue queue, learning paths, readiness and rehearsals, the go or no-go package, change impact and adoption, the operating rhythm and its logs, the value register, measures, forum packs, version control, acknowledgement, runnable checklists and quarterly priorities (FR-14, FR-16 to FR-18, FR-20 to FR-22, FR-35 to FR-37, FR-40 to FR-42).
- **Slice 3, Improve:** watching processes through a projection that removes who did the work, conformance, findings, proposals, trials, scheduled reassessment, the quarterly health check and the capability hand-over; ladder level 2 (FR-19, FR-23 to FR-26, FR-38, FR-39, FR-43).
- **Slice 4, Small business:** mode C and self-service setup (FR-04); later still, reference models, the full mentor, the multi-engine council and guidance at the point of work (FR-27 to FR-29, FR-44).

### 5.1 Intake and Design Map

#### Definition
| Field | Content |
|---|---|
| Name | Intake and Design Map |
| Purpose | read a decided design, or map one made elsewhere, so that nothing in it is lost or rewritten, and send every defect of a release back to the stage that made it (FR-01, FR-02, FR-05) |
| Trigger | T0 passed; a new release notice; a defect found at any stage |
| Inputs | the Input Pack |
| Outputs | the design map (Annex A.1); returns (Annex B) |
| Performed by | the Design Mapper (`[ORG]CELL-DDM`) in the Diagnosis Pod (`[ORG]POD-DD`); the Chief of Staff sends |
| Done when | T1 (§5.0); for a return, Annex B, Done when |
| Rules | 1. **Mode A: account for everything.** Every process, position, unit, decision, control and forum of the PPD Release in scope, and every role and hand-off of the TOM Release it names, is recorded `used`, `returned` (with the return) or `out of scope` (with the reason). **New** in v0.1.2: the value case of that TOM Release and the decided priority of each element (TOM blueprint `v0.6.0`, Annex H.6, H.7) are recorded in the design map as they stand, by reference, never changed; a baseline `unknown` or a target `not set` stays so. They are carried for the register of value of slice 2, which starts from them. 2. **Mode B: map, never rewrite.** Each element of the outside design is mapped onto the structure of a PPD release (process, step, decision, position, unit, forum, policy, measure), or marked `not mapped` with the reason. The author's words are kept as cited; the map records how each element was read, never what it should have said. A missing element is a gap (§5.3), never an invention. 3. **Never changed.** A release is read as decided. A defect becomes a return of one kind (Annex B) to the stage that made it: a process, position, unit or control defect to `[ORG]AIOC-PPD`; an operating-model defect to `[ORG]AIOC-TOM`. 4. **The touched elements wait.** Only the elements a return touches are held; the rest of the work goes on. 5. **The loop ends.** A return counts its rounds. Past `return_round_deadline` or `return_rounds_max`, it goes to the Requesting Authority, who answers it, or sets it aside and lets the affected elements go forward on a stated basis, a known defect or a decided assumption (49GAION Standard §3.1, items 4 and 6). 6. **Not a person.** A return names release parts, elements and fact-types, never a person. |

#### Process (SOP)
1. **Design Mapper**: read the release or the outside design, element by element → *design map, draft* (evidence: one row per element).
2. **Design Mapper**: for each defect of a release, draft a return with its kind, elements and evidence → *return draft*.
3. **Chief of Staff**: lock; run RP1 (§5.9) → *settled review*.
4. **Chief of Staff**: send each return and file it into `[ORG]AIOC-SL`; mark the touched elements held; follow each return to its end → *ended return* (evidence: the return's status and its answer or decision reference).

#### Role card
| Field | Content |
|---|---|
| Name | Design Mapper |
| Position and seat | Design Mapper; accountable seat: the DI Delivery Lead |
| Performed by | an agent (`[ORG]CELL-DDM`, full name DI Design Mapper) |
| Purpose | account for every element of the design, and draft every return |
| Authority limits | alone: read, record, map, draft returns; never: change a release, rewrite an outside design, send a return itself, fill a missing element, ask a person |
| Write location | the run record |
| Reports to | Chief of Staff |
| Escalation | to the Chief of Staff, with the elements and evidence |
| Tools and access | the Input Pack only; no tools, no outside access, a fresh context per dispatch |
| Fixed test and score | TEST-DI-DDM v1 (§9) |
| Card version and status | v0.1.0 · draft |

#### Fixed test
TEST-DI-DD v1 and TEST-DI-DDM v1 · result `NOT_RUN`

### 5.2 Needs Requests

#### Definition
As in the TOM blueprint `v0.5.0` §5.2, carried, with these changes. What this AIOC typically asks for: the jurisdictions and entities in scope; existing procedures, forms and templates; the systems in use; known legal obligations; the dates the organisation has in mind for launch. Each request names the gap, procedure, brief or criterion it is for. One decision per row; at most `rows_per_pass` rows per pass. A request never names a person. Done when: each request ends answered by reference, or with another outcome of the needs-answer contract.
#### Process (SOP)
As carried: the Pods raise needs candidates; the Chief of Staff batches, reviews (RPa), sends, waits, and admits each answer through the Input socket as a new pack version.
#### Role card
Performed by the Chief of Staff (§4.2).
#### Fixed test
TEST-DI v1, case 22 · result `NOT_RUN`

### 5.3 Gap Audit

#### Definition
| Field | Content |
|---|---|
| Name | Gap Audit |
| Purpose | find what in the design would stop the organisation from launching, and what is incomplete, each with what it costs and how to fix it (FR-03) |
| Trigger | T1 passed |
| Inputs | the design map; the Input Pack |
| Outputs | the gap report (Annex A.2) |
| Performed by | the Gap Auditor (`[ORG]CELL-DGA`) in the Diagnosis Pod (`[ORG]POD-DD`); the mechanical checks by the Chief of Staff's code steps |
| Done when | T2 (§5.0) |
| Rules | 1. **A fixed list.** The checks are those of Annex F, each with its ID and tier: **blocking** (the organisation cannot launch safely without it) and **completeness**. The list is versioned; a check is never skipped. 2. **Code first.** A check that code can decide on the design map (a step with no position, a decision with two deciders, a unit with no head) is run by code; the Gap Auditor judges only what code cannot. 3. **Every result with evidence.** Each check reads `met`, `gap` or `unknown`, citing design elements or source atoms. In mode B, an element `not mapped` makes the checks that need it `unknown`, never `met`. 4. **Every gap is worked.** Each gap names its consequence, its evidence, a proposed fix and its route: a return to the stage that made the release; a decision row; or work this AIOC prepares in S3. 5. **Bars.** On designs with planted gaps, blocking gaps found and false gaps raised are measured against `gap_bars` (a decision) before first use (NFR-12). 6. **Not a person.** A gap is about the design. It never says who failed. |

#### Process (SOP)
1. **Chief of Staff**: run the code checks of Annex F on the design map → *check record*.
2. **Gap Auditor**: judge the remaining checks; write each gap → *gap report, draft*.
3. **Chief of Staff**: run RP2; send the route rows for decision → *decided routes*.

#### Role card
| Field | Content |
|---|---|
| Name | Gap Auditor |
| Position and seat | Gap Auditor; accountable seat: the DI Delivery Lead |
| Performed by | an agent (`[ORG]CELL-DGA`, full name DI Gap Auditor) |
| Purpose | judge the checks code cannot, and write every gap |
| Authority limits | alone: judge and write; never: skip a check, mark `met` without evidence, fix the design, choose a gap's route, name a person |
| Write location | the run record |
| Reports to | Chief of Staff |
| Escalation | to the Chief of Staff |
| Tools and access | the design map and the Input Pack; a fresh context per dispatch |
| Fixed test and score | TEST-DI-DGA v1 (§9) |
| Card version and status | v0.1.0 · draft |

#### Fixed test
TEST-DI-DGA v1 · result `NOT_RUN`

### 5.4 Health Check

#### Definition
| Field | Content |
|---|---|
| Name | Health Check |
| Purpose | give the organisation a plain picture of where it stands, at entry, across strategy, structure, processes, measures, rhythm and controls (FR-43) |
| Trigger | T1 passed |
| Inputs | the design map; the Input Pack |
| Outputs | the health check (Annex A.3) |
| Performed by | the Health Checker (`[ORG]CELL-DHC`) in the Diagnosis Pod (`[ORG]POD-DD`) |
| Done when | T2 (§5.0) |
| Rules | 1. **A fixed checklist** of items under the six headings, versioned; each item `met`, `not met` or `unknown`, with evidence. 2. **The organisation only.** It scores the organisation, never a position's occupant, and never ranks one part against another. 3. **No outside benchmark** is used as evidence. 4. In this version it runs at entry; the quarterly check comes in slice 3. |

#### Process (SOP)
1. **Health Checker**: answer each item with evidence → *health check, draft*.
2. **Chief of Staff**: run RP2 with the gap report → *settled review*.

#### Role card
| Field | Content |
|---|---|
| Name | Health Checker |
| Position and seat | Health Checker; accountable seat: the DI Delivery Lead |
| Performed by | an agent (`[ORG]CELL-DHC`, full name DI Health Checker) |
| Purpose | the health check at entry |
| Authority limits | alone: answer the checklist; never: score a person, rank parts, use an outside benchmark as evidence |
| Write location | the run record |
| Reports to | Chief of Staff |
| Escalation | to the Chief of Staff |
| Tools and access | the design map and the Input Pack; a fresh context per dispatch |
| Fixed test and score | TEST-DI-DHC v1 (§9) |
| Card version and status | v0.1.0 · draft |

#### Fixed test
TEST-DI-DHC v1 · result `NOT_RUN`

### 5.5 Procedure Writing

#### Definition
| Field | Content |
|---|---|
| Name | Procedure Writing |
| Purpose | write, under each process, the procedure that tells the position at each step exactly what to do, with the forms, templates and records it uses (FR-06, FR-30) |
| Trigger | T2 passed |
| Inputs | per process: its record in the design (mode A: the PPD process record; mode B: the mapped process); the decided gap routes |
| Outputs | the procedures (Annex A.4) |
| Performed by | the Procedure Writer (`[ORG]CELL-DPW`) in the Preparation Pod (`[ORG]POD-DP`) |
| Done when | T3 (§5.0) |
| Rules | 1. **Critical processes first,** in the order the design decided. 2. **Every line traces.** Each procedure step traces to one process step and is done by that step's position; each names its instructions, the form or template it uses, and the record it leaves (from the step's record field). A line that traces to nothing fails. 3. **Never changes the process.** Where the process cannot be followed as written, that is a gap with its route, never an edit of the process. 4. **Done-when kept.** Each procedure step carries its process step's `done_when`, worst error and controls. 5. **Forms and templates are drafts** with position placeholders only. 6. **Every citation is verified** by the Citation Verifier before review (§5.8, rule 3). |

#### Process (SOP)
1. **Procedure Writer**: write each procedure → *procedure drafts*.
2. **Citation Verifier**: check every citation → *verification record*.
3. **Chief of Staff**: run the trace check by code, then RP3 → *settled review*.

#### Role card
| Field | Content |
|---|---|
| Name | Procedure Writer |
| Position and seat | Procedure Writer; accountable seat: the DI Delivery Lead |
| Performed by | an agent (`[ORG]CELL-DPW`, full name DI Procedure Writer) |
| Purpose | the procedures under each process |
| Authority limits | alone: write procedures, forms and templates; never: change a process, add a step, name a person, insert a procedure into a live record |
| Write location | the run record |
| Reports to | Chief of Staff |
| Escalation | to the Chief of Staff; a process that cannot be followed is a gap |
| Tools and access | the design and the Input Pack; a fresh context per dispatch |
| Fixed test and score | TEST-DI-DPW v1 (§9) |
| Card version and status | v0.1.0 · draft |

#### Fixed test
TEST-DI-DPW v1 · result `NOT_RUN`

### 5.6 Briefs

#### Definition
| Field | Content |
|---|---|
| Name | Briefs |
| Purpose | hand counsel and finance what they need to write the texts with legal or money effect: policies, the pay structure, contract and offer templates, authority instruments, the obligations register, the control matrix, and the systems, data and suppliers each process needs (FR-07 to FR-12, as briefs in slice 1) |
| Trigger | T2 passed |
| Inputs | the design (the policy register, the position register with job families and levels, the decision-rights register and authority matrix, the controls catalogue, the units); the decided gap routes; the jurisdictions and entities in scope |
| Outputs | the briefs (Annex A.5) |
| Performed by | the Brief Writer (`[ORG]CELL-DBW`) in the Preparation Pod (`[ORG]POD-DP`) |
| Done when | T3 (§5.0) |
| Rules | 1. **A brief, not the text.** Each brief states what the text must achieve, the design elements it serves, what is known, and the open questions. It is never the final text, and never advice. 2. **Entity and jurisdiction.** Each brief records its legal entity and its jurisdiction; where the jurisdiction is unknown, it writes an outline only. 3. **The mark.** Each brief carries "Draft, not legal advice" and is addressed to the counsel or finance position named in `deciding_positions`. 4. **No amount.** A brief states no pay amount, price or budget figure; it lists the decisions needed. The pay structure brief works from job families and levels and asks for objective, gender-neutral evaluation criteria. 5. **Positions only.** Contract, offer and authority briefs use position placeholders; no brief names a person or prepares a named offer. 6. **Every citation is verified** (§5.8, rule 3). |

#### Process (SOP)
1. **Brief Writer**: write each brief → *brief drafts*.
2. **Citation Verifier**: check every citation → *verification record*.
3. **Chief of Staff**: run the brief lint by code (mark, entity, jurisdiction, addressee, no amount, no name), then RP3 → *settled review*.

#### Role card
| Field | Content |
|---|---|
| Name | Brief Writer |
| Position and seat | Brief Writer; accountable seat: the DI Delivery Lead |
| Performed by | an agent (`[ORG]CELL-DBW`, full name DI Brief Writer) |
| Purpose | the briefs for counsel and finance |
| Authority limits | alone: write briefs; never: write a final legal or policy text, give advice, state an amount, name a person |
| Write location | the run record |
| Reports to | Chief of Staff |
| Escalation | to the Chief of Staff |
| Tools and access | the design and the Input Pack; a fresh context per dispatch |
| Fixed test and score | TEST-DI-DBW v1 (§9) |
| Card version and status | v0.1.0 · draft |

#### Fixed test
TEST-DI-DBW v1 · result `NOT_RUN`

### 5.7 Transition and Go-live Criteria

#### Definition
| Field | Content |
|---|---|
| Name | Transition and Go-live Criteria |
| Purpose | set out how the organisation moves to the decided design, and what must be true before it goes live (FR-13, FR-35 in part) |
| Trigger | T2 passed |
| Inputs | the design (units, positions, processes, the crosswalk from today's organisation); the decided gap routes |
| Outputs | the transition plan and the go-live criteria (Annex A.6) |
| Performed by | the Transition Planner (`[ORG]CELL-DTP`) in the Preparation Pod (`[ORG]POD-DP`) |
| Done when | T3 (§5.0) |
| Rules | 1. **The plan.** Waves; the cut-over runbook by position, each step with its rollback; a parallel run where the organisation decides one; communication by position; the position that chairs the transition review. For a new organisation, the waves are the order in which units and processes start. **New** in v0.1.2: the waves follow the decided priority the releases carry (`must`, then `should`, then `could`), then critical processes first; a wave that departs from that order states why, and the order is decided with the plan. 2. **Consultation first.** Where law requires information or consultation before changes to work organisation, the plan carries a consultation step before any transition notice, and the design stays a proposal until it ends (counsel confirms per jurisdiction). 3. **The criteria.** Each go-live criterion names what must be true, its measure, its evidence source, and a threshold that is a decision row. They include that every blocking gap is closed or decided, and an adoption criterion: each critical process can be completed by its positions unaided, judged at process level. 4. **Who decides.** The go or no-go deciding position is named. This AIOC never decides go or no-go, and never marks a criterion met by its own report. |

#### Process (SOP)
1. **Transition Planner**: draft the plan and the criteria → *drafts*.
2. **Citation Verifier**: check every citation → *verification record*.
3. **Chief of Staff**: run RP3; send the threshold rows for decision → *decided rows*.

#### Role card
| Field | Content |
|---|---|
| Name | Transition Planner |
| Position and seat | Transition Planner; accountable seat: the DI Delivery Lead |
| Performed by | an agent (`[ORG]CELL-DTP`, full name DI Transition Planner) |
| Purpose | the transition plan and the go-live criteria |
| Authority limits | alone: draft; never: set a threshold, decide go or no-go, mark a criterion met, issue a notice to staff, name a person |
| Write location | the run record |
| Reports to | Chief of Staff |
| Escalation | to the Chief of Staff |
| Tools and access | the design and the Input Pack; a fresh context per dispatch |
| Fixed test and score | TEST-DI-DTP v1 (§9) |
| Card version and status | v0.1.0 · draft |

#### Fixed test
TEST-DI-DTP v1 · result `NOT_RUN`

### 5.8 Answers

#### Definition
| Field | Content |
|---|---|
| Name | Answers |
| Purpose | let any position ask how the organisation works, and get an answer grounded in the decided design, or an honest "I do not know" (FR-15, NFR-02) |
| Trigger | a question from a position through the HU input port, at any time once a design is admitted |
| Inputs | the question (never a source); the admitted design and the filed launch package |
| Outputs | an answer record (Annex A.7) to the asking position only |
| Performed by | the Answer Guide (`[ORG]CELL-DAG`) and the Citation Verifier (`[ORG]CELL-DCV`) in the Answers Pod (`[ORG]POD-DA`) |
| Done when | the answer, verified, or "I do not know", has reached the asking position, and the answer record holds its citations |
| Rules | 1. **Only from the design.** An answer cites, for each claim, the design element, its version and a quoted span. A claim with no citation is removed. 2. **"I do not know."** Where the design is silent, the answer says so, and may name the stage or the deciding position that could settle it; it never guesses. 3. **A second engine checks.** The Citation Verifier, on an engine of another family than the writer's, checks that each citation resolves and supports its claim. An answer, a procedure, a brief or a criterion with a citation that fails is not sent. 4. **A question is not a source.** It never changes the design, and it is recorded by ID only. 5. **To the asker only.** The answer goes only to the asking position. 6. **Not about persons.** A question about a person, or about who occupies a position, is answered "outside what DI holds". 7. **Bars.** Grounded answers and "I do not know" on unanswerable questions are measured on a fixed question set against `answer_bars` (a decision) before first use. |

#### Process (SOP)
1. **Answer Guide**: draft the answer with its citations → *answer draft*.
2. **Citation Verifier**: check each citation → *verified answer* or *refused citation*.
3. **Chief of Staff**: send the verified answer, or "I do not know", to the asking position → *answer record* (evidence: the record with its citations and the verifier's result).

#### Role card
| Field | Content |
|---|---|
| Name | Answer Guide; Citation Verifier |
| Position and seat | each its own position; accountable seat: the DI Delivery Lead |
| Performed by | agents (`[ORG]CELL-DAG`, `[ORG]CELL-DCV`), on engines of two families |
| Purpose | the Guide drafts answers from the design; the Verifier checks every citation of every answer and draft |
| Authority limits | Guide: draft only from the design; never: answer from outside the design, guess, change the design, answer about a person. Verifier: check only; never: rewrite an answer, pass a citation it could not resolve |
| Write location | the answer record |
| Reports to | Chief of Staff |
| Escalation | to the Chief of Staff |
| Tools and access | the admitted design and the filed package only; a fresh context per question |
| Fixed test and score | TEST-DI-DAG v1, TEST-DI-DCV v1 (§9) |
| Card version and status | v0.1.0 · draft |

#### Fixed test
TEST-DI-DA v1 and the tests of its Cells · result `NOT_RUN`

### 5.9 Independent Review

#### Definition
The Review Panel rule of the TOM blueprint `v0.5.0` §5.8, carried as `[ORG]AIOC-PPD` carries it (PPD blueprint `v0.3.0` §5.9): several engines from two or more families review each locked output, alone first, then in a short debate held to quotes; code settles; the DI Delivery Lead rules only on what stays contested; the Chief of Staff never rules, dismisses, downgrades or lowers. This AIOC's review points: RP0 (P0), RP1 (design map and return drafts), RP2 (gap report and health check), RP3 (procedures, briefs, plan and criteria), RP4 (the package, before filing), and RPa (each needs pass). Done when: as carried.
#### Process (SOP)
As carried.
#### Role card
Blind Reviewers A to C (`[ORG]CELL-DBRA` to `[ORG]CELL-DBRC`), in the Review Pod (`[ORG]POD-DR`); as carried.
#### Fixed test
TEST-DI-DR v1 and the tests of its Cells · result `NOT_RUN`

### 5.10 Decision Package and Filing

#### Definition
| Field | Content |
|---|---|
| Name | Decision Package and Filing |
| Purpose | put every element to its deciding position, then freeze, file and trace the launch package |
| Trigger | T3 passed |
| Inputs | every reviewed part of S1 to S3, by hash; the settled review records |
| Outputs | the Decision Package (Annex A.8); the launch package manifest and its parts; the filing receipt; the notice to the deciding positions |
| Performed by | the Chief of Staff, by code steps; the DI Delivery Lead attests the method |
| Done when | T4 and T5 (§5.0) |
| Rules | 1. **Every element is decided** by its deciding position: `ACCEPT`, `CORRECT` or `REJECT`. Silence, or approval of a whole package, decides nothing (TOM blueprint `v0.5.0`, `docs/CARRIED-RULES.md` §5, carried). 2. **Inserted by a position.** No draft of this AIOC enters a live record, log or plan of the organisation unless a position inserts it (the ladder, level 1). 3. **Plain words.** The Decision Package states the unknowns, the assumptions, the open returns and the blocking gaps in plain words. 4. **Frozen and content-addressed.** The manifest lists every part by hash, every pack version, the design it was made from (IDs and manifest hashes) and every return. 5. **The package lint.** No person's name; no amount; no final legal text; every brief marked; every citation verified. 6. **Filed.** The package is filed into Source Lifecycle as a source of origin kind `delivery and implementation`, read back by hash, and announced to the deciding positions. 7. **The trace query.** Code resolves any artefact to its design element, its deciding position and its decision, and back (FR-33). |

#### Process (SOP)
1. **Chief of Staff**: generate the Decision Package; obtain the Delivery Lead's attestation of T0 to T3 → *Decision Package*.
2. **Chief of Staff**: run RP4; send each row to its deciding position → *decided rows*.
3. **Chief of Staff**: freeze the manifest, run the lint, file, read back, send the notice → *filed launch package* (evidence: the filing receipt and the read-back hash).

#### Role card
Performed by the Chief of Staff (§4.2); the attestation by the DI Delivery Lead (§13, H-12).

#### Fixed test
TEST-DI-DCS v1 (cases 40, 41) · result `NOT_RUN`

---

## 6. Coordination and routes

- **`[ORG]AIOC-PPD`.** The design source, linked directly.
  - **Routes.** Release notices arrive through the Input socket. Returns leave as Work Items through the output port, each also filed into Source Lifecycle.
  - **The connection.** Signed by the `[ORG]HOAC-ACS` position over `[ORG]AIOC-PPD` as `connect-external-port`, with two scopes: read its decided releases; send returns. A revocation cuts it at the gateway at once and holds the run.
- **`[ORG]AIOC-TOM`.** Its decided release is read by reference from Source Lifecycle. Returns on it leave through a connection signed over `[ORG]AIOC-TOM`, scope: send returns and receive their answers (TOM blueprint `v0.5.0`, §5.10).
- **Loops.** A return is a Work Item to the stage that made the release. That stage answers it on that Work Item: by a new release (announced, for PPD, by a new release notice) or by a decision of the Requesting Authority; it never opens a new item back to this AIOC, so the chain never loops (Protocol §4.6, item 2). Every return ends (Annex B).
- **`[ORG]AIOC-SL`.** The source of record, and the only route to any person in the organisation about the organisation. The connection (Protocol §13, item 5) has three scopes: read; needs requests; write only this AIOC's own packages and design reports (its returns).
- **The organisation's positions.** Questions arrive through the HU input port and answers leave through the HU output port, to the asking position only. Decision Package rows go to the deciding positions the same way.
- **Work Items.**
  - **The run.** One Work Item, opened by the Requesting Authority's Cell through the HU input port. Requested output: a launch package (Annex A). Acceptance test: the Requesting Authority's (T4 decided; the manifest valid; the filed reference reads back). Sources: the mode and the design reference.
- **`[ORG]AIOC-OCO`.** It installs, fixes and upgrades this AIOC through the front door. Every proposal, correction or critique of this AIOC's AIs is a `design-proposal` Work Item to OCO.
- **Routing rows this AIOC contributes.** `return → [ORG]AIOC-PPD or [ORG]AIOC-TOM`; `return filing → [ORG]AIOC-SL`; `needs request → [ORG]AIOC-SL`; `missing report → [ORG]AIOC-SL`; `launch package filing → [ORG]AIOC-SL`; `answer → the asking position`.

## 7. Records and where things live

| Record | Home | Source rule |
|---|---|---|
| This blueprint, its tests, decisions and cards | the writing repository `<org>aioc-di` | one home for each thing |
| The product requirements, the code steps and their tests | the code project `<org>aioc-di` | one home for each thing |
| An organisation's run records: Input Pack versions, drafts, review records, verification records, ruling sheets, answer records | `<org>aioc-di-records`; `-records-restricted` for any run record that touches a Strictly confidential source | append-only; referenced from the package manifest by hash |
| The organisation's sources, the needs answers, the decisions, the filed launch package and the filed returns | `[ORG]AIOC-SL` | Source Lifecycle is the only home of a source |
| The design releases | `[ORG]AIOC-PPD` and `[ORG]AIOC-TOM`, filed in `[ORG]AIOC-SL` | read by reference and hash, never copied |
| The link between positions and whoever occupies them | not here: top management's own mechanism (Standard §1.1, items 9 and 10) | never in this AIOC |
| Work Items | the shared queue | Protocol §2 |

- **References, not copies.** Atom text and release text are held only in the run workspace. Records store IDs and hashes.
- **Questions.** A question is recorded by ID, with the asking position's code and the answer's citations; its text stays in the run workspace.
- **Revocation or reclassification.** On a notice from Source Lifecycle or a design stage, the run is held and its workspace copies are sealed.
- **Engine ceilings.** No atom or release part is sent to an engine whose confidentiality ceiling is below its level (TOM blueprint `v0.5.0` §5.8, rule 17, carried).

## 8. Tools and the shared AI gateway

| Tool | Existing shared tool, or new | If new: asked of the builder as |
|---|---|---|
| The PPD connection (release notice in, returns out, answers in) | made on the PPD side in the PPD blueprint `v0.4.0` (`upstream/PROPOSALS.md`, item 1) | build items in the code project |
| The TOM return connection (returns out, answers in) | made on the TOM side in the TOM blueprint `v0.5.0` (`upstream/PROPOSALS.md`, item 2) | build items in the code project |
| The Source Lifecycle connection | existing in `[ORG]AIOC-SL`; the origin kind `delivery and implementation` is new | a change to `[ORG]AIOC-SL` proposed through OCO (`upstream/PROPOSALS.md`, item 3) |
| The code steps: the socket and the release check; the design-map checks; the code checks of Annex F; the procedure trace check; the brief lint; the citation resolver; the package manifest and lint; the trace query | new in this AIOC's code project, one build item per step, each with its tests | build items in the code project |
| The schemas of Annex A | field lists in Annex A, made into schemas before the first run; returns use the Library contract `library/contracts/design-return.schema.json` of `49GAION-protocol` | build items in the code project |
| Engine calls | through the tool gateway, bound per call from the engine register | — |

- **Metering.** Every engine call goes through the tool gateway of the `[ORG]AION`, metered for this AIOC within `budget_cap` (Standard §4.4, item 11; NFR-11).
- **Null default.** Every AI Cell runs with no tools, no outside access, no memory and a fresh context for each dispatch.
- **Tests stay hidden from the runners.** No Cell under test sees TEST-DI, its fixtures or §9.
- **Standing alone.** Outside an `[ORG]AION`, this AIOC runs behind its own gateway, which fails closed: one negative case for every Human Floor type passes before each release (NFR-09).

| Tool role | Connector | Access managed in | Part card version |
|---|---|---|---|
| design source | `[ORG]AIOC-PPD` release port | Panel; the grant is signed at the tool gateway as `connect-external-port` | 49GAION Process and Position Design, v2 |
| returns to the operating model | `[ORG]AIOC-TOM` return port | Panel; as above | 49GAION Target Operating Model, v1 |
| source of record | `[ORG]AIOC-SL` output socket | Panel; as above | 49GAION Source Lifecycle, v1 |

**Mechanism register.** Read on 15 October 2026. A row is never deleted.

| ID | Mechanism | What it does | Where it lives | Today | Target |
|---|---|---|---|---|---|
| M-01 | Release check | admits only decided releases whose hashes match their filed copies | — | decided, not built | build |
| M-02 | Return path | sends returns, holds touched elements, counts rounds, ends each return | — | decided, not built | build (with the PPD and TOM changes) |
| M-03 | Gap checks | the code checks of Annex F | — | decided, not built | build |
| M-04 | Citation resolver | resolves each citation to an element, its version and a quoted span | — | decided, not built | build |
| M-05 | Package lint | keeps the package to drafts for decision: no names, no amounts, every brief marked | — | decided, not built | build |
| M-06 | Trace query | from any artefact to its design element, deciding position and decision, and back | — | decided, not built | build |
| M-07 | Review rule | as carried from `[ORG]AIOC-TOM` | `[ORG]AIOC-TOM` code project, when built | decided, not built | reuse |

**Reserve.**

| ID | Idea | Why held | Reconsider when |
|---|---|---|---|
| R-01 | Slices 2 to 4 of `PRD-[ORG]AIOC-DI-001` | slice 1 first, by the governing seat's direction | slice 1 is approved and its test has run |
| R-02 | A shared review service for every design stage | one more part to build before the first run | a fourth stage needs the same rule |

## 9. Fixed tests: index, triggers and scores

The cases are written in `tests/TEST-DI.md`. Cases 1 to 17 are the Library's TEST-DELIVERY-AND-IMPLEMENTATION v1, unchanged. Cases 18 to 47 are this AIOC's own. The Delivery Lead's seat test is DDL-1 to DDL-5. The owner of every part's test is the DI Delivery Lead; the owner of the AIOC's whole test, and of the Delivery Lead's own seat test, is the Cell carrying `[ORG]HOAC-TM`. Library cases 9, 11 (level 2), 13 (the projection), 14 and 16 (the full export) test features of later slices; in this version they read `NOT_RUN`, so the whole test cannot pass until those slices are built.

| Part | Test ID and version | Cases of TEST-DI v1 | Evidence level | Last run | Result |
|---|---|---|---|---|---|
| `[ORG]AIOC-DI` (whole) | TEST-DI v1 | all (1–50) | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DDL` DI Delivery Lead | TEST-DI-DDL v1 | DDL-1 to DDL-5 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DCS` Chief of Staff (with Office, Input socket, Needs Requests, Decision Package and Filing) | TEST-DI-DCS v1 | 1, 4, 8, 10–13, 15–22, 25, 40–44, 46, 48 | MEASURED | — | `NOT_RUN` |
| Panel | default Panel test | — | MEASURED | — | `NOT_RUN` |
| `[ORG]POD-DD` Diagnosis | TEST-DI-DD v1 | 2, 3, 5, 23, 24, 26–29, 49 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DDM` Design Mapper | TEST-DI-DDM v1 | 2, 23, 24, 49 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DGA` Gap Auditor | TEST-DI-DGA v1 | 5, 26–28 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DHC` Health Checker | TEST-DI-DHC v1 | 29 | MEASURED | — | `NOT_RUN` |
| `[ORG]POD-DP` Preparation | TEST-DI-DP v1 | 6, 30–35, 50 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DPW` Procedure Writer | TEST-DI-DPW v1 | 6, 30, 31 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DBW` Brief Writer | TEST-DI-DBW v1 | 6, 32 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DTP` Transition Planner | TEST-DI-DTP v1 | 8, 33–35, 50 | MEASURED | — | `NOT_RUN` |
| `[ORG]POD-DA` Answers | TEST-DI-DA v1 | 7, 36–38 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DAG` Answer Guide | TEST-DI-DAG v1 | 7, 36, 37 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DCV` Citation Verifier | TEST-DI-DCV v1 | 36, 38 | MEASURED | — | `NOT_RUN` |
| `[ORG]POD-DR` Review | TEST-DI-DR v1 | 39 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DBRA` to `[ORG]CELL-DBRC` Blind Reviewers | TEST-DI-DBRA v1 to TEST-DI-DBRC v1 | 39 | MEASURED | — | `NOT_RUN` |
| Type (Specialised) | TEST-DI v1, case 47 | 47 | MEASURED | — | `NOT_RUN` |

- **Re-run triggers.** The template defaults, plus any change to the design return contract, to the PPD or TOM release format, to the Source Lifecycle output socket, to the check list of Annex F, or to the package lint.
- **Complete** only when every part's test has a visible result. `NOT_RUN` is never PASS.

**Checks that are not fixed tests.**

| Check | Placement | Budget per item | Degradation order | Blocks only for |
|---|---|---|---|---|
| Outbound name check: no person's name in any return, request, answer or package part | router | each outbound message | none | the message |
| Citation verification | inside the producer's loop, at most 2 fix rounds | each citation | none | the draft or the answer |
| Package lint | as evidence on the verdict record of RP4 | each package | none | the filing |
| Return reconciliation: every return sent has a filed copy with the same hash, and every return has ended or is within its deadline | after completion | daily | none; a failure opens a defect | nothing; it flags |

## 10. Build: what is generated from this file

| Built thing | Generated from | Recorded where |
|---|---|---|
| Panel profile | §0, §1, §3, §4.4, §5 role cards | the panel profile names this file's commit |
| Back office | §4.2 role card and SOP (instruction); §4 to §5 (knowledge) | the back office records the commit it was built from |
| Card in the protocol AIOC's map | §1 | the register links this file |
| Cards of the Pods and Cells, and the bot identity cards | §17 | `cards/`, by `tools/make_cards.py` |

**Delivery path:** definition change → tests → Panel and Back office update → one-click rollback to the previous commit.

## 11. Exceptions

1. **The Back office converses with humans** (`converses_with_humans: true`). Reason: answering positions' questions is part of this AIOC's purpose (FR-15). Bounds: it answers only from the decided design, to the asking position only; a question is never a source (§5.8).
2. **The Chief of Staff never asks the organisation's people anything about the organisation.** It reaches the organisation for facts only through the Chief of Staff of `[ORG]AIOC-SL`. Reason: as for `[ORG]AIOC-TOM` (its §11, item 1).
3. **Two design sources.** The template's Input socket takes sources. This one also takes a design release directly from `[ORG]AIOC-PPD`, by reference and hash, and returns defects to it and to `[ORG]AIOC-TOM`. Reason: the chain of design stages (49GAION Standard §3.1, items 3 to 6).
4. **Rules carried by reference.** The review rule, labels and decision rules are carried from the TOM blueprint `v0.5.0` by section (Annex E).

## 12. Lessons and proposals to the mother

One dated line per lesson, each written without any organisation's details. Nothing is proposed upstream without the governing seat's word; the drafts are in `upstream/PROPOSALS.md`.

1. 2026-10-15 · A decided design is not yet a working organisation: procedures, briefs for counsel and finance, the transition plan and the go-live criteria are still needed, and the organisation needs a stage beside it through launch and after. Test questions added: cases 30 to 35. This text is the mother.
2. 2026-10-15 · An assistant that answers questions about how an organisation works must answer only from the decided design, with a second engine checking each citation, and say "I do not know" otherwise. Test questions added: cases 36 to 38.
3. 2026-10-16 · The value an organisation expects from its new design, and the order in which its parts matter, are decided before this stage; this stage carries them unchanged and starts its rollout and its register of value from them. Test questions added: cases 49 and 50 (`decisions/DR-0003`).

## 13. For the `[ORG]HOAC-ACS` seat, and every decision only a human seat can take

Every decision that only a human seat can take is listed here once. Silence decides nothing; a general approval decides no row.

| ID | Decision | Seat | Default |
|---|---|---|---|
| H-01 | Name the Requesting Authority's Cell: the GOV Cell itself, or a human Cell to which it delegates these decisions (`delegate-authority`) | GOV | none: T0 fails |
| H-02 | **Top management's own mechanism.** Arrange the DI Delivery Lead position and any HOAC position added to this AIOC. Nothing of who occupies them enters this blueprint | the Cell carrying `[ORG]HOAC-TM` | the position is vacant: the AIOC does not join |
| H-03 | Install `[ORG]AIOC-DI` (`create-or-install-unit`); its `change-parent`; its `restart-stopped-unit` | the Cell carrying `[ORG]HOAC-TM` | none |
| H-04 | Accept the PPD, TOM and Source Lifecycle changes this AIOC needs (`upstream/PROPOSALS.md`, items 1 to 3; items 1 and 2 are made in the PPD blueprint `v0.4.0` and the TOM blueprint `v0.5.0`) | the Cell carrying `[ORG]HOAC-TM`, made through OCO | required before joining |
| H-05 | The connection grants to PPD, TOM and Source Lifecycle (`connect-external-port`), their widening and revocation | the `[ORG]HOAC-ACS` positions over those AIOCs | none: T0 fails |
| H-06 | `modes_enabled`, `gap_bars`, `answer_bars`, `return_round_deadline`, `return_rounds_max`, `review_budget_per_run`, `reduced_review_permitted` and the AIOC's `budget_cap` | the Cell carrying `[ORG]HOAC-TM` | none: must be set; reduced review `no` |
| H-07 | The permission ladder: each class of action and its level, at most level 1 in this version | the owner position | every class at level 1 |
| H-08 | `deciding_positions`: the go or no-go position; the counsel position for each jurisdiction; the finance position | Requesting Authority | none: T0 fails |
| H-09 | Open the run; name the mode and the scope | Requesting Authority | none: no run |
| H-10 | The rows of S1 to S4: mode B rows `not mapped`; the route of each gap; assumptions; contradictions; each procedure, brief, plan element and go-live criterion with its threshold; each element of the package | Requesting Authority, or the deciding position the row names | undecided |
| H-11 | The go or no-go itself, at go-live | the go or no-go deciding position | never this AIOC |
| H-12 | Inside a run: rule on contested `MATERIAL` findings; accept a reduced level within H-06; approve a second run; attest T0 to T3 | the DI Delivery Lead | none taken; the step waits |
| H-13 | Create `<org>aioc-di-records` and `-records-restricted`, recorded first (Naming Standard R9) | the Cell carrying `[ORG]HOAC-TM` | before the first run |
| H-14 | Send the drafts of `upstream/` to the parts they concern | GOV | after this blueprint is approved |
| H-15 | Approve this blueprint `v0.1.2` as the design of `[ORG]AIOC-DI`, slice 1 | the human hub | it stays a draft; nothing is installed |

**Money:** the budget cap and the review budget (H-06); every amount in a brief is a decision of the organisation, never this AIOC's. **People:** this AIOC prepares for positions, never for who fills them; the go or no-go is the deciding position's (H-11). **Legal:** every brief goes to the counsel position of its jurisdiction before any decision.

## 14. Change log

| Blueprint version | Date | Change | Template version | Commit |
|---|---|---|---|---|
| v0.1.0 | 2026-10-15 | First blueprint of `[ORG]AIOC-DI`, the mother text of the Library part 49GAION Delivery and Implementation (proposed): slice 1, the gap audit and the launch essentials; modes A and B; five stages; answers with verified citations; returns under the Library contract; TEST-DI v1 | v1.5.0 at `e89ed1d` | this commit |
| v0.1.1 | 2026-10-16 | Receives the answers to its returns, from `[ORG]AIOC-PPD` and `[ORG]AIOC-TOM` (a `tom-in` port and Annex B, rule 5), and the release notice of `[ORG]AIOC-PPD` under its contract (`decisions/DR-0002`); a return set aside carries its elements forward on the stated basis; the Library texts are merged, no longer proposed; the TOM rules are carried from the TOM blueprint `v0.5.0`. TEST-DI v1, case 48 | v1.5.0 at `e89ed1d` | this pull request |
| v0.1.2 | 2026-10-16 | Carries the value case of the TOM Release and each element's decided priority in the design map, unchanged (§5.1 rule 1; A.1), for the register of value of slice 2; the transition waves follow the decided priority (A.6); Annex D item 13; Annex E pins TOM `v0.6.0` (`decisions/DR-0003`). TEST-DI v1, cases 49 and 50, added before any use | v1.5.0 | this pull request |

---

## 15. Configuration

The template's slots, all `none: must be set` until the organisation sets them (Protocol §11), plus these slots of this AIOC:

| Slot | Card key | Default offered | Allowed values | Set by |
|---|---|---|---|---|
| Requesting Authority Cell | `requesting_authority_cell` | none: must be set | the Cell carrying `[ORG]HOAC-GOV`, or a human Cell it delegated these decisions to | the Cell carrying `[ORG]HOAC-GOV` |
| Modes enabled | `modes_enabled` | A, B | A, B (C in slice 4) | the Cell carrying `[ORG]HOAC-TM` |
| Deciding positions | `deciding_positions` | none: must be set | position codes of the organisation's decided design | Requesting Authority |
| Rows per needs pass | `rows_per_pass` | 12 | 1–12 | DI Delivery Lead |
| Passes past their deadline before a non-response stop | `non_response_passes` | none: must be set | ≥ 1 | the Cell carrying `[ORG]HOAC-TM` |
| Return round deadline; most rounds | `return_round_deadline`; `return_rounds_max` | none: must be set | a period; ≥ 1 | the Cell carrying `[ORG]HOAC-TM` |
| Engines per review point | `review_engines` | 3 | 3–5 | DI Delivery Lead, within the review budget |
| Families per review | `review_families_min` | 2 | 2–3 | DI Delivery Lead |
| Reduced review permitted | `reduced_review_permitted` | `no` | `yes`, `no` | the Cell carrying `[ORG]HOAC-TM` (never this AIOC's own `[ORG]HOAC-ACS` position) |
| Review budget per run | `review_budget_per_run` | none: must be set | within `budget_cap` | the Cell carrying `[ORG]HOAC-TM` |
| Gap bars | `gap_bars` | none: must be set | two shares: blocking gaps found, at or above; false gaps, at or below | the Cell carrying `[ORG]HOAC-TM` |
| Answer bars | `answer_bars` | none: must be set | two shares: grounded answers; "I do not know" on unanswerable questions | the Cell carrying `[ORG]HOAC-TM` |
| Permission ladder | `ladder` | every class at level 1 | level 0 or 1 per class in this version | the owner position |
| Template slots | `office_accountable_human`, `central_head`, `discussion_limits`, `waiting_deadlines`, `bounce_limit`, `chain_depth` (at least 1), `halt_request_priority` (immediate), `budget_cap`, `unattended_action` (`read-record-triage`), and the `v1.6.0` rows | as the template | — | as the template |

---

## 16. Type

- **Type:** Specialised.
- **Why this AIOC exists:** an organisation needs its decided design taken into a running organisation, with someone beside it through launch and after, who decides nothing for it.
- **Type-specific test:** TEST-DI v1, case 47 · result `NOT_RUN`.

---

## 17. Cells and Pods

The parts inside this AIOC (`docs/CELLS-AND-PODS.md` of `49GAION-aioc`). The role and nature of this AIOC are read from the type of its top Cell, the DI Delivery Lead. Every field that points to a human takes a position code only.

| Code | Kind | Type | Filler kind | HOAC label | Parent | Fixed test (owner) | External ports |
|---|---|---|---|---|---|---|---|
| `[ORG]CELL-DDL` | CELL | Human Seat | human | `[ORG]HOAC-ACS` | `[ORG]AIOC-DI` | TEST-DI-DDL v1 (the Cell carrying `[ORG]HOAC-TM`) | none |
| `[ORG]CELL-DCS` | CELL | AI Chief of Staff | ai | none | `[ORG]AIOC-DI` | TEST-DI-DCS v1 (`[ORG]CELL-DDL`) | `ppd-in`, `ppd-out`, `tom-out`, `tom-in`, `sl-in`, `sl-out` |
| `[ORG]POD-DD` | POD | AI Pod | — | none | `[ORG]AIOC-DI` | TEST-DI-DD v1 (`[ORG]CELL-DDL`) | — |
| `[ORG]CELL-DDM` | CELL | AI Agent | ai | none | `[ORG]POD-DD` | TEST-DI-DDM v1 (`[ORG]CELL-DDL`) | none |
| `[ORG]CELL-DGA` | CELL | AI Agent | ai | none | `[ORG]POD-DD` | TEST-DI-DGA v1 (`[ORG]CELL-DDL`) | none |
| `[ORG]CELL-DHC` | CELL | AI Agent | ai | none | `[ORG]POD-DD` | TEST-DI-DHC v1 (`[ORG]CELL-DDL`) | none |
| `[ORG]POD-DP` | POD | AI Pod | — | none | `[ORG]AIOC-DI` | TEST-DI-DP v1 (`[ORG]CELL-DDL`) | — |
| `[ORG]CELL-DPW` | CELL | AI Agent | ai | none | `[ORG]POD-DP` | TEST-DI-DPW v1 (`[ORG]CELL-DDL`) | none |
| `[ORG]CELL-DBW` | CELL | AI Agent | ai | none | `[ORG]POD-DP` | TEST-DI-DBW v1 (`[ORG]CELL-DDL`) | none |
| `[ORG]CELL-DTP` | CELL | AI Agent | ai | none | `[ORG]POD-DP` | TEST-DI-DTP v1 (`[ORG]CELL-DDL`) | none |
| `[ORG]POD-DA` | POD | AI Pod | — | none | `[ORG]AIOC-DI` | TEST-DI-DA v1 (`[ORG]CELL-DDL`) | — |
| `[ORG]CELL-DAG` | CELL | AI Agent | ai | none | `[ORG]POD-DA` | TEST-DI-DAG v1 (`[ORG]CELL-DDL`) | none |
| `[ORG]CELL-DCV` | CELL | AI Agent | ai | none | `[ORG]POD-DA` | TEST-DI-DCV v1 (`[ORG]CELL-DDL`) | none |
| `[ORG]POD-DR` | POD | AI Pod | — | none | `[ORG]AIOC-DI` | TEST-DI-DR v1 (`[ORG]CELL-DDL`) | — |
| `[ORG]CELL-DBRA` … `[ORG]CELL-DBRC` | CELL | AI Agent | ai | none | `[ORG]POD-DR` | TEST-DI-DBRA v1 … TEST-DI-DBRC v1 (`[ORG]CELL-DDL`) | none |

**The card data (the blueprint governs).** `tools/make_cards.py` expands the block below into the complete unit cards and bot identity cards, writes them into `cards/`, and checks them against the schemas of `49GAION-protocol`, Naming Standard R15, and this blueprint.

```yaml
parts:
  defaults:
    accountable_to: "[ORG]CELL-DDL"
    card_version: "v0.1.2"
    version: "0.1.2"
    lifecycle_state: "designed"
    test_version: "v1"
    test_owner: "[ORG]CELL-DDL"
    audit_trail: "the run record of [ORG]AIOC-DI"
    hu_in: ["run control and configuration from the DI Delivery Lead (never a source)"]
    hu_out: ["run report to the DI Delivery Lead"]
  cells:
    - code: "[ORG]CELL-DDL"
      full_name: "DI Delivery Lead"
      parent: "[ORG]AIOC-DI"
      type: "Human Seat"
      filler_kind: "human"
      hoac: "[ORG]HOAC-ACS"
      accountable_to: "[ORG]CELL-TMS"       # example code of the Cell carrying [ORG]HOAC-TM
      entity: "<entity>"
      authority_scope:
        decision_types: ["change-fixed-test-or-threshold", "create-or-install-unit", "change-filler", "retire-unit", "restart-stopped-unit", "appoint-acting-filler"]
        entity: "<entity>"
        expires: "2027-10-15"                # placeholder; each organisation sets it
        authority: "delegated"
      test: { id: "TEST-DI-DDL", cases: "DDL-1 to DDL-5", owner: "[ORG]CELL-TMS" }
      ai_in: ["run brief", "ruling sheets for contested MATERIAL findings", "release notice"]
      ai_out: ["run control and configuration"]
      hu_in: ["direction from the Cell carrying [ORG]HOAC-TM"]
      hu_out: ["rulings, attestations and reduced-level acceptances, under live sign-in", "report to the Cell carrying [ORG]HOAC-TM"]
    - code: "[ORG]CELL-DCS"
      full_name: "DI Chief of Staff"
      role: "Chief of Staff"
      parent: "[ORG]AIOC-DI"
      type: "AI Chief of Staff"
      filler_kind: "ai"
      cell_kind: "chief-of-staff-cell"
      test: { id: "TEST-DI-DCS", cases: "1, 4, 8, 10-13, 15-22, 25, 40-44, 46, 48" }
      ai_in: ["release notice", "return answer", "source reference", "needs answer", "needs status", "needs candidate", "return draft", "locked outputs of the Pods", "settled review records", "verified answer"]
      ai_out: ["Input Pack version", "dispatch to a Pod", "review packet", "return", "needs request", "missing report", "Decision Package", "launch package filing"]
      hu_in: ["run request from the Requesting Authority's Cell (references only)", "a question from a position (never a source)", "a decision of a deciding position", "run control from the DI Delivery Lead"]
      hu_out: ["answer to the asking position", "Decision Package rows to the deciding positions", "run brief and ruling sheets to the DI Delivery Lead", "filing notice to the Requesting Authority's Cell"]
      external_ports:
        - { port: "ppd-in", direction: "input", accepted_content: ["release notice", "return answer"], authority_limit: "the read scope signed under connect-external-port over [ORG]AIOC-PPD", audit_trail: "unit register; serve log of [ORG]AIOC-PPD" }
        - { port: "ppd-out", direction: "output", accepted_content: ["return"], authority_limit: "returns only, under the scope signed over [ORG]AIOC-PPD", audit_trail: "unit register; the Work Item record" }
        - { port: "tom-out", direction: "output", accepted_content: ["return"], authority_limit: "returns only, under the scope signed over [ORG]AIOC-TOM", audit_trail: "unit register; the Work Item record" }
        - { port: "tom-in", direction: "input", accepted_content: ["return answer"], authority_limit: "answers to this AIOC's returns only, under the scope signed over [ORG]AIOC-TOM", audit_trail: "unit register; the Work Item record" }
        - { port: "sl-in", direction: "input", accepted_content: ["source reference", "needs answer", "needs status"], authority_limit: "the read scope signed under connect-external-port over [ORG]AIOC-SL", audit_trail: "unit register; serve log of [ORG]AIOC-SL" }
        - { port: "sl-out", direction: "output", accepted_content: ["needs request", "missing report", "return filing", "launch package filing"], authority_limit: "the request and write scope signed over [ORG]AIOC-SL: this AIOC's own packages and design reports only", audit_trail: "unit register; serve log of [ORG]AIOC-SL" }
      bot:
        allowed_actions: ["dispatch Cells of this AIOC", "build Input Pack versions through the code steps", "lock outputs and run code steps", "draw review engines and run the review code steps", "write the run record", "send reviewed returns and file them in [ORG]AIOC-SL", "send needs requests and Missing Reports to [ORG]AIOC-SL", "send verified answers to the asking position", "send Decision Package rows to the deciding positions", "file a package whose elements are decided"]
        ask_first_actions: ["a second run in parallel", "a budget above the cap", "a reduced review level", "any change to configuration", "anything outside its role card"]
    - { code: "[ORG]CELL-DDM", full_name: "DI Design Mapper", role: "Design Mapper", parent: "[ORG]POD-DD", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DDM", cases: "2, 23, 24, 49" }, ai_in: ["Input Pack version"], ai_out: ["design map", "return draft", "needs candidate"], bot: { allowed_actions: ["read a release or map an outside design, element by element", "draft returns with their evidence"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DGA", full_name: "DI Gap Auditor", role: "Gap Auditor", parent: "[ORG]POD-DD", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DGA", cases: "5, 26-28" }, ai_in: ["design map", "check record", "Input Pack version"], ai_out: ["gap report draft", "needs candidate"], bot: { allowed_actions: ["judge the checks code cannot decide", "write each gap with its consequence, evidence, fix and route"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DHC", full_name: "DI Health Checker", role: "Health Checker", parent: "[ORG]POD-DD", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DHC", cases: "29" }, ai_in: ["design map", "Input Pack version"], ai_out: ["health check draft"], bot: { allowed_actions: ["answer the health checklist with evidence"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DPW", full_name: "DI Procedure Writer", role: "Procedure Writer", parent: "[ORG]POD-DP", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DPW", cases: "6, 30, 31" }, ai_in: ["process records of the design", "decided gap routes"], ai_out: ["procedure drafts", "gap candidate"], bot: { allowed_actions: ["write procedures, forms and templates under each process"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DBW", full_name: "DI Brief Writer", role: "Brief Writer", parent: "[ORG]POD-DP", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DBW", cases: "6, 32" }, ai_in: ["design registers", "decided gap routes", "jurisdictions and entities in scope"], ai_out: ["brief drafts", "needs candidate"], bot: { allowed_actions: ["write briefs for counsel and finance"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DTP", full_name: "DI Transition Planner", role: "Transition Planner", parent: "[ORG]POD-DP", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DTP", cases: "8, 33-35, 50" }, ai_in: ["units, positions, processes and the crosswalk of the design", "decided gap routes"], ai_out: ["transition plan draft", "go-live criteria draft"], bot: { allowed_actions: ["draft the transition plan and the go-live criteria"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DAG", full_name: "DI Answer Guide", role: "Answer Guide", parent: "[ORG]POD-DA", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DAG", cases: "7, 36, 37" }, ai_in: ["question by ID", "the admitted design and the filed package"], ai_out: ["answer draft with citations"], bot: { allowed_actions: ["draft answers only from the decided design, with citations"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DCV", full_name: "DI Citation Verifier", role: "Citation Verifier", parent: "[ORG]POD-DA", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DCV", cases: "36, 38" }, ai_in: ["draft with citations", "the cited elements and spans"], ai_out: ["verification record"], bot: { allowed_actions: ["check that each citation resolves and supports its claim"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DBRA", full_name: "DI Blind Reviewer A", role: "Blind Reviewer A", parent: "[ORG]POD-DR", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DBRA", cases: "39" }, ai_in: ["review packet", "collated findings of its review"], ai_out: ["review card", "positions on findings"], bot: { allowed_actions: ["write its own review card", "state its own positions on the findings of its review"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DBRB", full_name: "DI Blind Reviewer B", role: "Blind Reviewer B", parent: "[ORG]POD-DR", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DBRB", cases: "39" }, ai_in: ["review packet", "collated findings of its review"], ai_out: ["review card", "positions on findings"], bot: { allowed_actions: ["write its own review card", "state its own positions on the findings of its review"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DBRC", full_name: "DI Blind Reviewer C", role: "Blind Reviewer C", parent: "[ORG]POD-DR", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DBRC", cases: "39" }, ai_in: ["review packet", "collated findings of its review"], ai_out: ["review card", "positions on findings"], bot: { allowed_actions: ["write its own review card", "state its own positions on the findings of its review"], ask_first_actions: ["anything outside its role card"] } }
  pods:
    - { code: "[ORG]POD-DD", full_name: "DI Diagnosis", type: "AI Pod", inner_units: ["[ORG]CELL-DDM", "[ORG]CELL-DGA", "[ORG]CELL-DHC"], top_cell: "[ORG]CELL-DGA", test: { id: "TEST-DI-DD", cases: "2, 3, 5, 23, 24, 26-29, 49" }, ai_in: ["Input Pack version"], ai_out: ["design map", "gap report", "health check", "return draft"] }
    - { code: "[ORG]POD-DP", full_name: "DI Preparation", type: "AI Pod", inner_units: ["[ORG]CELL-DPW", "[ORG]CELL-DBW", "[ORG]CELL-DTP"], top_cell: "[ORG]CELL-DPW", test: { id: "TEST-DI-DP", cases: "6, 30-35, 50" }, ai_in: ["design map", "decided gap routes"], ai_out: ["procedures", "briefs", "transition plan", "go-live criteria"] }
    - { code: "[ORG]POD-DA", full_name: "DI Answers", type: "AI Pod", inner_units: ["[ORG]CELL-DAG", "[ORG]CELL-DCV"], top_cell: "[ORG]CELL-DAG", test: { id: "TEST-DI-DA", cases: "7, 36-38" }, ai_in: ["question by ID", "drafts with citations"], ai_out: ["verified answer", "verification record"] }
    - { code: "[ORG]POD-DR", full_name: "DI Review", type: "AI Pod", inner_units: ["[ORG]CELL-DBRA", "[ORG]CELL-DBRB", "[ORG]CELL-DBRC"], top_cell: "[ORG]CELL-DBRA", test: { id: "TEST-DI-DR", cases: "39" }, ai_in: ["review packet"], ai_out: ["review cards and positions"] }
```

- **Accountability.** Every Pod and Cell of this AIOC is `accountable_to` `[ORG]CELL-DDL`. The AIOC itself and the Delivery Lead are `accountable_to` the Cell carrying `[ORG]HOAC-TM`.
- **Bots.** Each AI Cell's bot (twelve) has its own identity card, its own credential, `never_signs: true`, and its memory sealed on a change of filler (Protocol §10, item 3). The credential IDs in `cards/bots/` are placeholders.
- The Requesting Authority, the deciding positions, the Chief of Staff of `[ORG]AIOC-SL` and the Cells of `[ORG]AIOC-PPD` and `[ORG]AIOC-TOM` are not Cells of this AIOC.

**Code checks** (Naming Standard R15 and §5), recorded on 15 October 2026. Each organisation repeats the check of §5.2 against its own register before first use.

| Code | Initials of the full name (R15) | §5.1 | §5.2: no match among this blueprint's codes, nor with `[ORG]AIOC-DI` | §5.3 |
|---|---|---|---|---|
| `[ORG]CELL-DDL` | **D**I **D**elivery **L**ead | pass | pass | pass |
| `[ORG]CELL-DCS` | **D**I **C**hief of **S**taff ("of" skipped) | pass | pass (distinct from `[ORG]CELL-PCS`, `[ORG]CELL-TCS` and `[ORG]CELL-SLCS` of other AIOCs) | pass |
| `[ORG]POD-DD` / `[ORG]CELL-DDM`, `-DGA`, `-DHC` | DI Diagnosis / Design Mapper, Gap Auditor, Health Checker | pass | pass | pass |
| `[ORG]POD-DP` / `[ORG]CELL-DPW`, `-DBW`, `-DTP` | DI Preparation / Procedure Writer, Brief Writer, Transition Planner | pass | pass | pass |
| `[ORG]POD-DA` / `[ORG]CELL-DAG`, `-DCV` | DI Answers / Answer Guide, Citation Verifier | pass | pass | pass |
| `[ORG]POD-DR` / `[ORG]CELL-DBRA` to `-DBRC` | DI Review / Blind Reviewer A to C | pass | pass | pass |

No code of this blueprint uses the suffix `DI` alone, so no part can be read as the AIOC itself.

---
## Annex A. The launch package: its parts and their field lists

Every part is a versioned, content-addressed object. Every element carries an ID, its provenance (`stated`, `inferred`, `unresolved` or `assumed`, as in TOM Annex B, carried), its basis (design element IDs and source atom IDs, at least one) and, after T4, its decision reference. JSON Schemas are made from these lists before the first run and may add nothing.

**A.1 Design map** (run record, summarised in the package). Mode A: one row per element in scope: `element_id`, `part`, `state` (`used`, `returned`, `out of scope`), `return_id`, `reason`, `priority` (as the release decided it, or none). The value case carried (**New** in v0.1.2): per entry of the TOM Release's value case, `entry_id` (`VC-n`), `outcome_ref`, `measures` (each with its baseline and target references, or `unknown` and `not set`, as the release states them) and `elements`, by reference, unchanged. Mode B: one row per element of the outside design: `source_atom`, `read_as` (process, step, decision, position, unit, forum, policy, measure), `maps_to` (an ID in this map's own structure), `state` (`mapped`, `not mapped`, `out of scope`), `reason`.

**A.2 Gap report** (package part). Per check: `check_id` (Annex F), `tier`, `result` (`met`, `gap`, `unknown`), `evidence`. Per gap: `gap_id` (`GAP-n`), `check_id`, `tier` (`blocking`, `completeness`), `elements`, `consequence`, `evidence`, `proposed_fix`, `route` (`return` with its ID; `decision` with its row; `prepare` with the S3 output that answers it), `state`.

**A.3 Health check** (package part). Per item: `item_id`, `heading` (strategy, structure, processes, measures, rhythm, controls), `question`, `result` (`met`, `not met`, `unknown`), `evidence`. A summary per heading, counts only. Never a person.

**A.4 Procedures** (package part; one per process). `procedure_id`; `process_id`; `version`; `owner_position`; `steps[]`: {`step_id` (the process step it traces to), `position`, `instructions`, `form_or_template` (IDs), `record_left`, `done_when`, `worst_error`, `controls`}; `forms_and_templates[]`: {`id`, `name`, `fields` (position placeholders only)}; `citations`.

**A.5 Briefs** (package part). Per brief: `brief_id` (`BRF-n`); `kind` (`policy`, `pay structure`, `contract and offer templates`, `authority instruments`, `obligations register`, `control matrix`, `systems, data and suppliers`); `entity`; `jurisdiction` (or `unknown`, then `outline only`); `serves` (design element IDs); `what_it_must_achieve`; `known`; `open_questions`; `decisions_needed` (never an amount); `addressed_to` (a position code from `deciding_positions`); `mark` ("Draft, not legal advice"); `citations`.

**A.6 Transition plan and go-live criteria** (package part). Plan: `waves[]` {units, processes, order, `priority` (the highest decided priority of what the wave starts), `departs_because` (when it departs from the order of priority)}; `cut_over[]` {step, position, rollback}; `parallel_run` (decided or none); `communication[]` {to position, what, when}; `consultation` {required by (per counsel), before which notice}; `review_chair` (position). Criteria: per criterion: `criterion_id` (`GLC-n`), `what_must_be_true`, `measure`, `evidence_source`, `threshold` (decision reference), `kind` (`blocking gaps closed`, `adoption`, `readiness`, other); `go_no_go_position`.

**A.7 Answer record** (run record). `question_id`; `asking_position`; `answer` or `I do not know`; `citations[]` {`element_id`, `version`, `span_sha256`}; `verifier` {engine family, result}; `sent_at`.

**A.8 Decision Package** (package part). A plain summary; the elements for decision, each with its deciding position and row; the blocking gaps and their routes; the unknowns, the assumptions and the open returns, in plain words; the review findings and their choices.

**The manifest.** `package_id` (`DIP-` + SHA-256 of the manifest body); `run_id`; `mode`; `design` {PPD and TOM release IDs and manifest hashes, or the outside design's source reference}; `parts[]` {name, sha256}; `input_packs[]`; `returns[]` (return IDs with their end states); `decided_at`; `final_status`.

## Annex B. Returns

Returns follow the Library's design return contract, `library/contracts/design-return.schema.json` of `49GAION-protocol` (49GAION Standard §3.1, item 6), with the prefix `DIR`. This AIOC keeps no copy of the contract.

**Rules.**
1. A return goes to the stage that made the release, directly through the gateway, and its copy is filed into Source Lifecycle with the same hash.
2. A return never changes the release.
3. It is answered by a new decided release, or by a decision of the Requesting Authority; each answer that does not end it opens the next round. Past `return_round_deadline` or `return_rounds_max`, it goes to the Requesting Authority, who answers it or sets it aside on a stated basis (`known defect` or `decided assumption`).
4. In mode B there is no release to return to: a defect of the outside design is a gap (§5.3).
5. **Answers.** A return answer arrives on the connection of the stage that made the release and is recorded on the return. An answer by release makes a new pack version through the release check and re-opens only the work that cites a changed element. A return set aside by decision lets its touched elements go forward on the stated basis, each marked `known defect` or `decided assumption` with the decision reference, and listed in the Decision Package in plain words. *(v0.1.1.)*

**Done when.** The return validates; it is sent and filed with one hash; its touched elements show `held: return open`; it ends in a status other than `open`.

## Annex C. Run states and gates

**C.1 Run states.** As §5.0. Endings other than a filed package: `closed: not admitted` (T0 failed, each failed condition named); `closed: non-response`; `closed: rejected`; `closed: withdrawn by the Requesting Authority`. Flags on any state, each with its age: `waiting`; `waiting: ruling`; `held: return open` (on the touched elements only); `held: material finding`; `held: connection revoked`; `held: no reviewers`; `held: review budget`; `stopped`. No flag releases the run slot; every ending releases it.

**C.2 The gates.** T0 to T5 as in §5.0. A gate passes only on its settled review (§5.9) and its done-test. T0 has these conditions: (a) the run request carries references only; (b) its mode is in `modes_enabled`; (c) mode A: the release check passes for the PPD Release and the TOM Release it names; mode B: the outside design is a source held in Source Lifecycle; (d) the connections are signed and in scope; (e) the engine register holds eligible engines for the highest confidentiality level in scope, of two families; (f) `requesting_authority_cell` and `deciding_positions` are set; (g) RP0 is settled.

## Annex D. What this AIOC never does

1. Change, merge, split or drop an element of a design release, or rewrite an outside design.
2. Decide anything for the organisation, the go or no-go included, or take silence as a decision.
3. Give legal, tax, employment or pay advice, write a final legal text, or state an amount.
4. Ask any person anything about the organisation, or send a request that names a person.
5. Name a person, read who occupies a position, or prepare a named offer.
6. Rank, score or watch the occupant of a position, infer emotion, or show a measure for a single position.
7. Read records of the organisation's work (slice 3, through the projection only).
8. Insert a draft into a live record, log or plan; apply any change (ladder level 2 is not in this version).
9. Answer a question from outside the decided design, or send an answer or draft whose citation failed verification.
10. Mark a go-live criterion met on its own report.
11. Grade its own work: no Cell reviews its own output, and the Chief of Staff rules on nothing.
12. Act on a type of the Human Floor signature list, at any level.
13. Change a value case, or set a baseline, a target or a priority of its own (TOM blueprint `v0.6.0`, Annex H.6, H.7).

## Annex E. What is carried from the Target Operating Model blueprint

This AIOC carries these rules from the blueprint of `[ORG]AIOC-TOM` `v0.6.0` (its writing repository, `<org>aioc-tom`), by section, not by copy, as `[ORG]AIOC-PPD` `v0.3.0` carries them (its Annex E). A change there reaches this AIOC only when this annex pins the new version.

| Rule | TOM section | Read here with |
|---|---|---|
| Labels and the honesty ceiling | Annex B | atoms of the organisation's sources and of an outside design; release elements keep their own provenance |
| Patterns are methods, never evidence | Annex B.5 | — |
| The Input Pack, its versions and its trace | §4.3, parts 1 to 3 and 6 to 8 | §4.3 of this blueprint |
| Needs requests, passes and the Missing Report | §5.2 | §5.2 of this blueprint |
| Decision rules: one decision per row; global assent is never approval; "don't know"; the weak-approval signal; delegated, not decided | `docs/CARRIED-RULES.md` §5 | — |
| The Review Panel rule | §5.8, rules 1 to 20 | the review points of §5.9; "DI Delivery Lead" for "TOM Design Lead" |
| The engine register | Annex E.12 | — |
| The value case and the priority of each element | Annex H.6, H.7 | §5.1, rule 1; the transition plan's waves; Annex A.1 and A.6 of this blueprint |

## Annex F. The gap checks

Version 1. Each check names its tier and whether code decides it. In mode B, a check that needs an element `not mapped` reads `unknown`.

| ID | Tier | Check | Decided by |
|---|---|---|---|
| B-01 | blocking | Every type of the Human Floor signature list the organisation will use has a deciding position in the decision-rights register | code |
| B-02 | blocking | Every critical process has an owner position, and each of its steps a position | code |
| B-03 | blocking | Every decision has exactly one deciding position and a limit, or a decision row for its limit | code |
| B-04 | blocking | Every step that signs, pays or commits money, or communicates outside carries a control, and no position breaks a segregation-of-duties rule without a decision | code |
| B-05 | blocking | Every position belongs to one unit and has one reporting line; every unit has a head position | code |
| B-06 | blocking | The authority matrix covers every decision class, and for each entity the signing positions are named | code, then the Gap Auditor |
| B-07 | blocking | Every legal obligation known from the sources is tied to a process and an owner position, or listed as unknown | the Gap Auditor |
| B-08 | blocking | The go or no-go deciding position is named | code |
| C-01 | completeness | Every policy in the policy register is held, or listed for a brief | code |
| C-02 | completeness | Every measure has a definition, a source, and a target or `not set` | code |
| C-03 | completeness | Every forum has a charter, a tier and a chair position | code |
| C-04 | completeness | Every position has a job description and a competence profile | code |
| C-05 | completeness | No position's workload figure is incomplete, and every peak finding is decided | code |
| C-06 | completeness | The systems, data and suppliers each process needs are stated | the Gap Auditor |
| C-07 | completeness | The crosswalk from today's organisation is complete, for an existing organisation | code |
| C-08 | completeness | Every decided process has its re-approval date | code |
| C-09 | completeness | The record each step leaves has a home | the Gap Auditor |
| C-10 | completeness | Every assumption in the design is decided, or listed | code |
| C-11 | completeness | Every return on the design has ended | code |

*Powered by 49GAION*
