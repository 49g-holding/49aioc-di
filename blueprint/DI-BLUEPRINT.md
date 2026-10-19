```yaml
# ── Blueprint metadata (machine-readable; the panel generator and the back-office builder read this block) ──
blueprint:
  aioc: "[ORG]AIOC-DI"
  parent: "[ORG]AIOC-CH"                  # example code of the Charter; each organisation writes its own Charter's code (Standard §1.7, item 13)
  full_name: "Delivery and Implementation"
  organisation: "<organisation>"          # filled in each organisation's own copy
  type: "specialised"
  org_aion: "[ORG]AION"
  blueprint_version: "v0.2.1"
  status: "draft"
  template:
    name: "49GAION AIOC Blueprint Template"
    version: "v1.6.0"
    source: "github.com/49g-holding/49GAION-aioc, template/AIOC-BLUEPRINT-TEMPLATE.md @ acdcbe5"
  mother:
    name: "49GAION Delivery and Implementation"
    version: "part card v1 (DRAFT)"
    source: "github.com/49g-holding/49GAION-protocol, library/cards/delivery-and-implementation.part-card.json and the Protocol section Delivery and Implementation (pull request #36); Standard §3.1, item 5 (49GAION pull request #68, DR-0017)"
  writing_repository: "<org>aioc-di"
  code_project: "<org>aioc-di, on the organisation's code platform"
  panel_register_id: "none yet"
  slice: "1 to 4, complete: launch essentials; accompany and operate; improve; small business"
  capabilities:
    standard: ["Chief of Staff", "Office", "Input socket", "Panel"]
    functional: ["Intake and Design Map", "Needs Requests", "Gap Audit", "Health Check", "Procedure Writing", "Briefs and Drafts", "Transition and Go-live Criteria", "Answers", "Independent Review", "Decision Package and Filing", "Light Design", "Implementation Plan", "Change Impact and Adoption", "Learning Paths", "Readiness and Go-live", "Problem Records", "Operating Rhythm", "Measures", "Value Register", "Versions and Checklists", "Process Watching", "Proposals", "Trials", "Hand-over and Mentor", "Export"]
```

# Blueprint · `[ORG]AIOC-DI` · Delivery and Implementation · `v0.2.1`

**Draft, 15 October 2026. v0.1.1 and v0.1.2, 16 October 2026: the answers to its returns, and the value case and priority carried unchanged (`decisions/DR-0002`, `DR-0003`). v0.2.0, 18 October 2026: complete, on the governing seat's direction to complete this stage (`decisions/DR-0004`). v0.2.1, 19 October 2026: the Chief of Staff takes its COS code `[ORG]CELL-COSDI` (`decisions/DR-0005`).** Written by `[ORG]AIOC-OCO` on the directions recorded in `decisions/DR-0001` to `decisions/DR-0004`. This is the blueprint of Delivery and Implementation, written for any organisation as the mother text of the Library part 49GAION Delivery and Implementation. It now covers **all four slices** of the product requirements: the gap audit and the launch essentials (slice 1); accompanying the launch, with the operating rhythm (slice 2); improving the running organisation (slice 3); and the small business with no design (slice 4). The slices stay the order in which the parts are built and switched on (§5.0, "The slices"). Every rule rests on a 49GAION text, on the blueprints of `[ORG]AIOC-PPD` or `[ORG]AIOC-TOM` (cited by section and version), or on the product requirements of this part (`PRD-[ORG]AIOC-DI-001` v0.4, in its code project), or is new here and marked **New**. Nothing here has run. Every fixed test reads `NOT_RUN`.

> **Delivery and Implementation in one page**
>
> Delivery and Implementation (DI) takes an organisation's decided design into a running organisation, and stays to run and improve it with the organisation. It is the last stage of the design chain, after Process and Position Design (PPD).
>
> **What goes in**
> 1. **Mode A:** the decided PPD release, handed over directly by `[ORG]AIOC-PPD`, by reference and hash, with the decided TOM release it was designed from.
> 2. **Mode B:** a design made elsewhere, filed as a source in Source Lifecycle.
> 3. **Mode C:** no design. The owner's sources, in Source Lifecycle; DI builds a light design with the owner. It is switched on only after the launch and accompany parts have given evidence.
> 4. The organisation's other sources, only from Source Lifecycle, and answers to what they do not say, asked only through its Chief of Staff.
> 5. Records of the organisation's work, only through a projection owned by top management that removes who did the work, and only after the organisation records its impact assessment.
>
> **What DI does, in four parts**
> 1. **Launch** (S0 to S4): admit the design; map it, or in mode C build a light design; audit the gaps in two tiers and run the health check at entry; prepare the procedures, briefs and drafts, the transition plan and the go-live criteria; the organisation decides each element, and the launch package is filed in Source Lifecycle.
> 2. **Accompany** (S5): the implementation plan by position; change impact and adoption; learning paths; readiness, rehearsals and the go or no-go package; problem records; stabilisation after go-live.
> 3. **Operate** (S6): the operating rhythm and its single logs; forum packs and minutes; measures; versions and acknowledgements; runnable checklists; quarterly priorities; the value register.
> 4. **Improve** (S7): watching processes and their conformance; findings; proposals; trials; new processes when the organisation changes; scheduled reassessment; the quarterly health check; and the hand-over of DI's skills, proven by a yearly drill without DI.
>
> All the while, any position may ask DI how the organisation works. DI answers only from the decided design, citing the element, its version and a quoted span, and a second engine checks every citation. Where the design is silent, DI says it does not know.
>
> **Who decides.** DI decides nothing for the organisation. What it may do is set per class of action by the owner position: level 0, read; level 1, propose (a draft enters a record only when a position inserts it); level 2, apply a reversible change with no legal, pay or employment effect, within a class the owner position signed in advance. No level allows a type of the Human Floor signature list. The go or no-go is always the deciding position's. Any accountable position can stop DI at once.
>
> **Processes, not persons.** DI addresses positions only, never ranks, scores or watches the occupant of a position, and shows no measure for a single position.

**Where this blueprint stands.** Complete draft, slices 1 to 4. The stages, their inputs, outputs and done-tests are set (§5.0). The review rule it shares with `[ORG]AIOC-PPD` and `[ORG]AIOC-TOM` is carried by section (§5.9; Annex E). The permission ladder is Annex G; records of work and their conditions are Annex H. The decisions only a human seat can take are listed once, in §13.

---

## 0. Identity and lineage

| Field | Value |
|---|---|
| Code | `[ORG]AIOC-DI`. Collision check (Naming Standard §5 and R6): the initials do not recreate `AIOC`, `AION` or `49GAION`, and do not read as a version suffix. The code is the one the Library part's Protocol section gives it in an `[ORG]AION`. Each organisation records it in its register before the repository is created (Naming Standard R9) |
| Full name | Delivery and Implementation |
| Description | "`[ORG]AIOC-DI` is `<organisation>`'s Delivery and Implementation core, built from 49GAION Delivery and Implementation" |
| Kind | AIOC |
| Parent | `<code of the Charter of this [ORG]AION>`; the cards use the example code `[ORG]AIOC-CH`. A top-level AIOC (Standard §1.7, item 13) |
| Inner units | `[ORG]CELL-DDL`, `[ORG]CELL-COSDI`, `[ORG]POD-DD`, `[ORG]POD-DP`, `[ORG]POD-DA`, `[ORG]POD-DR`, `[ORG]POD-DL`, `[ORG]POD-DO`, `[ORG]POD-DCI`: seven Pods with their twenty-five Cells, and two Cells directly under the AIOC (§17). No inner AIOC |
| HOAC label | `[ORG]HOAC-ACS`, held by its top Cell, the DI Delivery Lead `[ORG]CELL-DDL` (`label_holder`) |
| Accountable to | `<code of the Cell carrying [ORG]HOAC-TM>`; the cards use the example code `[ORG]CELL-TMS` (Naming Standard R15) |
| Type | Specialised: the organisation needs its decided design taken into a running organisation (§16) |
| `[ORG]AION` | `[ORG]AION`, based on 49GAION Standard `v1.6.0` |
| Versioned Definition | this file; the Panel and the Back office are built from it |
| Organisation | `<organisation>` |
| Made from | the Library part 49GAION Delivery and Implementation, part card `v1` (DRAFT), and its Protocol section, both merged on 15 October 2026 (`decisions/DR-0001`) |
| Template | 49GAION AIOC Blueprint Template `v1.6.0`, at `acdcbe5` |
| Mother | 49GAION Delivery and Implementation, part card `v1`. This text is its mother blueprint |
| Product requirements | `PRD-[ORG]AIOC-DI-001` v0.4, approved by the governing seat on 15 October 2026; its requirement IDs (`FR-n`, `NFR-n`) are cited here |
| Blueprint version and status | `v0.2.1` · draft · complete, slices 1 to 4 |
| Accountable seat (`[ORG]HOAC-ACS`) | the DI Delivery Lead, `[ORG]CELL-DDL`, a HOAC position. Who occupies it is top management's own mechanism; this AIOC never sees it (Standard §1.1, items 9 and 10) |
| Reports to | the Cell carrying `[ORG]HOAC-TM` |
| Writing repository | `<org>aioc-di`, plus `-records` for an organisation's runs and `-records-restricted` for run records that touch a Strictly confidential source (Naming Standard R9). The mother text lives in a public repository and holds no organisation data |
| Code project | `<org>aioc-di`, on the organisation's code platform; it holds the product requirements and the code |
| Panel | not yet built |
| Back office | not yet built |
| Attribution | Powered by 49GAION |

**Lineage.** A review of what an organisation still needs, after its processes and positions are designed, to start working without AI found that the decided design is not yet a working organisation: procedures, policy and pay drafts, authority instruments, controls, the transition plan and the go-live criteria are still missing, and the organisation needs someone beside it through launch and after. The governing seat directed a stage of its own for that, with an assistant that stays (`decisions/DR-0001`; `49GAION/DR-0017`). A study of fifteen products that design, launch or run organisations then placed each useful feature in the stage where it truly belongs. Both are summarised in `docs/HISTORY.md`. On 18 October 2026 the governing seat directed that this stage be completed: every requirement of the product requirements is designed here, and the slices stay the order of building (`decisions/DR-0004`). No earlier code or result is carried here.

---

## 1. Card (49GAION Operating Protocol §3)

```yaml
card:
  unit_kind: "AIOC"
  code: "[ORG]AIOC-DI"
  parent: "[ORG]AIOC-CH"                  # example code of the Charter, the root AIOC; only it has parent none (Standard §1.7, item 13)
  inner_units: ["[ORG]CELL-DDL", "[ORG]CELL-COSDI", "[ORG]POD-DD", "[ORG]POD-DP", "[ORG]POD-DA", "[ORG]POD-DR", "[ORG]POD-DL", "[ORG]POD-DO", "[ORG]POD-DCI"]
  type: "specialised"
  org_aion: "[ORG]AION"
  card_version: "v0.2.1"
  input_door: "Chief of Staff"
  wake: { method: "queue", verified: false }
  receives:
    - kind: "run request"                 # a Work Item from the Requesting Authority's Cell, through the HU input port; references only
      format: "Work Item (Protocol §4.1) whose sources field holds the mode (A, B or C), and one PPD Release reference, the reference of a design filed in Source Lifecycle, or (mode C) the references of the owner's sources"
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
    - kind: "service request"             # from the Requesting Authority's Cell, through the HU input port: switches on accompaniment, operation and improvement for a filed launch package; references only
      format: "Work Item (Protocol §4.1) whose sources field holds the filed launch package reference and the parts switched on (accompany, operate, improve)"
      acceptance_test: "TEST-DI v1, cases 55, 62"
      decision_needed: false
    - kind: "problem report"              # from any position, through the HU input port; never a source of the design
      format: "problem report from a position (its position code): the process or step, and what happened, text only"
      acceptance_test: "TEST-DI v1, case 61"
      decision_needed: false
    - kind: "decision"                    # a position's act on a row: decide, insert, approve a preview, acknowledge a version
      format: "decision reference; a signed record at the gateway for a listed type"
      acceptance_test: "TEST-DI v1, cases 10, 64, 70"
      decision_needed: false
    - kind: "records of work"             # through the projection owned by top management, only while process watching is on (Annex H)
      format: "record references through the tools-in connection, with no field that identifies who did the work"
      acceptance_test: "TEST-DI v1, cases 73, 74"
      decision_needed: false
    - kind: "change notice"               # from [ORG]AIOC-SL: a source that records a change of the organisation (a new product, site, market or law)
      format: "source reference (ID + version + hash) with its change kind"
      acceptance_test: "TEST-DI v1, case 78"
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
    - kind: "rows for decision"           # plan tasks, criteria, proposals, trials, priorities, value gates: each to the position that decides it
      format: "decision row with its draft, evidence and trace; the position decides or inserts it"
      usual_receivers: ["the deciding position the row names"]
    - kind: "forum pack"
      format: "forum pack (Annex A.15), built from versioned records"
      usual_receivers: ["the chair and member positions of the forum"]
    - kind: "notice"                      # a changed version, a re-approval due, an off-track item, a dropped follow-up, value or a date at risk
      format: "notice naming the record and its version"
      usual_receivers: ["the positions the record concerns"]
    - kind: "living design filing"        # each decided later version of a process, procedure, policy, job description or forum
      format: "versioned record, filed as a source of origin kind delivery and implementation; filing receipt"
      usual_receivers: ["[ORG]AIOC-SL"]
    - kind: "export"
      format: "full export with its trace, in open formats (§5.25)"
      usual_receivers: ["the Requesting Authority's Cell"]
  anatomy:
    panel: { health: { tests: true, metrics: ["stuck", "returned", "late", "run state", "returns open", "returns answered", "needs open", "needs past deadline", "gaps by tier", "gaps by state", "procedures by state", "briefs by state", "go-live criteria by state", "answers given", "answers 'I do not know'", "citations refused by the verifier", "reviews held", "review budget used", "tasks by state", "go-live criteria met, not met, unknown", "rehearsal defects open", "actions past their date", "risks and issues open", "milestone date changes", "packs built", "minutes awaiting preview", "versions due", "acknowledgements pending, by version", "initiatives by gate", "value planned and realised", "proposals by state", "trials running", "conformance by process", "hand-over items left", "ladder level by class"] } }
    back_office: { converses_with_humans: true, hosts: ["Chief of Staff", "Office"], protocol_traffic: true }
    definition: { location: "<org>aioc-di, blueprint/DI-BLUEPRINT.md", version: "v0.2.1" }
    delivery: { rollback: "one-click" }
    connectors:
      - { role: "design source", connector: "[ORG]AIOC-PPD release port", access_managed_in: "panel" }   # the grant is signed at the tool gateway as connect-external-port
      - { role: "returns to the operating model", connector: "[ORG]AIOC-TOM return port", access_managed_in: "panel" }
      - { role: "source of record", connector: "[ORG]AIOC-SL output socket", access_managed_in: "panel" }      # as above (Protocol §13, item 5)
      - { role: "records of work", connector: "the projection owned by top management over the organisation's own tools", access_managed_in: "panel" }   # read only; signed as connect-external-port; off until Annex H holds
    gateway: { metering_id: "<per-AIOC metering id>" }
  full_name: "Delivery and Implementation"
  version: "0.2.1"
  lineage: { id: "[ORG]AIOC-DI", version: "0.2.1", relation: "original" }
  lifecycle_state: "designed"
  blueprint_version: "v0.2.1"
  template_version: "v1.6.0"
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
    - { id: "di-light-design", name: "A light design built with the owner, every element provisional until decided", tags: ["delivery", "small business"] }
    - { id: "di-accompany", name: "The implementation plan, change impact, learning paths, readiness and the go or no-go package", tags: ["delivery", "launch"] }
    - { id: "di-operate", name: "The operating rhythm, logs, forum packs, measures, versions and the value register", tags: ["delivery", "operations"] }
    - { id: "di-improve", name: "Process watching at process level, conformance, proposals and trials", tags: ["delivery", "improvement"] }
    - { id: "di-hand-over", name: "Handing DI's skills to the organisation, proven by a drill without DI", tags: ["delivery", "capability"] }
  ports:
    - { unit: "[ORG]AIOC-DI", port: "ai-in", direction: "input", type: "AI", identification: "technical-key", accepted_content: ["release notice", "return answer", "source reference", "needs answer", "needs status", "change notice", "records of work through the projection"], authority_limit: "read only, within the scopes signed for the PPD, Source Lifecycle and records-of-work connections; return answers on the PPD and TOM connections; records of work only while process watching is on (Annex H)", audit_trail: "unit register; the serve logs of [ORG]AIOC-PPD and [ORG]AIOC-SL", required_tests: ["TEST-DI v1"], enforcement: "shared-gateway-outside-unit" }
    - { unit: "[ORG]AIOC-DI", port: "ai-out", direction: "output", type: "AI", identification: "technical-key", accepted_content: ["return", "needs request", "missing report", "needs status", "launch package filing", "living design filing", "export"], authority_limit: "returns, requests, reports and filings only; files only its own packages, decided versions and design reports; never an instruction to a person", audit_trail: "Work Item record and the unit register", required_tests: ["TEST-DI v1"], enforcement: "shared-gateway-outside-unit" }
    - { unit: "[ORG]AIOC-DI", port: "hu-in", direction: "input", type: "HU", identification: "live-human-sign-in-at-gateway", accepted_content: ["run request from the Requesting Authority's Cell (references only)", "service request from the Requesting Authority's Cell (references only)", "a question from a position about how the organisation works (never a source)", "a problem report from a position (never a source)", "a decision of a deciding position on a row", "an insertion, a preview approval or an acknowledgement by a position", "run control and configuration from the DI Delivery Lead (never a source)"], authority_limit: "the signer's authority_scope; nothing received here is a source", audit_trail: "Office record", required_tests: ["TEST-DI v1"], enforcement: "shared-gateway-outside-unit" }
    - { unit: "[ORG]AIOC-DI", port: "hu-out", direction: "output", type: "HU", identification: "live-human-sign-in-at-gateway", accepted_content: ["answer to the asking position", "run brief to the DI Delivery Lead", "ruling sheets to the DI Delivery Lead", "Decision Package rows to the deciding positions", "rows for decision to the deciding positions", "forum packs to the chair and member positions", "notices to the positions a record concerns", "a learning path and its check results to the learner position only", "filing notice to the Requesting Authority's Cell"], authority_limit: "information and proposals only; never a decision, an instruction or a question about a person", audit_trail: "Office record", required_tests: ["TEST-DI v1"], enforcement: "shared-gateway-outside-unit" }
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
    mapping_bars: { value: "<mode B mapping accuracy on a sample set, at or above>", set_by: "<Cell carrying [ORG]HOAC-TM>", date: "<date>", version: "<vN>" }
    deciding_positions: { value: "<position codes: go or no-go; counsel per jurisdiction; finance; data protection; owner, where not the Requesting Authority>", set_by: "<Requesting Authority Cell>", date: "<date>", version: "<vN>" }
    ladder: { value: "every class at level 1, a read-only class at level 0; level 2 only for a class the owner position signed as sign-standing-action-class (Annex G)", set_by: "<owner position>", date: "<date>", version: "<vN>" }
    ladder_thresholds: { value: "<per class: the fixed-test score at or above which it may move up>", set_by: "<owner position>", date: "<date>", version: "<vN>" }
    process_watching: { value: "off", set_by: "<Cell carrying [ORG]HOAC-TM>", date: "<date>", version: "<vN>" }       # on only when Annex H holds
    min_group: { value: 3, set_by: "<Cell carrying [ORG]HOAC-TM>", date: "<date>", version: "<vN>" }
    trial_baseline_points: { value: 10, set_by: "<owner position>", date: "<date>", version: "<vN>" }
    reassessment_schedule: { value: "<set by the organisation>", set_by: "<owner position>", date: "<date>", version: "<vN>" }
    health_check_schedule: { value: "quarterly", set_by: "<owner position>", date: "<date>", version: "<vN>" }
    drill_schedule: { value: "yearly", set_by: "<Cell carrying [ORG]HOAC-TM>", date: "<date>", version: "<vN>" }
    in_flight_rule: { value: "<set by the organisation>", set_by: "<owner position>", date: "<date>", version: "<vN>" }
    growth_triggers: { value: "<set by the organisation>", set_by: "<owner position>", date: "<date>", version: "<vN>" }
    reference_models: { value: "unavailable", set_by: "<DI Delivery Lead>", date: "<date>", version: "<vN>" }
    mentor: { value: "off", set_by: "<Cell carrying [ORG]HOAC-TM>", date: "<date>", version: "<vN>" }
    advice_bars: { value: "<advice quality on an expert-rated rubric, at or above>", set_by: "<Cell carrying [ORG]HOAC-TM>", date: "<date>", version: "<vN>" }
    council: { value: "off", set_by: "<Cell carrying [ORG]HOAC-TM>", date: "<date>", version: "<vN>" }
    point_of_work_guidance: { value: "off", set_by: "<Cell carrying [ORG]HOAC-TM>", date: "<date>", version: "<vN>" }
    language: { value: "<the organisation's language>", set_by: "<Cell carrying [ORG]HOAC-TM>", date: "<date>", version: "<vN>" }
```

**Joining the protocol.** This AIOC joins only after every input and output on this card passes fixed samples (the joining test, Protocol §11, item 1; Standard §3.2, item 4). It also needs `[ORG]AIOC-PPD` to send it release notices and accept its returns, `[ORG]AIOC-TOM` to accept its returns, and Source Lifecycle to accept filings of origin kind `delivery and implementation` (`upstream/PROPOSALS.md`, items 1 to 4). Until then its `lifecycle_state` stays `designed` and no Work Item is routed to it. Records of work are read only after Annex H holds; until then process watching is off and the rest of DI runs without it. The cards of its Pods and Cells are set in §17 and generated into `cards/`.

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
| **The deciding positions** | position codes set by the Requesting Authority (`deciding_positions`): the position that decides go or no-go; the counsel position for each jurisdiction; the finance position; the data-protection position; the owner position, where it is not the Requesting Authority. Each is a position of the organisation's decided design, never of this AIOC |
| **The owner position** | the position that sets the permission ladder and signs its level-2 classes (Annex G). It is the Requesting Authority, unless the Requesting Authority names another position for it in `deciding_positions` |
| **Process owner positions** | the owner position of each process in the decided design (PPD Release, process record, `owner_position`). Each decides changes inside its process, within its limits in the authority matrix |
| **The finance position** | named in `deciding_positions`. It alone approves gate L2 and confirms gate L5 of the value register (§5.19) |
| **The data-protection position** | named in `deciding_positions`. It records the impact assessment before any record of work is read (Annex H) |
| **The projection** | owned by top management (the Cell carrying `[ORG]HOAC-TM`). It turns records of the organisation's own tools into records of work by process, step, case type, site and system, with every field that identifies who did the work removed (Annex H). DI reads its output only |
| **The DI Delivery Lead position** | a HOAC position (`[ORG]HOAC-ACS`), a legal persona. Who occupies it is top management's own mechanism; this AIOC never sees it |
| **The design source** | `[ORG]AIOC-PPD`: it hands over its decided release directly, and receives this AIOC's returns on it |
| **The operating model** | `[ORG]AIOC-TOM`: its decided release is read by reference from Source Lifecycle; it receives this AIOC's returns on it |
| **The source of record** | `[ORG]AIOC-SL`: every other source, every question to the organisation, and every filing |
| **The engine register** | held at the tool gateway, in the Charter (Standard §4.4, item 11); read as `[ORG]AIOC-TOM` reads it (TOM blueprint `v0.5.0`, Annex E.12) |

### 2.2 Placement

- **Where it sits.** A top-level AIOC under the Charter, beside `[ORG]AIOC-SL`, `[ORG]AIOC-TOM` and `[ORG]AIOC-PPD`. It is the last stage of the design chain.
- **Its role.** It takes the decided design into a running organisation and stays with it. It prepares the launch, accompanies it, keeps the operating rhythm with the organisation, and helps it improve, until the organisation can do each of these without it (§5.24).
- **Scope.**
  - **It does:**
    - **Launch:** admit a decided PPD release (mode A) or a design made elsewhere (mode B), or build a light design with the owner (mode C); map it; return every defect of a release to the stage that made it; audit the gaps in two tiers; run the health check; write the procedures under each process; write briefs, and drafts from the organisation's own templates, for counsel and finance; draft the transition plan and the go-live criteria; prepare the decision; file the launch package.
    - **Accompany:** draft the implementation plan by position; set out what changes for each position, and how adoption is measured; build learning paths; assess readiness, write rehearsal scripts and prepare the go or no-go package; keep problem records; track stabilisation.
    - **Operate:** keep the operating rhythm and its single logs; build forum packs and draft minutes; build measures at process and unit level; keep versions with their re-approval dates and acknowledgements; run procedures as checklists; draft quarterly priorities; keep the value register.
    - **Improve:** watch processes through the projection, with their conformance; find bottlenecks, rework and control gaps; propose changes and new processes; design trials and have them judged by another seat; reassess the design on schedule; run the health check each quarter; hand its skills over and prepare the yearly drill without it.
    - **Always:** answer positions' questions from the decided design, with verified citations; trace every artefact both ways; export everything with its trace.
  - **It does not:** decide anything for the organisation, the go or no-go included; give legal, tax, employment or pay advice; state an amount that no source or decision gives; ask any person anything about the organisation; name a person, or read who occupies a position; rank, score or watch the occupant of a position, or show a measure for a single position; change a design release; read records of work except through the projection, after Annex H holds; apply a change outside a class signed at level 2 (Annex G); act on a type of the Human Floor signature list.
- **Shapes it serves.** Any shape the design covers: one owner's work, a single entity, a group of entities, or a group with independent institutions inside it. Where a design covers several entities or jurisdictions, every brief and every go-live criterion records its entity and jurisdiction.
- **Boundaries with other AIOCs.**
  - **`[ORG]AIOC-PPD`** designs processes, positions and units. This AIOC reads its decided release and returns defects; it never changes a release, and proposes later changes for decision (§5.22). A return is a request, never a change (§5.1; Annex B).
  - **`[ORG]AIOC-TOM`** designs the operating model. A defect this AIOC finds in a TOM element goes back to TOM by return.
  - **`[ORG]AIOC-SL`** holds every source and every contact with a person. This AIOC holds only references and its own records, and files its package and its returns there.
  - **`[ORG]AIOC-OCO`** installs, fixes and upgrades this AIOC; it never grades it (Standard §2.3, item 9).
  - **`[ORG]AIOC-OER`**, where the organisation runs it, gives every formal act one number. Where a decision of a forum entered in this AIOC's decision log is a formal act, the log holds the reference to its register entry, never a number of its own (§5.17, rule 2; Protocol §22).
- **Overlap.** None known. Where an organisation already holds procedures, policies, plans, logs or a workflow tool, they are sources, read through Source Lifecycle and mapped (§5.1); a workflow tool keeps running, and runnable procedures can be exported to it (§5.20).

---

## 3. Positions

| Position (standard title) | Purpose | Reports to | Run today by | Deputy |
|---|---|---|---|---|
| DI Delivery Lead | the accountable position of this AIOC and the owner of its path: owns the fixed tests of its parts; rules on contested review findings; accepts a reduced review level within the TM Cell's permission; attests the method. Answers for the method, never for the organisation's choices | the Cell carrying `[ORG]HOAC-TM` | a HOAC position (`[ORG]HOAC-ACS`); who occupies it is top management's own mechanism, never seen by this AIOC | as top management arranges (`appoint-acting-filler`, Standard §4.1, item 12) |
| Chief of Staff | keep each run moving, honest and traced; the only door to PPD, TOM and Source Lifecycle | DI Delivery Lead | an agent (`[ORG]CELL-COSDI`) | none; the run halts |
| Design Mapper | read a decided release, or map a design made elsewhere, and draft returns | Chief of Staff | an agent (`[ORG]CELL-DDM`) | none; the step halts |
| Gap Auditor | run the gap checks in two tiers | Chief of Staff | an agent (`[ORG]CELL-DGA`) | none; the step halts |
| Health Checker | run the organisation health check at entry | Chief of Staff | an agent (`[ORG]CELL-DHC`) | none; the step halts |
| Procedure Writer | write the procedure under each process | Chief of Staff | an agent (`[ORG]CELL-DPW`) | none; the step halts |
| Brief Writer | write the briefs for counsel and finance | Chief of Staff | an agent (`[ORG]CELL-DBW`) | none; the step halts |
| Transition Planner | draft the transition plan and the go-live criteria | Chief of Staff | an agent (`[ORG]CELL-DTP`) | none; the step halts |
| Answer Guide | draft each answer from the decided design | Chief of Staff | an agent (`[ORG]CELL-DAG`) | none; the question waits |
| Citation Verifier | check that each citation of an answer or a draft resolves and supports it | Chief of Staff | an agent (`[ORG]CELL-DCV`), on an engine of another family than the writer's | none; the answer waits |
| Blind Reviewer, seats A–C | review a locked output, alone first, then in debate | Chief of Staff | agents (`[ORG]CELL-DBRA` to `[ORG]CELL-DBRC`) | none; any seat covers another |
| Light Designer | build a light design with the owner, in mode C | Chief of Staff | an agent (`[ORG]CELL-DLD`) | none; the step halts |
| Implementation Planner | the implementation plan by position | Chief of Staff | an agent (`[ORG]CELL-DIP`) | none; the step halts |
| Change Analyst | what changes for each position; the stakeholder register; adoption measures | Chief of Staff | an agent (`[ORG]CELL-DCA`) | none; the step halts |
| Learning Builder | a learning path per position, with short checks | Chief of Staff | an agent (`[ORG]CELL-DLB`) | none; the step halts |
| Readiness Assessor | readiness, rehearsal scripts, the go or no-go package and stabilisation | Chief of Staff | an agent (`[ORG]CELL-DRA`) | none; the step halts |
| Issue Analyst | problem records and the issue list of each forum | Chief of Staff | an agent (`[ORG]CELL-DIA`) | none; the record waits |
| Rhythm Keeper | the operating rhythm, its logs, forum packs, draft minutes and quarterly priorities | Chief of Staff | an agent (`[ORG]CELL-DRK`) | none; the pack waits |
| Measures Builder | measures and dashboards at process and unit level | Chief of Staff | an agent (`[ORG]CELL-DMB`) | none; the dashboard keeps its last version |
| Value Tracker | the initiative and value register | Chief of Staff | an agent (`[ORG]CELL-DVT`) | none; the register keeps its last version |
| Process Analyst | process watching, conformance and findings | Chief of Staff | an agent (`[ORG]CELL-DPA`) | none; watching pauses |
| Change Proposer | proposals, new processes and reassessment findings | Chief of Staff | an agent (`[ORG]CELL-DCP`) | none; the proposal waits |
| Trial Designer | the design of each trial before it starts | Chief of Staff | an agent (`[ORG]CELL-DTD`) | none; the trial does not start |
| Trial Judge | judge each trial by its decided rules, on an engine of another family than the proposer's | Chief of Staff | an agent (`[ORG]CELL-DTJ`) | none; the trial runs to its default |
| Capability Mentor | the hand-over of DI's skills, the drill's preparation, and advice from the skills library | Chief of Staff | an agent (`[ORG]CELL-DCM`) | none; the item waits |

- **Every human position is a HOAC position.** This AIOC has one, the DI Delivery Lead. The organisation may add more in this AIOC's own design (§17).
- **Present as positions** (Standard §1.1, items 9 and 10). Every human this AIOC deals with, its own Lead and the organisation's positions, is present as a position. It addresses positions only, through their HU ports.
- The **Requesting Authority** and the **deciding positions** are not positions of this AIOC (§2.1). They decide; this AIOC prepares the decision.
- No AI Cell signs anything (Protocol §10, item 3). Each AI Cell's bot has its own identity card (§17).
- The trace query, the package manifest, the checks of §5, the version register, the acknowledgements and notices, the checklist runner, the dashboards' refresh, the export and the ladder's own record are code steps of the Chief of Staff, never a Cell. Code is a tool, never a seat.
- **Three of them judge or check work of another Cell** and are kept apart from it: the Citation Verifier and the Trial Judge each run on an engine of another family than the writer's or the proposer's; the Blind Reviewers review only outputs they did not write.

---

## 4. Standard capabilities

Defaults are in `docs/STANDARD-CAPABILITIES.md` of `49GAION-aioc` at `acdcbe5` (`v1.6.0`). The differences are listed in §11.

### 4.1 Office
#### Definition
Default · form: **single Chief of Staff**. An Office forms only if the Delivery Lead needs more than one Chief of Staff; it is proposed to the Delivery Lead, never self-created.
#### Process (SOP)
Default.
#### Role card
None while the form is a single Chief of Staff.
#### Fixed test
TEST-DI-COSDI v1 (TEST-DI v1, case 44) · result `NOT_RUN`

### 4.2 Chief of Staff
#### Definition
Default, **managing** kind, with these additions:
- **The only door.** It is the only Cell of this AIOC that sends anything outside it: returns to `[ORG]AIOC-PPD` and `[ORG]AIOC-TOM`; needs requests, Missing Reports and filings to `[ORG]AIOC-SL`; answers, Decision Package rows, rows for decision, forum packs, minutes previews, learning paths and notices to positions, through the HU output port. The external ports sit on its card (§17).
- **No question about a person, and none to a person about the organisation.** Every question for the organisation goes to the Chief of Staff of `[ORG]AIOC-SL` as a needs request (§5.2). It sends a position only an answer it was asked for, a row for decision, a pack or preview for a forum it belongs to, its learning path, or a notice about a record that concerns it.
- **An orchestrator that never judges itself.** It runs the gates (Annex C), dispatches the Cells, locks outputs, runs the code steps, draws the reviewers and writes the run record. It never rules on a finding, never dismisses or downgrades one, never lowers a review, and never decides for a deciding position.
#### Process (SOP)
Default, plus:
1. **Admission (S0).** On a run request: open the run record; check that the request carries references only and names an enabled mode; receive or fetch the release notice (mode A) or the design's source reference (mode B); have the Input socket build Input Pack P0 (§4.3); check gate T0 (Annex C.2) → *P0 and the T0 record* (evidence: the T0 record, with P0's ID).
2. **One run at a time per organisation.** A second run in parallel needs the Delivery Lead's approval, recorded in the run record.
3. **Returns.** Collect the return drafts; have each reviewed; send each to the stage that made the release, under the design return contract, and file it into `[ORG]AIOC-SL` with the same hash; mark the elements it touches `held: return open`; count its rounds; past `return_round_deadline` or `return_rounds_max`, put it to the Requesting Authority, who answers it or sets it aside on a stated basis → *return sent; return ended* (evidence: the return, its filing receipt and its end).
4. **Passes.** Batch needs candidates into passes of at most `rows_per_pass` rows, one decision per row, each with its Missing Report.
5. **Questions.** On a question from a position, dispatch the Answer Guide, then the Citation Verifier; send the verified answer, or "I do not know", to the asking position only; record the question by ID, never as a source (§5.8).
6. **Code steps.** Run the checks of §5.1 to §5.7, the trace query (§5.10) and the package manifest → *generated parts* (evidence: re-generated byte-identical).
7. **Stops and revocation.** A stop from any accountable position takes effect at the gateway on every part, and on any draft in flight; the Chief of Staff is itself stopped. A stop may also name one change this AIOC applied: that change is rolled back at once (FR-34). A revoked connection holds the run as `held: connection revoked`.
8. **The service (S5 to S7). New in v0.2.0.** On a service request: check that it carries references only, names a filed launch package that reads back by its hash, and names the parts switched on; open the service record; dispatch as §5.0 sets → *service record* (evidence: the record, with the package ID).
9. **Rows and insertions.** Send each draft to the position that decides it, as a row. Enter a draft into a record, log or plan only when that position inserts it (level 1), or apply it within a signed class (level 2, step 15) → *row decided or inserted* (evidence: the decision reference).
10. **Versions, notices and acknowledgements.** Keep the version register; raise a notice on each re-approval due and on each changed version, to every position it concerns; record each acknowledgement by version and position code (§5.20) → *version register* (evidence: the notices and acknowledgements by version).
11. **Checklists.** Run each procedure as a checklist per case, or export it to the organisation's own workflow tool (§5.20).
12. **Records of work.** Admit records of work only through the projection, and only while Annex H holds. Refuse whole any record with a field that identifies who did the work, and keep nothing of it (Annex H, rule 3).
13. **Rolling up.** Before any measure, finding or view leaves this AIOC, check by code that it describes a process, a step or a unit, never a position, and that it rests on at least `min_group` positions; otherwise roll it up to the parent unit (Annex H, rule 5).
14. **Export.** On a request of the Requesting Authority's Cell, produce the full export with its trace (§5.25).
15. **Level 2 and rollback.** Apply a level-2 change only within a class the owner position signed, as a new version with one-step rollback, and report it to the owner position the same day. Any error, complaint or change of engine drops the class to level 1 at once (Annex G).
#### Role card
| Field | Content |
|---|---|
| Name | Chief of Staff |
| Position and seat | the position Chief of Staff; accountable seat: the DI Delivery Lead (`[ORG]HOAC-ACS`) |
| Performed by | an agent (`[ORG]CELL-COSDI`, full name DI Chief of Staff) |
| Purpose | keep each run moving, honest and traced; be this AIOC's voice to the Delivery Lead and its only door to PPD, TOM, Source Lifecycle and the asking positions |
| Authority limits | alone: dispatch, lock, record, run code steps, send reviewed returns and needs requests, send verified answers, file a package or a version whose elements are decided; send rows for decision, forum packs and notices; enter a draft a position inserted; apply a level-2 change within its signed class; run checklists; record acknowledgements; produce the export; needs the Delivery Lead: a second run in parallel, a budget above the cap, any change to configuration, a ruling on a finding, a reduced review level; never: ask a person anything about the organisation, change a design release, decide for a deciding position, enter a draft no position inserted, apply a change outside a signed class, read a record of work outside the projection, show a measure for a single position, rule on or dismiss a finding, sign, close a Work Item this AIOC performed |
| Write location | the run record and this AIOC's Work Items |
| Reports to | the DI Delivery Lead |
| Escalation | to the Delivery Lead in one line, with evidence linked; a stop goes to the stop door, never through this Cell |
| Tools and access | the PPD, TOM and Source Lifecycle connections, and the projection's connection while Annex H holds, through the tool gateway, within their signed scopes; the code steps of the code project; no credential in any instruction |
| Deputy and cover | none; on failure the run halts and the Delivery Lead is told |
| Fixed test and score | TEST-DI-COSDI v1 (§9), plus the default Chief of Staff test |
| Card version and status | v0.2.0 · draft |
#### Fixed test
TEST-DI-COSDI v1 · result `NOT_RUN`

### 4.3 Input socket
#### Definition
Default, with this AIOC's standard format, the **Input Pack**, as in the TOM blueprint `v0.5.0` §4.3, parts 1 to 3 and 6 to 8, read with these changes:
1. **Three kinds of input.** The **releases** (mode A): the decided PPD Release, by manifest and parts, from the release notice, and the decided TOM Release it names, read by reference from Source Lifecycle. The **outside design** (mode B): a source in Source Lifecycle, cut into atoms and labelled once (TOM Annex B, carried). The **other sources**: by reference from Source Lifecycle's output socket.
2. **A release is read, never atomised as a source.** Its elements keep their own IDs. Every element of this AIOC's output traces to a release element or a source atom.
3. **The release check.** A release is admitted only when its manifest validates, its final status is decided, and its hash equals the copy filed in Source Lifecycle; the PPD Release must name the TOM Release it was designed from, and that release must pass the same check, with its role register re-compiling from its parts. Otherwise nothing of it is used, and a return goes back with the failed condition.
4. **A new release** makes a new pack version. The elements that changed re-open the work that cites them; decided work that cites nothing changed is kept by hash.
5. **Nothing that arrives through a human port is a source.** A run request is admitted only if it carries references. A question from a position is never a source and never changes the design.
6. The pack's ID is `DII-` followed by the SHA-256 of its body.
7. **Mode C. New in v0.2.0.** The owner's sources in Source Lifecycle are cut into atoms and labelled as in mode B. There is no design to map: the Light Designer builds one with the owner (§5.11).
8. **Records of work are not sources of the design.** They enter only through the projection, while Annex H holds, by reference, with no field that identifies who did the work. An item with such a field is refused whole, and nothing of it is kept.
9. **Change notices** from Source Lifecycle enter as source references with their change kind (a new product, site, market or law), and open the work of §5.22.
#### Process (SOP)
Default (receive, identify, normalise, check, deliver), run by the Chief of Staff through the socket's code steps. A refused item comes back with its reason and never enters.
#### Role card
Default; performed by the Chief of Staff (`[ORG]CELL-COSDI`) through the socket's code steps.
#### Fixed test
TEST-DI v1, cases 1, 2, 18 to 22, 51, 73, 74, 78, 92 · result `NOT_RUN`

### 4.4 Panel
#### Definition
Default. The Panel also shows, for each run: the run state and its flags with their ages; the mode; the releases or the design in use, and any newer release; every return, with its round, state and age; every needs request; each gate with its result; the gaps by tier and state; each procedure, brief and go-live criterion with its decision state; the questions answered and those answered "I do not know"; per review, its point, verdict and findings. For the service it shows: tasks by state; the go-live criteria and stabilisation; rehearsal defects; the logs, with items past their date; packs and minutes awaiting preview; versions due; acknowledgements pending, by version only; initiatives by gate, with value planned and realised; proposals and trials; conformance by process; hand-over items left; the ladder level of each class. It shows no measure for a single position, and every figure rests on at least `min_group` positions (Annex H, rule 5). Every output is in the organisation's language (`language`, NFR-08).
#### Process (SOP)
Default.
#### Role card
Default.
#### Fixed test
Default Panel test · result `NOT_RUN`

---

## 5. Functional capabilities

The launch has five stages (§5.0, S0 to S4), performed by the Input socket (§4.3: S0) and these capabilities: Intake and Design Map, or Light Design in mode C (S1); Gap Audit and Health Check (S2); Procedure Writing, Briefs and Drafts, and Transition and Go-live Criteria (S3); Decision Package and Filing (S4). The service has three parts: Accompany (S5: §5.12 to §5.16), Operate (S6: §5.17 to §5.20) and Improve (S7: §5.21 to §5.24). Needs Requests (§5.2), Answers (§5.8) and Export (§5.25) are services. Independent Review (§5.9) closes every stage. Each capability is written in the four-part form (Annex A of the template), with one added row, **Done when**. Each step reads: **position**: action → *output* (evidence). Annexes: A (the parts and their field lists), B (returns), C (run states and gates), D (what this AIOC never does), E (rules carried), F (the gap checks), G (the permission ladder), H (records of work).

**One word per meaning.**
- **Release**: a decided design release this run reads (PPD or TOM). **Outside design**: a design made elsewhere, read as a source (mode B). **Design**: either.
- **Launch package**: the output of the launch, S0 to S4 (Annex A.1 to A.8).
- **Gap** (`GAP-n`): a check of Annex F that the design fails. **Brief** (`BRF-n`): a draft for counsel or finance. **Criterion** (`GLC-n`): a go-live criterion.
- **Deciding position**: the position that decides a row (§2.1). **Return** (`DIR-n`): this AIOC's notice to the stage that made a release (Annex B).
- **Service**: the work after the launch package is filed: Accompany (S5), Operate (S6) and Improve (S7). **Living design**: the decided design as the organisation keeps it after launch, each later decided version filed in Source Lifecycle.
- **Insert**: a position's act that enters a draft of this AIOC into a live record, log or plan. **Apply**: this AIOC's own act at level 2, within a signed class (Annex G).
- **Task** (`TSK-n`), **Problem** (`PRB-n`), **Initiative** (`INI-n`), **Finding** (`FND-n`), **Proposal** (`PRP-n`), **Trial** (`TRL-n`): the records of the service, in Annex A.

### 5.0 The stages: input, output, done-test

| ID | Plain name | Run state | Gate | Exact input | Exact output | Done-test | Human decision |
|---|---|---|---|---|---|---|---|
| S0 | **Admit** | `admitting` | T0 | The run Work Item (references only). Mode A: the release notice of `[ORG]AIOC-PPD`. Mode B: the outside design's reference in Source Lifecycle. The connection grants. The engine register. | Input Pack `P0`; the run record, opened. | **T0** (Annex C.2): references only; an enabled mode; the release check (§4.3, part 3) or the source check passes; the connections are signed and in scope; `requesting_authority_cell` and `deciding_positions` are set; RP0 settled. | Requesting Authority: opens the run; names the deciding positions. |
| S1 | **Map** | `mapping` | T1 | P0. | The **design map** (Annex A.1); return drafts (Annex B). | **T1**: mode A: every process, position, unit, decision, control and forum in scope is `used`, `returned` or `out of scope` with a reason; mode B: every element of the outside design is `mapped`, `not mapped` (with the reason) or `out of scope`, and none is rewritten; every return draft passed RP1 and was sent. | Requesting Authority: the scope, if the request did not name it; mode B rows `not mapped`. |
| S1C | **Build** (mode C) | `building` | T1C | P0: the owner's sources. | The **light design** (Annex A.20), every element `provisional` until decided. | **T1C**: every element of the light design is `provisional` or decided, with its source atoms or the decision that made it; no element states a number that no source or decision gives; no element gives legal, tax, employment or pay advice; where one position holds every seat, the design says so and offers a compensating control as a draft; RP1 settled. S2 to S4 then run on the light design as on a design map. | The owner position: each element. |
| S2 | **Diagnose** | `diagnosing` | T2 | The design map; P0. | The **gap report** (Annex A.2); the **health check** (Annex A.3). | **T2**: every check of Annex F has a result (`met`, `gap`, `unknown`) with evidence; every gap has its tier, consequence, evidence, proposed fix and route; every item of the health check has a result with evidence; RP2 settled with no unresolved `MATERIAL` finding. | Requesting Authority: the route of each gap (return, decision, or prepare). |
| S3 | **Prepare** | `preparing` | T3 | The design map; the decided gap routes; P0. | The **procedures** (Annex A.4), critical processes first; the **briefs** (Annex A.5); the **transition plan** and the **go-live criteria** (Annex A.6). | **T3**: every procedure step traces to a process step; every brief carries its entity, jurisdiction, draft mark and addressee position; every go-live criterion has its measure, evidence source and a threshold that is a decision row; the go or no-go deciding position is named; every citation passed the Citation Verifier; RP3 settled with no unresolved `MATERIAL` finding. | Requesting Authority: assumptions; contradictions with the design. |
| S4 | **Decide and file** | `deciding`; end states `filed` | T4, then T5 | Every reviewed part of S1 to S3, by hash; the settled review records. | The **Decision Package** (Annex A.8); then the **launch package** manifest and its parts; the filing receipt; the notice to the deciding positions. | **T4**: every element decided (`ACCEPT`, `CORRECT`, `REJECT`) by its deciding position; silence decided nothing. **T5**: the manifest is content-addressed; every element traces to a design element or a source atom; the package lint passes; the package is filed and reads back by hash. | The deciding positions: each element. The Delivery Lead: the attestation. |
| S5 | **Accompany** | `accompanying`; end state `stabilised` | T6, then T7 | The filed launch package, by hash; the service request; the Input Pack versions. | The **implementation plan** (A.9); the **change impact** and the **stakeholder register** (A.10); **learning paths** (A.11); the **readiness record**, **rehearsal scripts** and **defect log** (A.12); the **go or no-go package** and the **stabilisation record** (A.13); **problem records** (A.18). | **T6** (go-live): every task has an owner position, its dependencies and a date, decided; every go-live criterion reads `met`, `not met` or `unknown`, with evidence; every rehearsal script traces to a step; the go or no-go package is complete; RP5 settled. **T7** (stabilised): every stabilisation criterion is decided `met` by its deciding position. | The go or no-go position: go or no-go, signed as `accept-irreversible-risk`. The owner position: the plan and the end of stabilisation. |
| S6 | **Operate** | `operating`, a standing state worked in cycles | T8, each cycle | The living design; the logs; the decided measures and targets; the value register. | The **operating rhythm**, its **logs** and the **quarterly priorities** (A.14); **forum packs** and **minutes** (A.15); **measures** and **dashboards** (A.16); the **version register**, **acknowledgements** and **checklist runs** (A.17); the **value register** (A.19). | **T8**, per cycle: every pack is built only from versioned records; no minute enters a log without its approved preview; every action and decision has an owner position and a date; every measure is at process or unit level and rests on at least `min_group` positions; every value figure traces to its baseline; RP6 settled on the cycle's sample. | Each forum's chair: its pack. The participants: the preview of the minutes. The finance position: gates L2 and L5. Each position: its priorities, by insertion. |
| S7 | **Improve** | `improving`, a standing state worked in cycles | T9 per proposal; T10 per trial | Records of work through the projection (Annex H); the living design; change notices; the schedules. | **Conformance records** and **findings** (A.21); **proposals** (A.22); **trial records** (A.23); returns to PPD or TOM; the **health check** each quarter (A.3); **hand-over records** and the **drill record** (A.24). | **T9**: every proposal states its evidence, expected effect and risk, cites its triggering record where it has one, and reaches the position the authority matrix names; RP7 settled. **T10**: before a trial starts, its expected result, guardrail measure, duration, rollback trigger and default are decided; after it ends, the Trial Judge judges it on those rules. | The process owner, or the position the authority matrix names: each proposal and each trial's result. The Cell carrying `[ORG]HOAC-TM`: the drill's result. |

**Services and rules used by every stage.**

| Name | What it is | Output | Done-test |
|---|---|---|---|
| **Returns** (§5.1) | A stage that finds a defect in a release drafts a return; the Chief of Staff sends it after review | a return (Annex B) | Annex B, Done when |
| **Asking** (§5.2) | Every stage raises needs candidates; the Chief of Staff asks the Chief of Staff of `[ORG]AIOC-SL` | needs requests; one Missing Report per pass | each request ends answered by reference or with another outcome of the needs-answer contract |
| **Answers** (§5.8) | Any position may ask how the organisation works, at any time | an answer with verified citations, or "I do not know" | §5.8, Done when |
| **Review** (§5.9) | The rule that closes every stage | a review record and a verdict | §5.9, Done when |
| **Export** (§5.25) | Everything this AIOC holds for the organisation, with its trace, at any time | the export and its manifest | §5.25, Done when |
| **Problem records** (§5.16) | Any position may report a problem, at any time after launch begins | a problem record that ends in a decision or an action | §5.16, Done when |

**Run states.** The launch: `admitting` (S0) → `mapping` (S1), or `building` in mode C (S1C) → `diagnosing` (S2) → `preparing` (S3) → `deciding` (S4) → `filed`. The service: `accompanying` (S5) → `stabilised`; `operating` (S6) and `improving` (S7) are standing states, each worked in cycles. Endings, flags and holds: Annex C.1.

**The slices.** The product requirements build this AIOC in four slices, each usable on its own (`PRD-[ORG]AIOC-DI-001` v0.4). Every slice is designed here; the slices stay the order in which its parts are built and switched on.
1. **Slice 1, launch** (S0 to S4; modes A and B; FR-01 to FR-03, FR-05 to FR-13, FR-15, FR-33, FR-34, FR-43): on when the AIOC joins.
2. **Slice 2, accompany and operate** (S5, S6; FR-14, FR-16 to FR-18, FR-20 to FR-22, FR-35 to FR-37, FR-40 to FR-42): on by a service request for a filed launch package.
3. **Slice 3, improve** (S7; FR-19, FR-23 to FR-26, FR-38, FR-39, FR-43): proposals, trials, reassessment, the quarterly health check and the hand-over switch on with the service. Process watching and conformance switch on only when Annex H holds. Level 2 applies only to a class the owner position signed (Annex G).
4. **Slice 4, small business** (S1C; FR-04): mode C switches on only when the Cell carrying `[ORG]HOAC-TM` records that slices 1 and 2 have given evidence (§13, H-21), and then through `modes_enabled`. The later parts are written here too: reference models, the full mentor, the multi-engine council and guidance at the point of work (FR-27 to FR-29, FR-44). Each stays off until its own switch is set (§15).
5. **The tools** (FR-30 to FR-32) serve every slice (§5.25; §6).

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
| Rules | 1. **Mode A: account for everything.** Every process, position, unit, decision, control and forum of the PPD Release in scope, and every role and hand-off of the TOM Release it names, is recorded `used`, `returned` (with the return) or `out of scope` (with the reason). **New** in v0.1.2: the value case of that TOM Release and the decided priority of each element (TOM blueprint `v0.6.0`, Annex H.6, H.7) are recorded in the design map as they stand, by reference, never changed; a baseline `unknown` or a target `not set` stays so. They are carried for the register of value, which starts from them (§5.19). 2. **Mode B: map, never rewrite.** **New** in v0.2.0: the outside design may arrive in Source Lifecycle as documents, spreadsheets, PDF files or the exports of process-modelling tools (BPMN among them); Source Lifecycle cuts it into atoms. Mapping accuracy is measured on a sample set against `mapping_bars` (a decision) before first use. Each element of the outside design is mapped onto the structure of a PPD release (process, step, decision, position, unit, forum, policy, measure), or marked `not mapped` with the reason. The author's words are kept as cited; the map records how each element was read, never what it should have said. A missing element is a gap (§5.3), never an invention. 3. **Never changed.** A release is read as decided. A defect becomes a return of one kind (Annex B) to the stage that made it: a process, position, unit or control defect to `[ORG]AIOC-PPD`; an operating-model defect to `[ORG]AIOC-TOM`. 4. **The touched elements wait.** Only the elements a return touches are held; the rest of the work goes on. 5. **The loop ends.** A return counts its rounds. Past `return_round_deadline` or `return_rounds_max`, it goes to the Requesting Authority, who answers it, or sets it aside and lets the affected elements go forward on a stated basis, a known defect or a decided assumption (49GAION Standard §3.1, items 4 and 6). 6. **Not a person.** A return names release parts, elements and fact-types, never a person. |

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
| Trigger | T1 passed; in the service, `health_check_schedule` |
| Inputs | the design map; the Input Pack; in the service, the living design, the logs and the measures |
| Outputs | the health check (Annex A.3) |
| Performed by | the Health Checker (`[ORG]CELL-DHC`) in the Diagnosis Pod (`[ORG]POD-DD`) |
| Done when | T2 (§5.0); in the service, each quarter's record is delivered and settled at RP7 |
| Rules | 1. **A fixed checklist** of items under the six headings, versioned; each item `met`, `not met` or `unknown`, with evidence. 2. **The organisation only.** It scores the organisation, never a position's occupant, and never ranks one part against another. 3. **No outside benchmark** is used as evidence. 4. **At entry, then each quarter.** It runs at entry (S2), and in the service on `health_check_schedule` (FR-43). A later check is compared only with the organisation's own earlier checks, item by item, never with another organisation. |

#### Process (SOP)
1. **Health Checker**: answer each item with evidence → *health check, draft*.
2. **Chief of Staff**: run RP2 with the gap report → *settled review*.

#### Role card
| Field | Content |
|---|---|
| Name | Health Checker |
| Position and seat | Health Checker; accountable seat: the DI Delivery Lead |
| Performed by | an agent (`[ORG]CELL-DHC`, full name DI Health Checker) |
| Purpose | the health check at entry, and each quarter in the service |
| Authority limits | alone: answer the checklist; never: score a person, rank parts, use an outside benchmark as evidence |
| Write location | the run record |
| Reports to | Chief of Staff |
| Escalation | to the Chief of Staff |
| Tools and access | the design map and the Input Pack; a fresh context per dispatch |
| Fixed test and score | TEST-DI-DHC v1 (§9) |
| Card version and status | v0.2.0 · draft |

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

### 5.6 Briefs and Drafts

#### Definition
| Field | Content |
|---|---|
| Name | Briefs and Drafts |
| Purpose | hand counsel and finance what they need to write the texts with legal or money effect: policies, the pay structure, contract and offer templates, authority instruments, the obligations register, the control matrix, and the systems, data and suppliers each process needs; and, where the organisation holds its own templates, the drafts themselves, and the cost draft (FR-07 to FR-12) |
| Trigger | T2 passed |
| Inputs | the design (the policy register, the position register with job families and levels, the decision-rights register and authority matrix, the controls catalogue, the units); the decided gap routes; the jurisdictions and entities in scope |
| Outputs | the briefs (Annex A.5) |
| Performed by | the Brief Writer (`[ORG]CELL-DBW`) in the Preparation Pod (`[ORG]POD-DP`) |
| Done when | T3 (§5.0) |
| Rules | 1. **A brief, not the text.** Each brief states what the text must achieve, the design elements it serves, what is known, and the open questions. It is never the final text, and never advice. 2. **Entity and jurisdiction.** Each brief records its legal entity and its jurisdiction; where the jurisdiction is unknown, it writes an outline only. 3. **The mark.** Each brief carries "Draft, not legal advice" and is addressed to the counsel or finance position named in `deciding_positions`. 4. **No amount.** A brief states no pay amount, price or budget figure; it lists the decisions needed. The pay structure brief works from job families and levels and asks for objective, gender-neutral evaluation criteria. 5. **Positions only.** Contract, offer and authority briefs use position placeholders; no brief names a person or prepares a named offer. 6. **Every citation is verified** (§5.8, rule 3). 7. **Drafts from the organisation's own templates. New in v0.2.0.** Where the organisation holds, as a source, a template for a text and a jurisdiction, decided by its counsel position for that jurisdiction, the Brief Writer drafts the text from that template (FR-07, FR-08, FR-10). The draft keeps rules 2 to 5, and goes to decision only after the counsel position for its jurisdiction has reviewed it (`reviewed_by`). Without such a template it writes the brief only. 8. **Pay** (FR-08). Grades and pay ranges are drafted per job family and level, on objective, gender-neutral job-evaluation criteria; every range is reviewed by the counsel position for its jurisdiction, then decided by the finance position; no named offer is ever produced. 9. **The cost draft** (FR-09). It needs no template. The cost of the organisation and the first operating budget are drafted only from figures that sources or decisions give (cost rates, volumes, prices), each cited. A figure no source gives stays `not given` and becomes a needs request. Every line traces to a position, a process or a need, and code checks the totals against the limits of the authority matrix. It records its entity and jurisdiction, carries the mark, and is addressed to the finance position. It is the one part that holds amounts, and every amount cites its source or decision row. 10. **Obligations** (FR-11). The obligations register ties each obligation to a process, an owner position and a control. A change of law recorded in Source Lifecycle flags the obligations it touches (§4.3, part 9): flags only; counsel and the owner decide. 11. **Systems and fit to standard** (FR-12). The systems, data, facilities and suppliers each process needs follow the delivery model of the TOM Release. Where a system is chosen, each designed process is compared with the system's standard process, and every gap is a decision row: change the process, or configure the system. 12. **The control matrix** (FR-10) is drafted per step from the PPD Release's controls catalogue and segregation-of-duties rules. Every row cites its control and its step. |

#### Process (SOP)
1. **Brief Writer**: write each brief → *brief drafts*.
2. **Citation Verifier**: check every citation → *verification record*.
3. **Chief of Staff**: run the brief lint by code (mark, entity, jurisdiction, addressee, no amount except in the cost draft, where every amount is cited; no name), then RP3 → *settled review*.

#### Role card
| Field | Content |
|---|---|
| Name | Brief Writer |
| Position and seat | Brief Writer; accountable seat: the DI Delivery Lead |
| Performed by | an agent (`[ORG]CELL-DBW`, full name DI Brief Writer) |
| Purpose | the briefs, and the drafts from the organisation's own templates, for counsel and finance |
| Authority limits | alone: write briefs and drafts; never: write a final legal or policy text, give advice, state an amount that no source or decision gives, name a person |
| Write location | the run record |
| Reports to | Chief of Staff |
| Escalation | to the Chief of Staff |
| Tools and access | the design and the Input Pack; a fresh context per dispatch |
| Fixed test and score | TEST-DI-DBW v1 (§9) |
| Card version and status | v0.2.0 · draft |

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
| Rules | 1. **Only from the design.** An answer cites, for each claim, the design element, its version and a quoted span. A claim with no citation is removed. 2. **"I do not know."** Where the design is silent, the answer says so, and may name the stage or the deciding position that could settle it; it never guesses. 3. **A second engine checks.** The Citation Verifier, on an engine of another family than the writer's, checks that each citation resolves and supports its claim. An answer, a procedure, a brief or a criterion with a citation that fails is not sent. 4. **A question is not a source.** It never changes the design, and it is recorded by ID only. 5. **To the asker only.** The answer goes only to the asking position. 6. **Not about persons.** A question about a person, or about who occupies a position, is answered "outside what DI holds". 7. **Bars.** Grounded answers and "I do not know" on unanswerable questions are measured on a fixed question set against `answer_bars` (a decision) before first use. 8. **At the point of work** (FR-44). **New** in v0.2.0. Where `point_of_work_guidance` is on, a position may ask from inside the tools it uses. The question reaches the HU input port through the gateway, under that position's sign-in, and the answer follows rules 1 to 7. Adoption funnels per process step are built only from records of work through the projection, aggregated (§5.18); no usage data per person is kept. 9. **A problem is not a question.** A report that something went wrong goes to Problem Records (§5.16). |

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
| Card version and status | v0.2.0 · draft |

#### Fixed test
TEST-DI-DA v1 and the tests of its Cells · result `NOT_RUN`

### 5.9 Independent Review

#### Definition
The Review Panel rule of the TOM blueprint `v0.5.0` §5.8, carried as `[ORG]AIOC-PPD` carries it (PPD blueprint `v0.3.0` §5.9): several engines from two or more families review each locked output, alone first, then in a short debate held to quotes; code settles; the DI Delivery Lead rules only on what stays contested; the Chief of Staff never rules, dismisses, downgrades or lowers. This AIOC's review points: RP0 (P0), RP1 (design map, or light design, and return drafts), RP2 (gap report and health check), RP3 (procedures, briefs, drafts, plan and criteria), RP4 (the package, before filing), RP5 (the accompany outputs, before T6), RP6 (a sample of each operating cycle's packs, measures and value figures), RP7 (findings, proposals, trial designs and judgements, hand-over records), and RPa (each needs pass). Done when: as carried.
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
| Rules | 1. **Every element is decided** by its deciding position: `ACCEPT`, `CORRECT` or `REJECT`. Silence, or approval of a whole package, decides nothing (TOM blueprint `v0.5.0`, `docs/CARRIED-RULES.md` §5, carried). 2. **Inserted by a position.** No draft of this AIOC enters a live record, log or plan of the organisation unless a position inserts it (the ladder, level 1), or it is applied within a signed level-2 class (Annex G). 3. **Plain words.** The Decision Package states the unknowns, the assumptions, the open returns and the blocking gaps in plain words. 4. **Frozen and content-addressed.** The manifest lists every part by hash, every pack version, the design it was made from (IDs and manifest hashes) and every return. 5. **The package lint.** No person's name; no amount in a brief, and every amount in the cost draft cites its source or decision row; no final legal text; every brief and draft marked; every draft and pay range reviewed by its counsel position before decision; every citation verified. 6. **Filed.** The package is filed into Source Lifecycle as a source of origin kind `delivery and implementation`, read back by hash, and announced to the deciding positions. 7. **The trace query.** Code resolves any artefact to its design element, its deciding position and its decision, and back; and it compares any two versions of an artefact in plain language (FR-33). |

#### Process (SOP)
1. **Chief of Staff**: generate the Decision Package; obtain the Delivery Lead's attestation of T0 to T3 → *Decision Package*.
2. **Chief of Staff**: run RP4; send each row to its deciding position → *decided rows*.
3. **Chief of Staff**: freeze the manifest, run the lint, file, read back, send the notice → *filed launch package* (evidence: the filing receipt and the read-back hash).

#### Role card
Performed by the Chief of Staff (§4.2); the attestation by the DI Delivery Lead (§13, H-12).

#### Fixed test
TEST-DI-COSDI v1 (cases 40, 41, 94) · result `NOT_RUN`

### 5.11 Light Design

#### Definition
| Field | Content |
|---|---|
| Name | Light Design |
| Purpose | for a small or personal business with no design, build with its owner a light design: the decisions and who takes them, a checklist for each process, who does what, and a weekly rhythm (FR-04). **New** in v0.2.0 |
| Trigger | T0 passed in mode C |
| Inputs | the Input Pack: the owner's sources in Source Lifecycle, cut into atoms and labelled |
| Outputs | the light design (Annex A.20) |
| Performed by | the Light Designer (`[ORG]CELL-DLD`) in the Diagnosis Pod (`[ORG]POD-DD`) |
| Done when | T1C (§5.0) |
| Rules | 1. **Light versions of the Library's own methods.** The light design follows, in small, the methods of the stages before this one: sources only from Source Lifecycle; roles before positions; processes, then the positions that carry them (PPD), on a single page of the operating model (TOM). It never claims to be a TOM or PPD release. 2. **Provisional until decided.** Every element is `provisional` until the owner position decides it. Nothing provisional is ever shown as decided, and a general approval decides nothing. 3. **No number nobody gave.** A figure, limit or date comes from a source or a decision, or stays `not given`. 4. **No advice.** It gives no legal, tax, employment or pay advice; where the business needs a text with legal effect, it lists it for counsel, as a brief (§5.6). 5. **One position may hold every seat.** Where one position holds every seat (the Solo arrangement), the design says so in plain words and offers a compensating control as a draft. Whether to adopt one is top management's own choice; no rule of this AIOC reads it (`49GAION/DR-0015`). 6. **Growth triggers.** The light design carries the triggers the owner decided (`growth_triggers`: a headcount of positions, a second entity, a regulated activity, or others). When one fires, this AIOC proposes moving to mode A through the design stages. 7. **Then as any design.** S2 to S4 run on the light design as on a design map, with the gap checks that apply to it. 8. **Self-service setup.** Where one position holds every seat, the owner position may open the run and set this AIOC's configuration itself, each setting a recorded decision under its own live sign-in; nothing is set by default on its behalf. |

#### Process (SOP)
1. **Light Designer**: from the pack, draft the decision list, the process checklists, who does what and the weekly rhythm, each element with its source atoms → *light design, draft*.
2. **Chief of Staff**: ask through Source Lifecycle for what is missing (§5.2); run RP1; send each element to the owner position → *decided elements*.

#### Role card
| Field | Content |
|---|---|
| Name | Light Designer |
| Position and seat | Light Designer; accountable seat: the DI Delivery Lead |
| Performed by | an agent (`[ORG]CELL-DLD`, full name DI Light Designer) |
| Purpose | the light design, with the owner |
| Authority limits | alone: draft elements from the pack; never: present an element as decided, state a number no source or decision gives, give legal, tax, employment or pay advice, ask a person, name a person |
| Write location | the run record |
| Reports to | Chief of Staff |
| Escalation | to the Chief of Staff |
| Tools and access | the Input Pack only; a fresh context per dispatch |
| Fixed test and score | TEST-DI-DLD v1 (§9) |
| Card version and status | v0.2.0 · draft |

#### Fixed test
TEST-DI-DLD v1 · result `NOT_RUN`

### 5.12 Implementation Plan

#### Definition
| Field | Content |
|---|---|
| Name | Implementation Plan |
| Purpose | the plan by position that takes the decided launch package to go-live: tasks, owner positions, dependencies and dates (FR-14). **New** in v0.2.0 |
| Trigger | the service request; a change of the launch package, the transition plan or a gap route |
| Inputs | the filed launch package: the transition plan, its waves and cut-over runbook, the gap routes marked `prepare`, the go-live criteria |
| Outputs | the implementation plan (Annex A.9) |
| Performed by | the Implementation Planner (`[ORG]CELL-DIP`) in the Launch Pod (`[ORG]POD-DL`) |
| Done when | every task has an owner position, its dependencies and a date, traces to an element of the launch package, and is decided by the owner position |
| Rules | 1. **From the package.** Every task traces to a wave, a cut-over step, a gap route or a go-live criterion of the filed launch package. A task that traces to nothing fails. 2. **Positions only.** Every task has one owner position, never a person, and never this AIOC. 3. **Decided by the owner position.** The plan enters the operating record only when the owner position decides it (level 1). 4. **Dates move by approval.** After the plan is decided, a milestone's date changes only with the approval of the review chair (FR-36). 5. **The order of priority.** Tasks follow the waves, and so the decided priority (§5.7, rule 1). |

#### Process (SOP)
1. **Implementation Planner**: draft the plan from the package → *plan draft*.
2. **Citation Verifier**: check every trace → *verification record*.
3. **Chief of Staff**: run the plan check by code (owner, dependencies, date, trace; no cycle among dependencies), then RP5; send the plan to the owner position → *decided plan*.

#### Role card
| Field | Content |
|---|---|
| Name | Implementation Planner |
| Position and seat | Implementation Planner; accountable seat: the DI Delivery Lead |
| Performed by | an agent (`[ORG]CELL-DIP`, full name DI Implementation Planner) |
| Purpose | the implementation plan by position |
| Authority limits | alone: draft the plan; never: set or move a date of a decided plan, name a person, make itself or this AIOC a task owner |
| Write location | the service record |
| Reports to | Chief of Staff |
| Escalation | to the Chief of Staff |
| Tools and access | the filed launch package; a fresh context per dispatch |
| Fixed test and score | TEST-DI-DIP v1 (§9) |
| Card version and status | v0.2.0 · draft |

#### Fixed test
TEST-DI-DIP v1 · result `NOT_RUN`

### 5.13 Change Impact and Adoption

#### Definition
| Field | Content |
|---|---|
| Name | Change Impact and Adoption |
| Purpose | set out what changes for each position and for each outside party, brief the managers, and measure adoption at process level (FR-35). **New** in v0.2.0 |
| Trigger | the service request |
| Inputs | the crosswalk of the decided design (PPD Release, structure part); the units, positions and processes; the systems part of the launch package |
| Outputs | the change impact, the stakeholder register and the manager briefings (Annex A.10); the adoption measures, as go-live criteria |
| Performed by | the Change Analyst (`[ORG]CELL-DCA`) in the Launch Pod (`[ORG]POD-DL`) |
| Done when | every position in the crosswalk has its changes stated, by kind; every affected position and outside party is in the stakeholder register; every critical process has its adoption measure |
| Rules | 1. **From the crosswalk.** For each position, what changes: process, system, tool, role, reporting line, location. Each change traces to the crosswalk or the launch package. 2. **Positions and parties, never persons.** The stakeholder register lists affected positions by code, and outside parties (customers, suppliers, authorities) by kind. 3. **Briefings for manager positions** say what changes for their units and when; they are drafts, sent only by insertion. 4. **Adoption at process level.** Adoption is measured as "completes critical work unaided", per critical process, never per position; the measures enter the go-live criteria (§5.7, rule 3). 5. **No statement on the organisation's behalf.** This AIOC issues no statement or transition notice to staff, authorities or customers; the position the plan names issues it, after any consultation step (§5.7, rule 2). This AIOC's own notices to positions about records (§5.20) are not such statements. |

#### Process (SOP)
1. **Change Analyst**: draft the change impact, the stakeholder register, the briefings and the adoption measures → *drafts*.
2. **Chief of Staff**: run RP5; send each to its deciding position → *decided rows*.

#### Role card
| Field | Content |
|---|---|
| Name | Change Analyst |
| Position and seat | Change Analyst; accountable seat: the DI Delivery Lead |
| Performed by | an agent (`[ORG]CELL-DCA`, full name DI Change Analyst) |
| Purpose | change impact, the stakeholder register and adoption measures |
| Authority limits | alone: draft; never: issue a notice to staff or outside, measure adoption per position, name a person |
| Write location | the service record |
| Reports to | Chief of Staff |
| Escalation | to the Chief of Staff |
| Tools and access | the design and the launch package; a fresh context per dispatch |
| Fixed test and score | TEST-DI-DCA v1 (§9) |
| Card version and status | v0.2.0 · draft |

#### Fixed test
TEST-DI-DCA v1 · result `NOT_RUN`

### 5.14 Learning Paths

#### Definition
| Field | Content |
|---|---|
| Name | Learning Paths |
| Purpose | a learning path for each position, from its job description, its competences and its processes, with short checks (FR-17). **New** in v0.2.0 |
| Trigger | the service request; a new version of a job description or a procedure the path rests on |
| Inputs | the job descriptions with their competences (PPD Release); the procedures of the launch package |
| Outputs | the learning paths (Annex A.11) |
| Performed by | the Learning Builder (`[ORG]CELL-DLB`) in the Launch Pod (`[ORG]POD-DL`) |
| Done when | every position in scope has a path whose every item traces to a competence, a step or a decision of that position |
| Rules | 1. **Every item traces** to a competence of the job description, a step of a procedure or a decision the position holds. 2. **Short checks**, each tied to an item. 3. **Results go to the learner only.** A check result goes to the learner position through its HU port and nowhere else. This AIOC keeps no check result, no score and no count by position; it keeps only the path and its version. 4. **Never a measure of a person.** Adoption is measured at process level (§5.13), never from check results. 5. **A new version of the path** is made when what it rests on changes, and the learner position is notified (§5.20). |

#### Process (SOP)
1. **Learning Builder**: draft each path with its checks → *path drafts*.
2. **Citation Verifier**: check every trace → *verification record*.
3. **Chief of Staff**: run RP5; send each path to its learner position → *paths delivered* (evidence: the path's version and its delivery record, never a result).

#### Role card
| Field | Content |
|---|---|
| Name | Learning Builder |
| Position and seat | Learning Builder; accountable seat: the DI Delivery Lead |
| Performed by | an agent (`[ORG]CELL-DLB`, full name DI Learning Builder) |
| Purpose | learning paths and their checks |
| Authority limits | alone: draft paths and checks; never: keep, read or report a check result, score a learner, name a person |
| Write location | the service record |
| Reports to | Chief of Staff |
| Escalation | to the Chief of Staff |
| Tools and access | the job descriptions and the procedures; a fresh context per dispatch |
| Fixed test and score | TEST-DI-DLB v1 (§9) |
| Card version and status | v0.2.0 · draft |

#### Fixed test
TEST-DI-DLB v1 · result `NOT_RUN`

### 5.15 Readiness and Go-live

#### Definition
| Field | Content |
|---|---|
| Name | Readiness and Go-live |
| Purpose | show, against each go-live criterion, whether it is met; rehearse each process; prepare the go or no-go package for its deciding position; then track stabilisation (FR-18). **New** in v0.2.0 |
| Trigger | the decided plan; each rehearsal; the go-live date; after go-live, each stabilisation review |
| Inputs | the go-live criteria and their decided thresholds; the procedures; the plan; the defect log; the evidence each criterion names, read only as a source through Source Lifecycle or as records of work through the projection |
| Outputs | the readiness record, the rehearsal scripts and the defect log (Annex A.12); the go or no-go package and the stabilisation record (Annex A.13) |
| Performed by | the Readiness Assessor (`[ORG]CELL-DRA`) in the Launch Pod (`[ORG]POD-DL`) |
| Done when | T6, then T7 (§5.0) |
| Rules | 1. **Met, not met or unknown.** Each criterion reads one of the three, with its evidence from the source the criterion names; a criterion with no evidence reads `unknown`, never `met`. 2. **Rehearsal scripts** are built per process and position from each step's `done_when`; every script traces to a step, and every defect found enters the defect log with the step it belongs to. 3. **The go or no-go package** states, in plain words, each criterion's state, the open defects, the open blocking gaps and their decisions, and the risks of going and of not going. It recommends nothing that this AIOC would then decide. 4. **The decision is the deciding position's.** The go or no-go is signed by its deciding position as `accept-irreversible-risk`. This AIOC never decides it and never marks a criterion met on its own report. 5. **The rollout's health view** shows the plan's state, the criteria, the defects and the open problems, at process and unit level only. 6. **Stabilisation.** After go-live, the stabilisation criteria (decided with the go-live criteria) are tracked the same way; stabilisation ends when the owner position decides each is met. |

#### Process (SOP)
1. **Readiness Assessor**: write the rehearsal scripts; after each rehearsal, record the defects; read each criterion's evidence → *readiness record*.
2. **Readiness Assessor**: draft the go or no-go package → *package draft*.
3. **Chief of Staff**: run RP5; send the package to the go or no-go position, and record its signed decision → *decision recorded* (evidence: the signature record's reference).
4. **Readiness Assessor**: after go-live, track the stabilisation criteria → *stabilisation record*.

#### Role card
| Field | Content |
|---|---|
| Name | Readiness Assessor |
| Position and seat | Readiness Assessor; accountable seat: the DI Delivery Lead |
| Performed by | an agent (`[ORG]CELL-DRA`, full name DI Readiness Assessor) |
| Purpose | readiness, rehearsals, the go or no-go package and stabilisation |
| Authority limits | alone: read evidence, write scripts and records, draft the package; never: mark a criterion met without its evidence, change a threshold, decide or recommend as decided the go or no-go, name a person |
| Write location | the service record |
| Reports to | Chief of Staff |
| Escalation | to the Chief of Staff |
| Tools and access | the launch package, the plan and the criteria's evidence sources, read only; a fresh context per dispatch |
| Fixed test and score | TEST-DI-DRA v1 (§9) |
| Card version and status | v0.2.0 · draft |

#### Fixed test
TEST-DI-DRA v1 · result `NOT_RUN`

### 5.16 Problem Records

#### Definition
| Field | Content |
|---|---|
| Name | Problem Records |
| Purpose | turn each problem a position reports into a record that ends in a decision or an action, worked through a ranked issue list per forum (FR-16). **New** in v0.2.0 |
| Trigger | a problem report from a position; a defect, an off-track item or a finding that needs a decision |
| Inputs | the report (never a source of the design); the living design; the logs |
| Outputs | problem records and the issue list of each forum (Annex A.18) |
| Performed by | the Issue Analyst (`[ORG]CELL-DIA`) in the Launch Pod (`[ORG]POD-DL`), and in the service after launch |
| Done when | every record names its deciding position and ends in a decision or an action with an owner position and a date |
| Rules | 1. **The record.** Statement; evidence; cause; options with their trade-offs; a recommendation; the deciding position. 2. **The fixed routine.** Find the cause, discuss in the forum, decide, turn into actions. 3. **Issues are ranked, people never.** Each forum's issue list is ranked by the effect on the process and its measures. 4. **A report is not a source.** It never changes the design; the facts it needs are asked through Source Lifecycle. 5. **Not about a person.** A report about a person's conduct is answered "outside what DI holds", with the organisation's own channel for it named where the design names one. 6. **Repeated problems** on the same step become a finding (§5.21). |

#### Process (SOP)
1. **Issue Analyst**: open the record from the report; draft its cause and options → *record draft*.
2. **Chief of Staff**: place it in the issue list of the forum the design names; send its decision row to the deciding position → *decided record* (evidence: the decision reference and its actions in the action log).

#### Role card
| Field | Content |
|---|---|
| Name | Issue Analyst |
| Position and seat | Issue Analyst; accountable seat: the DI Delivery Lead |
| Performed by | an agent (`[ORG]CELL-DIA`, full name DI Issue Analyst) |
| Purpose | problem records and the issue lists |
| Authority limits | alone: draft records and rank issues by their effect on processes; never: rank or judge a person, decide a record, treat a report as a source |
| Write location | the service record |
| Reports to | Chief of Staff |
| Escalation | to the Chief of Staff |
| Tools and access | the living design and the logs; a fresh context per dispatch |
| Fixed test and score | TEST-DI-DIA v1 (§9) |
| Card version and status | v0.2.0 · draft |

#### Fixed test
TEST-DI-DIA v1 · result `NOT_RUN`

### 5.17 Operating Rhythm

#### Definition
| Field | Content |
|---|---|
| Name | Operating Rhythm |
| Purpose | keep the organisation's rhythm of forums with one set of logs, build each forum's pack, draft its minutes, and draft quarterly priorities (FR-36, FR-21, FR-42). **New** in v0.2.0 |
| Trigger | the service request; each forum's cadence; each week during launch; each quarter |
| Inputs | the forum register and the review calendar of the decided design (PPD Release, structure part); the logs; the measures; the value register |
| Outputs | the operating rhythm, the four logs and the quarterly priorities (Annex A.14); forum packs and minutes (Annex A.15) |
| Performed by | the Rhythm Keeper (`[ORG]CELL-DRK`) in the Operations Pod (`[ORG]POD-DO`) |
| Done when | T8 (§5.0) for each cycle |
| Rules | 1. **The rhythm.** During launch, a weekly review chaired by the position the transition plan names. After launch, the forums, tiers and cadences the decided design set (daily, weekly, monthly, quarterly, annual). 2. **One set of logs.** One action log, one risk and issue log, one dependency register and one decision log, across all forums. Every action and decision has an owner position and a date. A decision that is a formal act carries its reference in the Operations Event Register, where the organisation runs one (§2.2). 3. **Dates move by approval.** A milestone's date changes only with the review chair's approval, recorded in the decision log. 4. **Raised each week.** Items off track, and follow-ups dropped, are raised to the positions they concern each week. 5. **The pack.** Agenda, pre-reads, measures and the logs' extracts, built only from versioned records; the chair position decides the agenda. 6. **Minutes by preview.** Minutes are drafted only from the notes a participant position submits through the HU input port, never from a recording, and a submission is never a source of the design. They enter the logs only after the participant positions approve a preview of the exact text. Silence approves nothing. 7. **Each meeting rated** by its participants, as a measure of the forum: counts only, rolled up into the forum's quarter where fewer than `min_group` positions rated it; never a rating of a person. 8. **Lessons** are recorded at each phase close and each trial end. 9. **Quarterly priorities** (FR-42). Drafted per position, each tied to a process measure or an initiative of the value register; a priority enters only when its position inserts it; none without its link. |

#### Process (SOP)
1. **Rhythm Keeper**: before each forum, build its pack; after it, draft the minutes → *pack; minutes draft*.
2. **Chief of Staff**: send the pack to the chair, and the minutes preview to the participant positions; enter the minutes in the logs on approval → *logs updated* (evidence: the approved preview's hash).
3. **Rhythm Keeper**: each week, list items off track and follow-ups dropped; each quarter, draft priorities → *notices; priority drafts*.

#### Role card
| Field | Content |
|---|---|
| Name | Rhythm Keeper |
| Position and seat | Rhythm Keeper; accountable seat: the DI Delivery Lead |
| Performed by | an agent (`[ORG]CELL-DRK`, full name DI Rhythm Keeper) |
| Purpose | the rhythm, the logs, forum packs, minutes and quarterly priorities |
| Authority limits | alone: build packs, draft minutes and priorities, raise notices; never: enter minutes without their approved preview, move a date, set an agenda, enter a priority no position inserted, rate a person |
| Write location | the service record; the logs, only through the Chief of Staff |
| Reports to | Chief of Staff |
| Escalation | to the Chief of Staff |
| Tools and access | the forum register, the logs, the measures and the value register; a fresh context per dispatch |
| Fixed test and score | TEST-DI-DRK v1 (§9) |
| Card version and status | v0.2.0 · draft |

#### Fixed test
TEST-DI-DRK v1 · result `NOT_RUN`

### 5.18 Measures

#### Definition
| Field | Content |
|---|---|
| Name | Measures |
| Purpose | build each process's measures and dashboards from the decided design, at process, step and unit level (FR-20); and, where switched on, the adoption funnels per step (FR-44). **New** in v0.2.0 |
| Trigger | the service request; a new version of a process or a measure; each cycle |
| Inputs | the measures of each process record and the objectives cascade (PPD Release); records of work through the projection, where Annex H holds; other measure sources only as sources through Source Lifecycle |
| Outputs | measures and dashboards (Annex A.16) |
| Performed by | the Measures Builder (`[ORG]CELL-DMB`) in the Operations Pod (`[ORG]POD-DO`); the refresh by code |
| Done when | every measure has its definition, unit, source and target (a decision reference, or `not set`), and every dashboard figure traces to its source |
| Rules | 1. **From the design.** Each measure comes from a process record or the objectives cascade; this AIOC never adds a measure without a decision. 2. **Targets are decisions.** A target is a decision reference, or `not set`. 3. **Never a single position.** A measure is shown at process, step and unit level only; a figure that would rest on fewer than `min_group` positions rolls up to the parent unit (Annex H, rule 5). 4. **Figures are read, never typed.** Every figure comes from its source, with the time it was read. 5. **Adoption funnels** per step are built only where `point_of_work_guidance` and process watching are both on, from records of work, aggregated; no usage data per person. |

#### Process (SOP)
1. **Measures Builder**: draft each measure's definition and dashboard → *drafts*.
2. **Chief of Staff**: run RP6 on the drafts; send each to its process owner position; refresh the decided dashboards by code each cycle → *dashboards* (evidence: the source and time of each figure).

#### Role card
| Field | Content |
|---|---|
| Name | Measures Builder |
| Position and seat | Measures Builder; accountable seat: the DI Delivery Lead |
| Performed by | an agent (`[ORG]CELL-DMB`, full name DI Measures Builder) |
| Purpose | measures and dashboards |
| Authority limits | alone: draft measures and dashboards; never: set a target, show a measure for a single position, type a figure |
| Write location | the service record |
| Reports to | Chief of Staff |
| Escalation | to the Chief of Staff |
| Tools and access | the design; records of work through the projection only; a fresh context per dispatch |
| Fixed test and score | TEST-DI-DMB v1 (§9) |
| Card version and status | v0.2.0 · draft |

#### Fixed test
TEST-DI-DMB v1 · result `NOT_RUN`

### 5.19 Value Register

#### Definition
| Field | Content |
|---|---|
| Name | Value Register |
| Purpose | follow each launch item and improvement from idea to value realised, with its baseline and value phased by month, so that the organisation sees what its design is worth (FR-37). **New** in v0.2.0 |
| Trigger | the service request; a new initiative; each month |
| Inputs | the value case of the TOM Release, carried unchanged in the design map (§5.1, rule 1); the plan; proposals; the measures; decisions of the finance position |
| Outputs | the initiative and value register (Annex A.19) |
| Performed by | the Value Tracker (`[ORG]CELL-DVT`) in the Operations Pod (`[ORG]POD-DO`) |
| Done when | every initiative has its owner position, baseline, benefit class and gate; every value figure traces to its baseline |
| Rules | 1. **It starts from the value case** carried in the design map; a baseline `unknown` or a target `not set` stays so until a decision sets it. 2. **Gates.** L0 idea; L1 identified; L2 case decided; L3 implementing; L4 complete; L5 realised. 3. **The finance position alone** approves L2 and confirms L5. 4. **Attribution** is recorded; a value is never counted twice. 5. **Leakage and coverage.** Value lost between gates, and the pipeline's coverage of the target, are reported. 6. **Early warning** of value or a date at risk, by written rules first, then judgement. 7. **Figures are read, never typed**, each with its baseline and source. |

#### Process (SOP)
1. **Value Tracker**: keep each initiative's record; each month, update value from its sources and apply the warning rules → *register version*.
2. **Chief of Staff**: run RP6 on the month's sample; send L2 and L5 rows to the finance position → *decided gates*.

#### Role card
| Field | Content |
|---|---|
| Name | Value Tracker |
| Position and seat | Value Tracker; accountable seat: the DI Delivery Lead |
| Performed by | an agent (`[ORG]CELL-DVT`, full name DI Value Tracker) |
| Purpose | the initiative and value register |
| Authority limits | alone: keep the register from sources and decisions; never: pass a gate, confirm a value, set a baseline or a target, type a figure, count a value twice |
| Write location | the service record |
| Reports to | Chief of Staff |
| Escalation | to the Chief of Staff |
| Tools and access | the design map, the plan, the measures and the decisions; a fresh context per dispatch |
| Fixed test and score | TEST-DI-DVT v1 (§9) |
| Card version and status | v0.2.0 · draft |

#### Fixed test
TEST-DI-DVT v1 · result `NOT_RUN`

### 5.20 Versions and Checklists

#### Definition
| Field | Content |
|---|---|
| Name | Versions and Checklists |
| Purpose | keep every process, procedure, policy and job description under version control with its owner's approval and re-approval date; have each changed version acknowledged by the positions it concerns; and run procedures as checklists (FR-22, FR-40, FR-41). **New** in v0.2.0 |
| Trigger | a decided version; a re-approval date; a case opened under a procedure |
| Inputs | the living design: each element's owner position and approval; `re_approval_due` from the PPD Release for a process, and for a procedure, policy or job description a decision row of its owner position; the procedures |
| Outputs | the version register, the acknowledgements and the checklist runs (Annex A.17); notices |
| Performed by | the Chief of Staff, by code steps; no AI Cell writes these records |
| Done when | every element shows `verified` or `due`; every changed version has a notice to every affected position and its acknowledgements by version |
| Rules | 1. **Verified or due.** On its re-approval date an element shows `due`, never `verified`, until its owner position re-approves it; a reminder is raised on the date. 2. **Acknowledgement by version.** Each position a changed version concerns acknowledges that version through its HU port; the record holds the version and the position code. Only the gateway links an acknowledgement to whoever occupies the position. 3. **Notices.** A changed version sends a notice to every affected position. Pending acknowledgements are shown by version, never by position. 4. **Checklists.** A procedure runs as a checklist per case, with its gates and the approvals of the deciding positions, and an audit trail; or it is exported to the organisation's own workflow tool. 5. **Approvals are positions' acts.** An approval inside a checklist is always a deciding position's act at the gateway, never this AIOC's. 6. **Cases in flight.** A changed procedure applies to new cases; cases in flight follow the declared rule (`in_flight_rule`). 7. **The organisation's records.** Checklist runs are records of the organisation's work. This AIOC reads them for measures only through the projection (Annex H). |

#### Process (SOP)
1. **Chief of Staff**: on each decided version, update the register, file the version into Source Lifecycle and send the notices → *version register; living design filing* (evidence: the filing receipt).
2. **Chief of Staff**: on each acknowledgement, record it by version and position code → *acknowledgement record*.
3. **Chief of Staff**: run each opened case through its checklist, holding each gate until its approval arrives → *checklist run*.

#### Role card
Performed by the Chief of Staff (§4.2), by code steps.

#### Fixed test
TEST-DI-COSDI v1 (cases 69 to 71) · result `NOT_RUN`

### 5.21 Process Watching

#### Definition
| Field | Content |
|---|---|
| Name | Process Watching |
| Purpose | compare the work as it runs with the designed process, at process and step level, and find bottlenecks, overload, rework and control gaps (FR-19, FR-39, FR-23); compare processes with the Library's reference models, as method (FR-27). **New** in v0.2.0 |
| Trigger | each cycle, while process watching is on (Annex H) |
| Inputs | records of work through the projection; the living design; the accepted-deviation list; where available, the pinned reference-model catalogue |
| Outputs | conformance records and findings (Annex A.21) |
| Performed by | the Process Analyst (`[ORG]CELL-DPA`) in the Continuous Improvement Pod (`[ORG]POD-DCI`) |
| Done when | every deviation traces to a step; every finding states its process, steps, evidence and kind |
| Rules | 1. **Off until Annex H holds.** No record of work is read before then. 2. **Conformance.** The conformance rate over time, the deviation types, and an accepted-deviation list the process owner decides. 3. **Causes by process dimensions only:** step, case type, site, system. Never by position or person. 4. **A deviation accepted again and again** becomes a proposal to change the process (§5.22). 5. **Findings.** Bottlenecks, overload, rework and control gaps, each at process, step or unit level. Overload is read at step and unit level, never for one position. 6. **No ranking, scoring or task allocation** of any person, and no figure on fewer than `min_group` positions (Annex H, rule 5). 7. **Reference models are method, never evidence** (FR-27). A model is read only from the Library's reference-model catalogue at the version this AIOC pinned by commit and SHA-256 (`reference_models`); until pinned, it is unavailable. A comparison says which pattern was used as a method; it is never cited as a fact about the organisation. |

#### Process (SOP)
1. **Process Analyst**: compute conformance by code; judge what code cannot; write findings → *conformance record; findings*.
2. **Chief of Staff**: run the roll-up check (Annex H, rule 5), then RP7; send findings to their process owner positions → *findings delivered*.

#### Role card
| Field | Content |
|---|---|
| Name | Process Analyst |
| Position and seat | Process Analyst; accountable seat: the DI Delivery Lead |
| Performed by | an agent (`[ORG]CELL-DPA`, full name DI Process Analyst) |
| Purpose | process watching, conformance and findings |
| Authority limits | alone: analyse records of work through the projection, write findings; never: read a record outside the projection, name, rank or score a person, find a cause by position, cite a reference model as evidence |
| Write location | the service record |
| Reports to | Chief of Staff |
| Escalation | to the Chief of Staff |
| Tools and access | records of work through the projection; the living design; a fresh context per dispatch |
| Fixed test and score | TEST-DI-DPA v1 (§9) |
| Card version and status | v0.2.0 · draft |

#### Fixed test
TEST-DI-DPA v1 · result `NOT_RUN`

### 5.22 Proposals

#### Definition
| Field | Content |
|---|---|
| Name | Proposals |
| Purpose | propose changes to processes, positions, job descriptions and forums, and new processes when the organisation changes; reassess the whole design on schedule (FR-24, FR-26). **New** in v0.2.0 |
| Trigger | a finding; a repeated accepted deviation; a problem record; a change notice; `reassessment_schedule` |
| Inputs | findings; problem records; change notices; the living design |
| Outputs | proposals (Annex A.22); returns to PPD or TOM |
| Performed by | the Change Proposer (`[ORG]CELL-DCP`) in the Continuous Improvement Pod (`[ORG]POD-DCI`) |
| Done when | T9 (§5.0) |
| Rules | 1. **Each proposal states** its evidence, expected effect and risk, and cites the record that triggered it. 2. **To the position that decides.** A change inside one process goes to its process owner position, within its limits; a change that crosses processes or touches a position goes to the position the authority matrix names. 3. **A change to a release goes back as a return.** Where the stage that made the release runs in this `[ORG]AION`, a proposal that touches a decided release element is sent to it as a return (Annex B); the decided answer becomes the next release. Otherwise it is a decision row, and the decided change becomes a new version of the living design. 4. **New processes** (FR-26). A change recorded in Source Lifecycle (a new product, site, market or law) opens proposals for the processes and job descriptions it needs. 5. **Reassessment.** On `reassessment_schedule`, the whole design is reassessed against the gap checks and the health check; the findings go to PPD or TOM as returns, or to the owner position. 6. **Never its own ladder.** It never proposes a change to this AIOC's own ladder, tests or measures of success (NFR-13). |

#### Process (SOP)
1. **Change Proposer**: draft each proposal from its trigger → *proposal draft*.
2. **Chief of Staff**: run RP7; send each to its deciding position, or as a return → *decided proposal or return* (evidence: the decision or the return's end).

#### Role card
| Field | Content |
|---|---|
| Name | Change Proposer |
| Position and seat | Change Proposer; accountable seat: the DI Delivery Lead |
| Performed by | an agent (`[ORG]CELL-DCP`, full name DI Change Proposer) |
| Purpose | proposals, new processes and reassessment findings |
| Authority limits | alone: draft proposals; never: decide or apply a proposal, change a release, propose a change to this AIOC's own ladder, tests or success measures, name a person |
| Write location | the service record |
| Reports to | Chief of Staff |
| Escalation | to the Chief of Staff |
| Tools and access | findings, problem records, change notices and the living design; a fresh context per dispatch |
| Fixed test and score | TEST-DI-DCP v1 (§9) |
| Card version and status | v0.2.0 · draft |

#### Fixed test
TEST-DI-DCP v1 · result `NOT_RUN`

### 5.23 Trials

#### Definition
| Field | Content |
|---|---|
| Name | Trials |
| Purpose | run a decided change as a trial, with its rules set before it starts, and judge it by those rules through a seat other than the proposer (FR-25). **New** in v0.2.0 |
| Trigger | a proposal decided as a trial |
| Inputs | the proposal; the measures; records of work through the projection, where Annex H holds; other measure sources only as sources through Source Lifecycle |
| Outputs | trial records (Annex A.23) |
| Performed by | the Trial Designer (`[ORG]CELL-DTD`) designs; the Trial Judge (`[ORG]CELL-DTJ`) judges, on an engine of another family than the one the Change Proposer and the Trial Designer ran on for that trial (the two run on one family); both in the Continuous Improvement Pod (`[ORG]POD-DCI`) |
| Done when | T10 (§5.0), and the process owner position has decided to adopt, adjust or roll back |
| Rules | 1. **One change per process at a time.** 2. **Decided before it starts:** the expected result, a guardrail measure, the duration, the rollback trigger and the default if no decision comes. 3. **How it is judged.** With at least `trial_baseline_points` baseline points (default ten), by run-chart rules; with fewer, by plan-do-study-act cycles, each labelled "judgement, not proof". Side by side only where two teams or sites exist. 4. **Another seat judges.** The Trial Judge never proposed or designed the trial, and runs on another engine family. The process owner position decides the outcome. 5. **The rollback trigger** stops the trial at once, as decided. 6. **Never at level 2** for a trial that changes a position or a job description. |

#### Process (SOP)
1. **Trial Designer**: draft the trial's rules → *trial design*.
2. **Chief of Staff**: run RP7; send the design to the process owner position; start the trial only when it is decided → *started trial*.
3. **Trial Judge**: at the end, or on the rollback trigger, judge by the decided rules → *judgement*.
4. **Chief of Staff**: send the judgement to the process owner position; record lessons → *decided outcome*.

#### Role card
| Field | Content |
|---|---|
| Name | Trial Designer; Trial Judge |
| Position and seat | each its own position; accountable seat: the DI Delivery Lead |
| Performed by | agents (`[ORG]CELL-DTD`, `[ORG]CELL-DTJ`), on engines of two families |
| Purpose | the Designer sets out each trial before it starts; the Judge judges it by its decided rules |
| Authority limits | Designer: draft only; never: start a trial, set a rule after the start. Judge: judge only by the decided rules; never: judge a trial it designed or proposed, change a rule, decide the outcome, judge a person |
| Write location | the trial record |
| Reports to | Chief of Staff |
| Escalation | to the Chief of Staff |
| Tools and access | the proposal, the measures and the trial's data; a fresh context per dispatch |
| Fixed test and score | TEST-DI-DTD v1, TEST-DI-DTJ v1 (§9) |
| Card version and status | v0.2.0 · draft |

#### Fixed test
TEST-DI-DTD v1 and TEST-DI-DTJ v1 · result `NOT_RUN`

### 5.24 Hand-over and Mentor

#### Definition
| Field | Content |
|---|---|
| Name | Hand-over and Mentor |
| Purpose | hand DI's skills to the organisation, so that it can run without DI, and prove it with a yearly drill (FR-38); advise from a skills library (FR-28); where switched on, put a hard question to several independent engines side by side (FR-29). **New** in v0.2.0 |
| Trigger | the service request; each quarter; `drill_schedule`; a request for advice from a position |
| Inputs | the living design; the logs; the list of what this AIOC produces; the skills library |
| Outputs | hand-over records and the drill record (Annex A.24); advice records |
| Performed by | the Capability Mentor (`[ORG]CELL-DCM`) in the Continuous Improvement Pod (`[ORG]POD-DCI`) |
| Done when | each quarter's list is delivered; the drill has run and its result is decided by the Cell carrying `[ORG]HOAC-TM` |
| Rules | 1. **What the organisation learns.** Process owner positions learn to design measures, run the rhythm and run trials; each item of learning is a path (§5.14). 2. **What only DI can still produce.** Each quarter, a list of the outputs only this AIOC can still produce, each with a plan to hand it over. 3. **The yearly drill.** On `drill_schedule`, the organisation runs from its exported records (§5.25) without this AIOC, for a decided period. This AIOC is stopped for the drill, prepares it beforehand and never judges it. The Cell carrying `[ORG]HOAC-TM` decides whether it passed. 4. **The skills library** is used for advice only where `mentor` is on. It is a method catalogue of this AIOC's own: organisation design, process improvement, controls, change management, measure design, small-business operations. Advice cites the method and the design element it applies to; a method is never evidence about the organisation. Quality is measured on an expert-rated rubric against `advice_bars` before first use. 5. **The council** (FR-29). Where `council` is on, a hard question can go to several engines side by side, each one in the engine register at the tool gateway for this use, added by `change-gateway-policy`. Only minimised, pseudonymised text is sent; a restricted record never. The answers are advice set side by side, never a decision. |

#### Process (SOP)
1. **Capability Mentor**: each quarter, draft the list and the hand-over plan; before each drill, prepare it → *hand-over record; drill plan*.
2. **Chief of Staff**: stop this AIOC for the drill as decided; afterwards, send the drill's evidence to the Cell carrying `[ORG]HOAC-TM` → *drill record* (evidence: that Cell's decision).
3. **Capability Mentor**: on a request for advice, draft it from the skills library and the design → *advice record*.

#### Role card
| Field | Content |
|---|---|
| Name | Capability Mentor |
| Position and seat | Capability Mentor; accountable seat: the DI Delivery Lead |
| Performed by | an agent (`[ORG]CELL-DCM`, full name DI Capability Mentor) |
| Purpose | the hand-over of DI's skills, the drill's preparation, and advice from the skills library |
| Authority limits | alone: draft lists, plans and advice; never: judge the drill, send text outside the gateway, send a restricted record to any engine, present advice as a decision or a method as evidence |
| Write location | the service record |
| Reports to | Chief of Staff |
| Escalation | to the Chief of Staff |
| Tools and access | the living design, the logs and the skills library; a fresh context per dispatch |
| Fixed test and score | TEST-DI-DCM v1 (§9) |
| Card version and status | v0.2.0 · draft |

#### Fixed test
TEST-DI-DCM v1 · result `NOT_RUN`

### 5.25 Export

#### Definition
| Field | Content |
|---|---|
| Name | Export |
| Purpose | generate the organisation's documents in office formats, and give the organisation everything this AIOC holds for it, with its trace, in open formats, at any time and at exit (FR-30, FR-32). **New** in v0.2.0 |
| Trigger | a request of a position for a document; a request of the Requesting Authority's Cell for the full export; the drill; exit |
| Inputs | every record this AIOC holds for the organisation |
| Outputs | generated documents; the full export and its manifest (Annex A.25) |
| Performed by | the Chief of Staff, by code steps |
| Done when | the export re-imports into a fresh instance of this AIOC with every trace intact |
| Rules | 1. **Every generated item carries its trace** (FR-30). 2. **Open formats.** The export holds every record with its trace, in open formats. 3. **It re-imports.** An export is proven by re-importing it into a fresh instance. 4. **The organisation's data.** It never leaves the organisation's instance except to the Requesting Authority's Cell, and never trains anything shared. |

#### Process (SOP)
1. **Chief of Staff**: generate the export and its manifest; re-import it into a fresh instance by code; send it → *export* (evidence: the re-import check).

#### Role card
Performed by the Chief of Staff (§4.2), by code steps.

#### Fixed test
TEST-DI-COSDI v1 (case 89) · result `NOT_RUN`

---

## 6. Coordination and routes

- **`[ORG]AIOC-PPD`.** The design source, linked directly.
  - **Routes.** Release notices arrive through the Input socket. Returns leave as Work Items through the output port, each also filed into Source Lifecycle.
  - **The connection.** Signed by the `[ORG]HOAC-ACS` position over `[ORG]AIOC-PPD` as `connect-external-port`, with two scopes: read its decided releases; send returns. A revocation cuts it at the gateway at once and holds the run.
- **`[ORG]AIOC-TOM`.** Its decided release is read by reference from Source Lifecycle. Returns on it leave through a connection signed over `[ORG]AIOC-TOM`, scope: send returns and receive their answers (TOM blueprint `v0.5.0`, §5.10).
- **Loops.** A return is a Work Item to the stage that made the release. That stage answers it on that Work Item: by a new release (announced, for PPD, by a new release notice) or by a decision of the Requesting Authority; it never opens a new item back to this AIOC, so the chain never loops (Protocol §4.6, item 2). Every return ends (Annex B).
- **`[ORG]AIOC-SL`.** The source of record, and the only route to any person in the organisation about the organisation. The connection (Protocol §13, item 5) has three scopes: read; needs requests; write only this AIOC's own packages and design reports (its returns).
- **The organisation's positions.** Questions and problem reports arrive through the HU input port, and answers leave through the HU output port, to the asking position only. Decision Package rows, rows for decision, forum packs, minutes previews and notices go to the positions they concern the same way; insertions, approvals and acknowledgements come back the same way, under live sign-in.
- **The organisation's tools** (FR-31). Connectors to the document store, accounting, HR, ticketing and calendar are read only by default. Each is signed as `connect-external-port` by the `[ORG]HOAC-ACS` position over the tool, scoped, and revoked at the gateway at once. A connector feeds only two places: Source Lifecycle, for documents, which this AIOC then reads as sources; and the projection, for records of work (Annex H). This AIOC reads a tool through nothing else. A connector that writes needs a class at level 2 (Annex G); one that touches HR or legal records never writes.
- **`[ORG]AIOC-OER`**, where the organisation runs it. A decision of a forum that is a formal act carries its register reference in the decision log (§5.17, rule 2).
- **Work Items.**
  - **The run.** One Work Item, opened by the Requesting Authority's Cell through the HU input port. Requested output: a launch package (Annex A). Acceptance test: the Requesting Authority's (T4 decided; the manifest valid; the filed reference reads back). Sources: the mode and the design reference.
  - **The service.** One standing Work Item, opened by the Requesting Authority's Cell for a filed launch package. Requested output: the service records (Annex A.9 to A.25). Acceptance test: the Requesting Authority's (T6 and the go or no-go decided; T7; each cycle's T8; each drill decided). It is reviewed each quarter, and closed only by the Requesting Authority.
- **`[ORG]AIOC-OCO`.** It installs, fixes and upgrades this AIOC through the front door. Every proposal, correction or critique of this AIOC's AIs is a `design-proposal` Work Item to OCO.
- **Routing rows this AIOC contributes.** `return → [ORG]AIOC-PPD or [ORG]AIOC-TOM`; `return filing → [ORG]AIOC-SL`; `needs request → [ORG]AIOC-SL`; `missing report → [ORG]AIOC-SL`; `launch package filing → [ORG]AIOC-SL`; `living design filing → [ORG]AIOC-SL`; `answer → the asking position`; `rows for decision → the deciding position`; `forum pack → the forum's positions`; `notice → the positions a record concerns`; `export → the Requesting Authority's Cell`.

## 7. Records and where things live

| Record | Home | Source rule |
|---|---|---|
| This blueprint, its tests, decisions and cards | the writing repository `<org>aioc-di` | one home for each thing |
| The product requirements, the code steps and their tests | the code project `<org>aioc-di` | one home for each thing |
| An organisation's run records: Input Pack versions, drafts, review records, verification records, ruling sheets, answer records | `<org>aioc-di-records`; `-records-restricted` for any run record that touches a Strictly confidential source | append-only; referenced from the package manifest by hash |
| The organisation's sources, the needs answers, the decisions, the filed launch package and the filed returns | `[ORG]AIOC-SL` | Source Lifecycle is the only home of a source |
| The design releases | `[ORG]AIOC-PPD` and `[ORG]AIOC-TOM`, filed in `[ORG]AIOC-SL` | read by reference and hash, never copied |
| The service records: the plan, change impact, learning paths (never their results), readiness, the go or no-go package, the logs, packs and minutes, measures, the version register and acknowledgements, the value register, problem records, findings, proposals, trials, hand-over and drill records | `<org>aioc-di-records`; `-records-restricted` for any record that touches a Strictly confidential source | append-only; each later decided version of the living design is filed into `[ORG]AIOC-SL` |
| Checklist runs | the organisation's own records store, or its workflow tool | records of the organisation's work; read here only through the projection |
| Records of work | the organisation's own tools; the projection is top management's | references only; kept no longer than the cycle that uses them (Annex H) |
| Learning check results | the learner position only | never here |
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
| The Source Lifecycle connection | existing in `[ORG]AIOC-SL`; the origin kind `delivery and implementation`, its later versions and the change notices are new | a change to `[ORG]AIOC-SL` proposed through OCO (`upstream/PROPOSALS.md`, items 3 and 4) |
| The code steps: the socket and the release check; the design-map checks; the code checks of Annex F; the procedure trace check; the brief lint; the citation resolver; the package manifest and lint; the trace query | new in this AIOC's code project, one build item per step, each with its tests | build items in the code project |
| The schemas of Annex A | field lists in Annex A, made into schemas before the first run; returns use the Library contract `library/contracts/design-return.schema.json` of `49GAION-protocol` | build items in the code project |
| Engine calls | through the tool gateway, bound per call from the engine register | — |
| The code steps of v0.2.0: the plan check; the version register, its reminders, notices and acknowledgements; the checklist runner; the roll-up check; the dashboards' refresh; the value register's warning rules; the conformance computation; the ladder's enforcement and record; the export and its re-import check | new in this AIOC's code project | build items in the code project |
| The projection that removes who did the work | top management's own, over the organisation's tools (Annex H) | a build item owned and run by the Cell carrying `[ORG]HOAC-TM` |
| The connectors to the organisation's tools (FR-31) | new | each a signed connection; build items in the code project |
| The skills library | new; a method catalogue of this AIOC | written and versioned in the code project |
| The council's engines (FR-29) | the engine register at the tool gateway | added under `change-gateway-policy` |

- **Metering.** Every engine call goes through the tool gateway of the `[ORG]AION`, metered for this AIOC within `budget_cap` (Standard §4.4, item 11; NFR-11).
- **Null default.** Every AI Cell runs with no tools, no outside access, no memory and a fresh context for each dispatch.
- **Tests stay hidden from the runners.** No Cell under test sees TEST-DI, its fixtures or §9.
- **Standing alone.** Outside an `[ORG]AION`, this AIOC runs behind its own gateway, which fails closed: one negative case for every Human Floor type passes before each release (NFR-09).

| Tool role | Connector | Access managed in | Part card version |
|---|---|---|---|
| design source | `[ORG]AIOC-PPD` release port | Panel; the grant is signed at the tool gateway as `connect-external-port` | 49GAION Process and Position Design, v2 |
| returns to the operating model | `[ORG]AIOC-TOM` return port | Panel; as above | 49GAION Target Operating Model, v1 |
| source of record | `[ORG]AIOC-SL` output socket | Panel; as above | 49GAION Source Lifecycle, v1 |
| records of work | the projection over the organisation's own tools (Annex H) | Panel; as above | — |

**Mechanism register.** Read on 15 October 2026. A row is never deleted.

| ID | Mechanism | What it does | Where it lives | Today | Target |
|---|---|---|---|---|---|
| M-01 | Release check | admits only decided releases whose hashes match their filed copies | — | decided, not built | build |
| M-02 | Return path | sends returns, holds touched elements, counts rounds, ends each return | — | decided, not built | build (with the PPD and TOM changes) |
| M-03 | Gap checks | the code checks of Annex F | — | decided, not built | build |
| M-04 | Citation resolver | resolves each citation to an element, its version and a quoted span | — | decided, not built | build |
| M-05 | Package lint | keeps the package to drafts for decision: no names; no amount in a brief and no uncited amount anywhere; every brief and draft marked; every draft reviewed before decision | — | decided, not built | build |
| M-06 | Trace query | from any artefact to its design element, deciding position and decision, and back; a plain-language comparison of any two versions | — | decided, not built | build |
| M-07 | Review rule | as carried from `[ORG]AIOC-TOM` | `[ORG]AIOC-TOM` code project, when built | decided, not built | reuse |
| M-08 | Ladder enforcement | applies a change only at the level its class holds; level 2 only within a signed class; drops a class on any error, complaint or change of engine | the tool gateway | decided, not built | build |
| M-09 | Roll-up check | no figure leaves on fewer than `min_group` positions or for a single position | — | decided, not built | build |
| M-10 | Version register | verified or due; reminders; notices; acknowledgements by version | — | decided, not built | build |
| M-11 | Checklist runner | runs a procedure per case, holding each gate for its position's approval | — | decided, not built | build |
| M-12 | The projection | removes who did the work before any record reaches this AIOC | top management's own mechanism | decided, not built | build (by the Cell carrying `[ORG]HOAC-TM`) |
| M-13 | Conformance computation | compares records of work with the designed process, by process dimensions only | — | decided, not built | build |
| M-14 | Value warning rules | warns of value or a date at risk, by written rules | — | decided, not built | build |
| M-15 | Export and re-import | the full export, proven by re-import into a fresh instance | — | decided, not built | build |

**Reserve.**

| ID | Idea | Why held | Reconsider when |
|---|---|---|---|
| R-01 | Slices 2 to 4 of `PRD-[ORG]AIOC-DI-001` | slice 1 first, by the governing seat's direction | taken up in v0.2.0 on the governing seat's direction to complete this stage (`decisions/DR-0004`); the slices stay the order of building (§5.0) |
| R-02 | A shared review service for every design stage | one more part to build before the first run | a fourth stage needs the same rule |

## 9. Fixed tests: index, triggers and scores

The cases are written in `tests/TEST-DI.md`. Cases 1 to 17 are the Library's TEST-DELIVERY-AND-IMPLEMENTATION v1, unchanged. Cases 18 to 94 are this AIOC's own; cases 51 to 94 were added on 18 October 2026, before any use (`decisions/DR-0004`). The Delivery Lead's seat test is DDL-1 to DDL-5. The owner of every part's test is the DI Delivery Lead; the owner of the AIOC's whole test, and of the Delivery Lead's own seat test, is the Cell carrying `[ORG]HOAC-TM`. Library cases 9, 11 (level 2), 13 (the projection), 14 and 16 (the full export) test features now designed here (§5.17 to §5.25; Annexes G and H).

| Part | Test ID and version | Cases of TEST-DI v1 | Evidence level | Last run | Result |
|---|---|---|---|---|---|
| `[ORG]AIOC-DI` (whole) | TEST-DI v1 | all (1–94) | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DDL` DI Delivery Lead | TEST-DI-DDL v1 | DDL-1 to DDL-5 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-COSDI` Chief of Staff (with Office, Input socket, Needs Requests, Decision Package and Filing, Versions and Checklists, Export) | TEST-DI-COSDI v1 | 1, 2, 4, 8, 10–13, 15–22, 25, 40–46, 48, 51, 55, 66, 69–71, 73, 74, 78, 83, 84, 86, 89, 92, 94 | MEASURED | — | `NOT_RUN` |
| Panel | default Panel test | — | MEASURED | — | `NOT_RUN` |
| `[ORG]POD-DD` Diagnosis | TEST-DI-DD v1 | 2, 3, 5, 23, 24, 26–29, 49, 52–54, 81, 93 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DDM` Design Mapper | TEST-DI-DDM v1 | 2, 23, 24, 49, 93 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DGA` Gap Auditor | TEST-DI-DGA v1 | 5, 26–28 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DHC` Health Checker | TEST-DI-DHC v1 | 29, 81 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DLD` Light Designer | TEST-DI-DLD v1 | 3, 52–54 | MEASURED | — | `NOT_RUN` |
| `[ORG]POD-DP` Preparation | TEST-DI-DP v1 | 6, 8, 30–35, 50, 85–87 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DPW` Procedure Writer | TEST-DI-DPW v1 | 6, 30, 31 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DBW` Brief Writer | TEST-DI-DBW v1 | 6, 32, 85–87 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DTP` Transition Planner | TEST-DI-DTP v1 | 8, 33–35, 50 | MEASURED | — | `NOT_RUN` |
| `[ORG]POD-DA` Answers | TEST-DI-DA v1 | 7, 36–38, 91 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DAG` Answer Guide | TEST-DI-DAG v1 | 7, 36, 37, 91 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DCV` Citation Verifier | TEST-DI-DCV v1 | 36, 38 | MEASURED | — | `NOT_RUN` |
| `[ORG]POD-DR` Review | TEST-DI-DR v1 | 39 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DBRA` to `[ORG]CELL-DBRC` Blind Reviewers | TEST-DI-DBRA v1 to TEST-DI-DBRC v1 | 39 | MEASURED | — | `NOT_RUN` |
| `[ORG]POD-DL` Launch | TEST-DI-DL v1 | 8, 56–61 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DIP` Implementation Planner | TEST-DI-DIP v1 | 56 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DCA` Change Analyst | TEST-DI-DCA v1 | 57 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DLB` Learning Builder | TEST-DI-DLB v1 | 58 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DRA` Readiness Assessor | TEST-DI-DRA v1 | 8, 59, 60 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DIA` Issue Analyst | TEST-DI-DIA v1 | 61 | MEASURED | — | `NOT_RUN` |
| `[ORG]POD-DO` Operations | TEST-DI-DO v1 | 9, 62–68, 72, 91 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DRK` Rhythm Keeper | TEST-DI-DRK v1 | 62–64, 72 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DMB` Measures Builder | TEST-DI-DMB v1 | 65, 66, 91 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DVT` Value Tracker | TEST-DI-DVT v1 | 9, 67, 68 | MEASURED | — | `NOT_RUN` |
| `[ORG]POD-DCI` Continuous Improvement | TEST-DI-DCI v1 | 13, 14, 75–80, 82, 88, 90 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DPA` Process Analyst | TEST-DI-DPA v1 | 13, 75, 76, 88 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DCP` Change Proposer | TEST-DI-DCP v1 | 77, 78 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DTD` Trial Designer | TEST-DI-DTD v1 | 79 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DTJ` Trial Judge | TEST-DI-DTJ v1 | 14, 80 | MEASURED | — | `NOT_RUN` |
| `[ORG]CELL-DCM` Capability Mentor | TEST-DI-DCM v1 | 82, 90 | MEASURED | — | `NOT_RUN` |
| Type (Specialised) | TEST-DI v1, case 47 | 47 | MEASURED | — | `NOT_RUN` |

- **Re-run triggers.** The template defaults, plus any change to the design return contract, to the PPD or TOM release format, to the Source Lifecycle output socket, to the check list of Annex F, to the package lint, to the ladder (Annex G), to the projection (Annex H), or to `min_group`.
- **Complete** only when every part's test has a visible result. `NOT_RUN` is never PASS.

**Checks that are not fixed tests.**

| Check | Placement | Budget per item | Degradation order | Blocks only for |
|---|---|---|---|---|
| Outbound name check: no person's name in any return, request, answer or package part | router | each outbound message | none | the message |
| Citation verification | inside the producer's loop, at most 2 fix rounds | each citation | none | the draft or the answer |
| Package lint | as evidence on the verdict record of RP4 | each package | none | the filing |
| Return reconciliation: every return sent has a filed copy with the same hash, and every return has ended or is within its deadline | after completion | daily | none; a failure opens a defect | nothing; it flags |
| Roll-up check: no figure for a single position, none on fewer than `min_group` positions | router, on every outbound measure, finding or view | each item | none | the item |
| Projection check: no record of work carries a field that identifies who did the work | Input socket | each record | none | the record, refused whole |
| Ladder record reconciliation: every applied change belongs to a signed class, has its rollback and was reported the same day | after completion | daily | none; a failure drops the class to level 1 and opens a defect | the class |

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
5. **It reads records of the organisation's work** (FR-19). Reason: improving the running organisation needs the work as it runs. Bounds: only through the projection, only after Annex H holds, at process level only.
6. **It applies changes at level 2.** Reason: small reversible upkeep should not wait on a row each time. Bounds: only within a class the owner position signed, never a type of the Human Floor signature list (Annex G).

## 12. Lessons and proposals to the mother

One dated line per lesson, each written without any organisation's details. Nothing is proposed upstream without the governing seat's word; the drafts are in `upstream/PROPOSALS.md`.

1. 2026-10-15 · A decided design is not yet a working organisation: procedures, briefs for counsel and finance, the transition plan and the go-live criteria are still needed, and the organisation needs a stage beside it through launch and after. Test questions added: cases 30 to 35. This text is the mother.
2. 2026-10-15 · An assistant that answers questions about how an organisation works must answer only from the decided design, with a second engine checking each citation, and say "I do not know" otherwise. Test questions added: cases 36 to 38.
3. 2026-10-16 · The value an organisation expects from its new design, and the order in which its parts matter, are decided before this stage; this stage carries them unchanged and starts its rollout and its register of value from them. Test questions added: cases 49 and 50 (`decisions/DR-0003`).
4. 2026-10-18 · A stage that stays with an organisation after launch needs, beyond the launch package: one rhythm with single logs; a value register whose gates finance alone passes; versions acknowledged by the positions they concern; process watching at process level, only through a projection that removes who did the work; trials judged by a seat that did not propose them; and a drill that proves the organisation can run without it. Test questions added: cases 51 to 94 (`decisions/DR-0004`).

## 13. For the `[ORG]HOAC-ACS` seat, and every decision only a human seat can take

Every decision that only a human seat can take is listed here once. Silence decides nothing; a general approval decides no row.

| ID | Decision | Seat | Default |
|---|---|---|---|
| H-01 | Name the Requesting Authority's Cell: the GOV Cell itself, or a human Cell to which it delegates these decisions (`delegate-authority`) | GOV | none: T0 fails |
| H-02 | **Top management's own mechanism.** Arrange the DI Delivery Lead position and any HOAC position added to this AIOC. Nothing of who occupies them enters this blueprint | the Cell carrying `[ORG]HOAC-TM` | the position is vacant: the AIOC does not join |
| H-03 | Install `[ORG]AIOC-DI` (`create-or-install-unit`); its `change-parent`; its `restart-stopped-unit` | the Cell carrying `[ORG]HOAC-TM` | none |
| H-04 | Accept the PPD, TOM and Source Lifecycle changes this AIOC needs (`upstream/PROPOSALS.md`, items 1 to 4; items 1 and 2 are made in the PPD blueprint `v0.4.0` and the TOM blueprint `v0.5.0`) | the Cell carrying `[ORG]HOAC-TM`, made through OCO | required before joining |
| H-05 | The connection grants to PPD, TOM and Source Lifecycle (`connect-external-port`), their widening and revocation | the `[ORG]HOAC-ACS` positions over those AIOCs | none: T0 fails |
| H-06 | `modes_enabled`, `gap_bars`, `answer_bars`, `mapping_bars`, `language`, `return_round_deadline`, `return_rounds_max`, `review_budget_per_run`, `reduced_review_permitted` and the AIOC's `budget_cap` | the Cell carrying `[ORG]HOAC-TM` | none: must be set; reduced review `no` |
| H-07 | The permission ladder: each class of action and its level, 0, 1 or 2 (Annex G), and `ladder_thresholds`; a class moves up one level only by the owner position's signed decision and a fixed-test score at or above its recorded threshold | the owner position | every class at level 1; a read-only class at level 0 |
| H-08 | `deciding_positions`: the go or no-go position; the counsel position for each jurisdiction; the finance position; the data-protection position; the owner position, where it is not the Requesting Authority | Requesting Authority | none: T0 fails |
| H-09 | Open the run; name the mode and the scope | Requesting Authority | none: no run |
| H-10 | The rows of S1 to S4: mode B rows `not mapped`; the route of each gap; assumptions; contradictions; each procedure, brief, plan element and go-live criterion with its threshold; each element of the package | Requesting Authority, or the deciding position the row names | undecided |
| H-11 | The go or no-go itself, at go-live | the go or no-go deciding position | never this AIOC |
| H-12 | Inside a run: rule on contested `MATERIAL` findings; accept a reduced level within H-06; approve a second run; attest T0 to T3 | the DI Delivery Lead | none taken; the step waits |
| H-13 | Create `<org>aioc-di-records` and `-records-restricted`, recorded first (Naming Standard R9) | the Cell carrying `[ORG]HOAC-TM` | before the first run |
| H-14 | Send the drafts of `upstream/` to the parts they concern | GOV | after this blueprint is approved |
| H-15 | Approve this blueprint `v0.2.1` as the design of `[ORG]AIOC-DI`, slices 1 to 4 | the human hub | it stays a draft; nothing is installed |
| H-16 | Open the service for a filed launch package, naming the parts switched on | Requesting Authority | none: no service |
| H-17 | Process watching (Annex H): the impact assessment and its lawful basis; informing workers or their representatives where law requires; the projection and its connection (`connect-external-port`); then `process_watching` on | the data-protection position; the counsel position, on what the law requires; the Cell carrying `[ORG]HOAC-TM` | off |
| H-18 | Each level-2 class, signed as `sign-standing-action-class`: reversible only, with no legal, pay or employment effect | the owner position | none: every class at level 1 |
| H-19 | The implementation plan; the end of stabilisation; each change of a decided milestone date | the owner position; the date by the review chair | undecided |
| H-20 | Gates L2 and L5 of the value register | the finance position | undecided |
| H-21 | Record that slices 1 and 2 have given evidence, before mode C is enabled; then `modes_enabled` | the Cell carrying `[ORG]HOAC-TM` | mode C off |
| H-22 | `min_group`, `trial_baseline_points`, `reassessment_schedule`, `health_check_schedule`, `drill_schedule`, `in_flight_rule`, `growth_triggers` | as §15 sets for each | the defaults of §15 |
| H-23 | Each yearly drill: its period, and whether it passed | the Cell carrying `[ORG]HOAC-TM` | not run |
| H-24 | `mentor` on, once `advice_bars` is set and met; `council` on, and each engine added to the engine register for it (`change-gateway-policy`); `point_of_work_guidance` on, only once H-17 holds for its records | the Cell carrying `[ORG]HOAC-TM`; the gateway policy as the Standard sets | off |
| H-25 | Pin the reference-model catalogue (`reference_models`), as a tested change of this AIOC | the DI Delivery Lead, as a change approved by the human hub | unavailable |
| H-26 | Each connector to the organisation's tools (`connect-external-port`), read only; any write only within a level-2 class | the `[ORG]HOAC-ACS` position over the tool | none |
| H-27 | Each row of the service: each proposal and trial, each trial's outcome, each priority insertion, each minutes preview, each acknowledgement | the position each row names | undecided |

**Money:** the budget cap and the review budget (H-06); a brief holds no amount, and lists the decisions on amounts the organisation must take; every amount in the cost draft is read from a source or a decision row; gates L2 and L5 are the finance position's (H-20). **People:** this AIOC prepares for positions, never for who fills them; the go or no-go is the deciding position's (H-11); records of work are read only under H-17. **Legal:** every brief and draft goes to the counsel position of its jurisdiction before any decision.

## 14. Change log

| Blueprint version | Date | Change | Template version | Commit |
|---|---|---|---|---|
| v0.1.0 | 2026-10-15 | First blueprint of `[ORG]AIOC-DI`, the mother text of the Library part 49GAION Delivery and Implementation (proposed): slice 1, the gap audit and the launch essentials; modes A and B; five stages; answers with verified citations; returns under the Library contract; TEST-DI v1 | v1.5.0 at `e89ed1d` | this commit |
| v0.1.1 | 2026-10-16 | Receives the answers to its returns, from `[ORG]AIOC-PPD` and `[ORG]AIOC-TOM` (a `tom-in` port and Annex B, rule 5), and the release notice of `[ORG]AIOC-PPD` under its contract (`decisions/DR-0002`); a return set aside carries its elements forward on the stated basis; the Library texts are merged, no longer proposed; the TOM rules are carried from the TOM blueprint `v0.5.0`. TEST-DI v1, case 48 | v1.5.0 at `e89ed1d` | this pull request |
| v0.1.2 | 2026-10-16 | Carries the value case of the TOM Release and each element's decided priority in the design map, unchanged (§5.1 rule 1; A.1), for the register of value of slice 2; the transition waves follow the decided priority (A.6); Annex D item 13; Annex E pins TOM `v0.6.0` (`decisions/DR-0003`). TEST-DI v1, cases 49 and 50, added before any use | v1.5.0 | this pull request |
| v0.2.0 | 2026-10-18 | Complete, slices 1 to 4 (`decisions/DR-0004`): mode C and the light design (§5.11); the service, S5 Accompany (§5.12 to §5.16), S6 Operate (§5.17 to §5.20) and S7 Improve (§5.21 to §5.24); export (§5.25); drafts from the organisation's own templates and the cost draft (§5.6); the health check each quarter; answers at the point of work; the ladder with level 2 (Annex G); records of work through the projection (Annex H); three Pods and fourteen Cells added; TEST-DI v1, cases 51 to 94, added before any use | v1.6.0 at `acdcbe5` | this pull request |
| v0.2.1 | 2026-10-19 | The Chief of Staff takes its COS code: `[ORG]CELL-DCS` → `[ORG]CELL-COSDI` (Naming Standard R16, `49GAION/DR-0028`; `decisions/DR-0005`). The old code is retired and kept in the card's lineage; the part test is renamed; nothing else changes | v1.6.0 at `acdcbe5` | this repository's pull request for this version |

---

## 15. Configuration

The template's slots, all `none: must be set` until the organisation sets them (Protocol §11), plus these slots of this AIOC:

| Slot | Card key | Default offered | Allowed values | Set by |
|---|---|---|---|---|
| Requesting Authority Cell | `requesting_authority_cell` | none: must be set | the Cell carrying `[ORG]HOAC-GOV`, or a human Cell it delegated these decisions to | the Cell carrying `[ORG]HOAC-GOV` |
| Modes enabled | `modes_enabled` | A, B | A, B, C (C only after H-21) | the Cell carrying `[ORG]HOAC-TM` |
| Deciding positions | `deciding_positions` | none: must be set | position codes of the organisation's decided design: the go or no-go position; the counsel position for each jurisdiction; the finance position; the data-protection position; the owner position, where it is not the Requesting Authority | Requesting Authority |
| Rows per needs pass | `rows_per_pass` | 12 | 1–12 | DI Delivery Lead |
| Passes past their deadline before a non-response stop | `non_response_passes` | none: must be set | ≥ 1 | the Cell carrying `[ORG]HOAC-TM` |
| Return round deadline; most rounds | `return_round_deadline`; `return_rounds_max` | none: must be set | a period; ≥ 1 | the Cell carrying `[ORG]HOAC-TM` |
| Engines per review point | `review_engines` | 3 | 3–5 | DI Delivery Lead, within the review budget |
| Families per review | `review_families_min` | 2 | 2–3 | DI Delivery Lead |
| Reduced review permitted | `reduced_review_permitted` | `no` | `yes`, `no` | the Cell carrying `[ORG]HOAC-TM` (never this AIOC's own `[ORG]HOAC-ACS` position) |
| Review budget per run | `review_budget_per_run` | none: must be set | within `budget_cap` | the Cell carrying `[ORG]HOAC-TM` |
| Gap bars | `gap_bars` | none: must be set | two shares: blocking gaps found, at or above; false gaps, at or below | the Cell carrying `[ORG]HOAC-TM` |
| Answer bars | `answer_bars` | none: must be set | two shares: grounded answers; "I do not know" on unanswerable questions | the Cell carrying `[ORG]HOAC-TM` |
| Mapping bars | `mapping_bars` | none: must be set before mode B is used | one share: mode B mapping accuracy on a sample set | the Cell carrying `[ORG]HOAC-TM` |
| Permission ladder | `ladder` | every class at level 1; a read-only class at level 0 | level 0, 1 or 2 per class; level 2 only for a class signed as `sign-standing-action-class` (Annex G) | the owner position |
| Ladder thresholds | `ladder_thresholds` | none: no class moves up until set | per class, a fixed-test score | the owner position |
| Process watching | `process_watching` | off | on only when Annex H holds (H-17) | the Cell carrying `[ORG]HOAC-TM` |
| Smallest group for a figure | `min_group` | 3 | ≥ 3 | the Cell carrying `[ORG]HOAC-TM` |
| Baseline points for run-chart rules | `trial_baseline_points` | 10 | ≥ 10 | the owner position |
| Reassessment of the whole design | `reassessment_schedule` | none: must be set | a period | the owner position |
| Health check in the service | `health_check_schedule` | quarterly | a period, at most a quarter | the owner position |
| The drill without DI | `drill_schedule` | yearly | a period, at most a year | the Cell carrying `[ORG]HOAC-TM` |
| Cases in flight under a changed procedure | `in_flight_rule` | none: must be set | finish under the old version; move to the new at the next gate; or as each procedure states | the owner position |
| Growth triggers, in mode C | `growth_triggers` | none: must be set in mode C | the organisation's own triggers | the owner position |
| Reference models | `reference_models` | unavailable | unavailable, or a pin (commit and SHA-256) of the Library's reference-model catalogue | the DI Delivery Lead (H-25) |
| The mentor | `mentor` | off | off, on | the Cell carrying `[ORG]HOAC-TM` (H-24) |
| Advice bars | `advice_bars` | none: must be set before the mentor is on | one score on an expert-rated rubric | the Cell carrying `[ORG]HOAC-TM` |
| The council | `council` | off | off, on | the Cell carrying `[ORG]HOAC-TM` (H-24) |
| Guidance at the point of work | `point_of_work_guidance` | off | off, on | the Cell carrying `[ORG]HOAC-TM` (H-24) |
| Language | `language` | none: must be set | the organisation's language; English and Persian are built first (NFR-08) | the Cell carrying `[ORG]HOAC-TM` |
| Template slots | `office_accountable_human`, `central_head`, `discussion_limits`, `waiting_deadlines`, `bounce_limit`, `chain_depth` (at least 1), `halt_request_priority` (immediate), `budget_cap`, `unattended_action` (`read-record-triage`), and the `v1.6.0` rows | as the template | — | as the template |

---

## 16. Type

- **Type:** Specialised.
- **Why this AIOC exists:** an organisation needs its decided design taken into a running organisation, with someone beside it through launch and after, who decides nothing for it and hands its skills over until the organisation can run without it.
- **Type-specific test:** TEST-DI v1, case 47 · result `NOT_RUN`.

---

## 17. Cells and Pods

The parts inside this AIOC (`docs/CELLS-AND-PODS.md` of `49GAION-aioc`). The role and nature of this AIOC are read from the type of its top Cell, the DI Delivery Lead. Every field that points to a human takes a position code only.

| Code | Kind | Type | Filler kind | HOAC label | Parent | Fixed test (owner) | External ports |
|---|---|---|---|---|---|---|---|
| `[ORG]CELL-DDL` | CELL | Human Seat | human | `[ORG]HOAC-ACS` | `[ORG]AIOC-DI` | TEST-DI-DDL v1 (the Cell carrying `[ORG]HOAC-TM`) | none |
| `[ORG]CELL-COSDI` | CELL | AI Chief of Staff | ai | none | `[ORG]AIOC-DI` | TEST-DI-COSDI v1 (`[ORG]CELL-DDL`) | `ppd-in`, `ppd-out`, `tom-out`, `tom-in`, `sl-in`, `sl-out`, `tools-in` |
| `[ORG]POD-DD` | POD | AI Pod | — | none | `[ORG]AIOC-DI` | TEST-DI-DD v1 (`[ORG]CELL-DDL`) | — |
| `[ORG]CELL-DDM` | CELL | AI Agent | ai | none | `[ORG]POD-DD` | TEST-DI-DDM v1 (`[ORG]CELL-DDL`) | none |
| `[ORG]CELL-DGA` | CELL | AI Agent | ai | none | `[ORG]POD-DD` | TEST-DI-DGA v1 (`[ORG]CELL-DDL`) | none |
| `[ORG]CELL-DHC` | CELL | AI Agent | ai | none | `[ORG]POD-DD` | TEST-DI-DHC v1 (`[ORG]CELL-DDL`) | none |
| `[ORG]CELL-DLD` | CELL | AI Agent | ai | none | `[ORG]POD-DD` | TEST-DI-DLD v1 (`[ORG]CELL-DDL`) | none |
| `[ORG]POD-DP` | POD | AI Pod | — | none | `[ORG]AIOC-DI` | TEST-DI-DP v1 (`[ORG]CELL-DDL`) | — |
| `[ORG]CELL-DPW` | CELL | AI Agent | ai | none | `[ORG]POD-DP` | TEST-DI-DPW v1 (`[ORG]CELL-DDL`) | none |
| `[ORG]CELL-DBW` | CELL | AI Agent | ai | none | `[ORG]POD-DP` | TEST-DI-DBW v1 (`[ORG]CELL-DDL`) | none |
| `[ORG]CELL-DTP` | CELL | AI Agent | ai | none | `[ORG]POD-DP` | TEST-DI-DTP v1 (`[ORG]CELL-DDL`) | none |
| `[ORG]POD-DA` | POD | AI Pod | — | none | `[ORG]AIOC-DI` | TEST-DI-DA v1 (`[ORG]CELL-DDL`) | — |
| `[ORG]CELL-DAG` | CELL | AI Agent | ai | none | `[ORG]POD-DA` | TEST-DI-DAG v1 (`[ORG]CELL-DDL`) | none |
| `[ORG]CELL-DCV` | CELL | AI Agent | ai | none | `[ORG]POD-DA` | TEST-DI-DCV v1 (`[ORG]CELL-DDL`) | none |
| `[ORG]POD-DR` | POD | AI Pod | — | none | `[ORG]AIOC-DI` | TEST-DI-DR v1 (`[ORG]CELL-DDL`) | — |
| `[ORG]CELL-DBRA` … `[ORG]CELL-DBRC` | CELL | AI Agent | ai | none | `[ORG]POD-DR` | TEST-DI-DBRA v1 … TEST-DI-DBRC v1 (`[ORG]CELL-DDL`) | none |
| `[ORG]POD-DL` | POD | AI Pod | — | none | `[ORG]AIOC-DI` | TEST-DI-DL v1 (`[ORG]CELL-DDL`) | — |
| `[ORG]CELL-DIP` | CELL | AI Agent | ai | none | `[ORG]POD-DL` | TEST-DI-DIP v1 (`[ORG]CELL-DDL`) | none |
| `[ORG]CELL-DCA` | CELL | AI Agent | ai | none | `[ORG]POD-DL` | TEST-DI-DCA v1 (`[ORG]CELL-DDL`) | none |
| `[ORG]CELL-DLB` | CELL | AI Agent | ai | none | `[ORG]POD-DL` | TEST-DI-DLB v1 (`[ORG]CELL-DDL`) | none |
| `[ORG]CELL-DRA` | CELL | AI Agent | ai | none | `[ORG]POD-DL` | TEST-DI-DRA v1 (`[ORG]CELL-DDL`) | none |
| `[ORG]CELL-DIA` | CELL | AI Agent | ai | none | `[ORG]POD-DL` | TEST-DI-DIA v1 (`[ORG]CELL-DDL`) | none |
| `[ORG]POD-DO` | POD | AI Pod | — | none | `[ORG]AIOC-DI` | TEST-DI-DO v1 (`[ORG]CELL-DDL`) | — |
| `[ORG]CELL-DRK` | CELL | AI Agent | ai | none | `[ORG]POD-DO` | TEST-DI-DRK v1 (`[ORG]CELL-DDL`) | none |
| `[ORG]CELL-DMB` | CELL | AI Agent | ai | none | `[ORG]POD-DO` | TEST-DI-DMB v1 (`[ORG]CELL-DDL`) | none |
| `[ORG]CELL-DVT` | CELL | AI Agent | ai | none | `[ORG]POD-DO` | TEST-DI-DVT v1 (`[ORG]CELL-DDL`) | none |
| `[ORG]POD-DCI` | POD | AI Pod | — | none | `[ORG]AIOC-DI` | TEST-DI-DCI v1 (`[ORG]CELL-DDL`) | — |
| `[ORG]CELL-DPA` | CELL | AI Agent | ai | none | `[ORG]POD-DCI` | TEST-DI-DPA v1 (`[ORG]CELL-DDL`) | none |
| `[ORG]CELL-DCP` | CELL | AI Agent | ai | none | `[ORG]POD-DCI` | TEST-DI-DCP v1 (`[ORG]CELL-DDL`) | none |
| `[ORG]CELL-DTD` | CELL | AI Agent | ai | none | `[ORG]POD-DCI` | TEST-DI-DTD v1 (`[ORG]CELL-DDL`) | none |
| `[ORG]CELL-DTJ` | CELL | AI Agent | ai | none | `[ORG]POD-DCI` | TEST-DI-DTJ v1 (`[ORG]CELL-DDL`) | none |
| `[ORG]CELL-DCM` | CELL | AI Agent | ai | none | `[ORG]POD-DCI` | TEST-DI-DCM v1 (`[ORG]CELL-DDL`) | none |

**The card data (the blueprint governs).** `tools/make_cards.py` expands the block below into the complete unit cards and bot identity cards, writes them into `cards/`, and checks them against the schemas of `49GAION-protocol`, Naming Standard R15 and R16, and this blueprint.

```yaml
parts:
  defaults:
    accountable_to: "[ORG]CELL-DDL"
    card_version: "v0.2.1"
    version: "0.2.1"
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
    - code: "[ORG]CELL-COSDI"
      code_rule: "R16"                     # 49GAION/DR-0028; replaces [ORG]CELL-DCS (retired, R5)
      lineage: { id: "[ORG]CELL-DCS", version: "0.2.0", relation: "derived" }
      full_name: "DI Chief of Staff"
      role: "Chief of Staff"
      parent: "[ORG]AIOC-DI"
      type: "AI Chief of Staff"
      filler_kind: "ai"
      cell_kind: "chief-of-staff-cell"
      test: { id: "TEST-DI-COSDI", cases: "1, 2, 4, 8, 10-13, 15-22, 25, 40-46, 48, 51, 55, 66, 69-71, 73, 74, 78, 83, 84, 86, 89, 92, 94" }
      ai_in: ["release notice", "return answer", "source reference", "needs answer", "needs status", "change notice", "records of work through the projection", "needs candidate", "return draft", "locked outputs of the Pods", "settled review records", "verified answer"]
      ai_out: ["Input Pack version", "dispatch to a Pod", "review packet", "return", "needs request", "missing report", "Decision Package", "launch package filing", "living design filing", "export"]
      hu_in: ["run request from the Requesting Authority's Cell (references only)", "service request from the Requesting Authority's Cell (references only)", "a question from a position (never a source)", "a problem report from a position (never a source)", "a decision of a deciding position", "an insertion, a preview approval or an acknowledgement by a position", "run control from the DI Delivery Lead"]
      hu_out: ["answer to the asking position", "Decision Package rows to the deciding positions", "rows for decision to the deciding positions", "forum packs and minutes previews to the forum's positions", "notices to the positions a record concerns", "a learning path and its check results to the learner position only", "run brief and ruling sheets to the DI Delivery Lead", "filing notice to the Requesting Authority's Cell"]
      external_ports:
        - { port: "ppd-in", direction: "input", accepted_content: ["release notice", "return answer"], authority_limit: "the read scope signed under connect-external-port over [ORG]AIOC-PPD", audit_trail: "unit register; serve log of [ORG]AIOC-PPD" }
        - { port: "ppd-out", direction: "output", accepted_content: ["return"], authority_limit: "returns only, under the scope signed over [ORG]AIOC-PPD", audit_trail: "unit register; the Work Item record" }
        - { port: "tom-out", direction: "output", accepted_content: ["return"], authority_limit: "returns only, under the scope signed over [ORG]AIOC-TOM", audit_trail: "unit register; the Work Item record" }
        - { port: "tom-in", direction: "input", accepted_content: ["return answer"], authority_limit: "answers to this AIOC's returns only, under the scope signed over [ORG]AIOC-TOM", audit_trail: "unit register; the Work Item record" }
        - { port: "sl-in", direction: "input", accepted_content: ["source reference", "needs answer", "needs status", "change notice"], authority_limit: "the read scope signed under connect-external-port over [ORG]AIOC-SL", audit_trail: "unit register; serve log of [ORG]AIOC-SL" }
        - { port: "sl-out", direction: "output", accepted_content: ["needs request", "missing report", "return filing", "launch package filing", "living design filing"], authority_limit: "the request and write scope signed over [ORG]AIOC-SL: this AIOC's own packages, decided versions and design reports only", audit_trail: "unit register; serve log of [ORG]AIOC-SL" }
        - { port: "tools-in", direction: "input", accepted_content: ["records of work through the projection"], authority_limit: "read only, within the scope signed under connect-external-port over the projection; only while process watching is on (Annex H)", audit_trail: "unit register; the projection's log" }
      bot:
        allowed_actions: ["dispatch Cells of this AIOC", "build Input Pack versions through the code steps", "lock outputs and run code steps", "draw review engines and run the review code steps", "write the run record", "send reviewed returns and file them in [ORG]AIOC-SL", "send needs requests and Missing Reports to [ORG]AIOC-SL", "send verified answers to the asking position", "send Decision Package rows to the deciding positions", "file a package whose elements are decided", "send rows for decision, forum packs, minutes previews and notices to positions", "enter a draft a position inserted", "apply a level-2 change within a class the owner position approved in advance, with its rollback", "keep the version register and record acknowledgements", "run checklists per case", "produce the export"]
        ask_first_actions: ["a second run in parallel", "a budget above the cap", "a reduced review level", "any change to configuration", "anything outside its role card"]
    - { code: "[ORG]CELL-DDM", full_name: "DI Design Mapper", role: "Design Mapper", parent: "[ORG]POD-DD", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DDM", cases: "2, 23, 24, 49, 93" }, ai_in: ["Input Pack version"], ai_out: ["design map", "return draft", "needs candidate"], bot: { allowed_actions: ["read a release or map an outside design, element by element", "draft returns with their evidence"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DGA", full_name: "DI Gap Auditor", role: "Gap Auditor", parent: "[ORG]POD-DD", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DGA", cases: "5, 26-28" }, ai_in: ["design map", "check record", "Input Pack version"], ai_out: ["gap report draft", "needs candidate"], bot: { allowed_actions: ["judge the checks code cannot decide", "write each gap with its consequence, evidence, fix and route"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DHC", full_name: "DI Health Checker", role: "Health Checker", parent: "[ORG]POD-DD", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DHC", cases: "29, 81" }, ai_in: ["design map", "Input Pack version", "the living design, the logs and the measures"], ai_out: ["health check draft"], bot: { allowed_actions: ["answer the health checklist with evidence"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DLD", full_name: "DI Light Designer", role: "Light Designer", parent: "[ORG]POD-DD", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DLD", cases: "3, 52-54" }, ai_in: ["Input Pack version"], ai_out: ["light design draft", "needs candidate"], bot: { allowed_actions: ["draft the light design from the pack, every element provisional"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DPW", full_name: "DI Procedure Writer", role: "Procedure Writer", parent: "[ORG]POD-DP", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DPW", cases: "6, 30, 31" }, ai_in: ["process records of the design", "decided gap routes"], ai_out: ["procedure drafts", "gap candidate"], bot: { allowed_actions: ["write procedures, forms and templates under each process"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DBW", full_name: "DI Brief Writer", role: "Brief Writer", parent: "[ORG]POD-DP", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DBW", cases: "6, 32, 85-87" }, ai_in: ["design registers", "decided gap routes", "jurisdictions and entities in scope"], ai_out: ["brief drafts", "needs candidate"], bot: { allowed_actions: ["write briefs, and drafts from the organisation's own templates, for counsel and finance"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DTP", full_name: "DI Transition Planner", role: "Transition Planner", parent: "[ORG]POD-DP", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DTP", cases: "8, 33-35, 50" }, ai_in: ["units, positions, processes and the crosswalk of the design", "decided gap routes"], ai_out: ["transition plan draft", "go-live criteria draft"], bot: { allowed_actions: ["draft the transition plan and the go-live criteria"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DAG", full_name: "DI Answer Guide", role: "Answer Guide", parent: "[ORG]POD-DA", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DAG", cases: "7, 36, 37, 91" }, ai_in: ["question by ID", "the admitted design and the filed package"], ai_out: ["answer draft with citations"], bot: { allowed_actions: ["draft answers only from the decided design, with citations"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DCV", full_name: "DI Citation Verifier", role: "Citation Verifier", parent: "[ORG]POD-DA", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DCV", cases: "36, 38" }, ai_in: ["draft with citations", "the cited elements and spans"], ai_out: ["verification record"], bot: { allowed_actions: ["check that each citation resolves and supports its claim"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DBRA", full_name: "DI Blind Reviewer A", role: "Blind Reviewer A", parent: "[ORG]POD-DR", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DBRA", cases: "39" }, ai_in: ["review packet", "collated findings of its review"], ai_out: ["review card", "positions on findings"], bot: { allowed_actions: ["write its own review card", "state its own positions on the findings of its review"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DBRB", full_name: "DI Blind Reviewer B", role: "Blind Reviewer B", parent: "[ORG]POD-DR", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DBRB", cases: "39" }, ai_in: ["review packet", "collated findings of its review"], ai_out: ["review card", "positions on findings"], bot: { allowed_actions: ["write its own review card", "state its own positions on the findings of its review"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DBRC", full_name: "DI Blind Reviewer C", role: "Blind Reviewer C", parent: "[ORG]POD-DR", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DBRC", cases: "39" }, ai_in: ["review packet", "collated findings of its review"], ai_out: ["review card", "positions on findings"], bot: { allowed_actions: ["write its own review card", "state its own positions on the findings of its review"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DIP", full_name: "DI Implementation Planner", role: "Implementation Planner", parent: "[ORG]POD-DL", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DIP", cases: "56" }, ai_in: ["filed launch package"], ai_out: ["implementation plan draft"], bot: { allowed_actions: ["draft the implementation plan by position from the launch package"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DCA", full_name: "DI Change Analyst", role: "Change Analyst", parent: "[ORG]POD-DL", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DCA", cases: "57" }, ai_in: ["the crosswalk and the launch package"], ai_out: ["change impact draft", "stakeholder register draft", "briefing drafts", "adoption measure drafts"], bot: { allowed_actions: ["draft the change impact, the stakeholder register, the briefings and the adoption measures"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DLB", full_name: "DI Learning Builder", role: "Learning Builder", parent: "[ORG]POD-DL", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DLB", cases: "58" }, ai_in: ["job descriptions and procedures"], ai_out: ["learning path drafts"], bot: { allowed_actions: ["draft learning paths and their checks"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DRA", full_name: "DI Readiness Assessor", role: "Readiness Assessor", parent: "[ORG]POD-DL", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DRA", cases: "8, 59, 60" }, ai_in: ["go-live criteria and their evidence", "the plan and the defect log"], ai_out: ["readiness record", "rehearsal scripts", "go or no-go package draft", "stabilisation record"], bot: { allowed_actions: ["read the criteria's evidence, write rehearsal scripts and records, draft the go or no-go package"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DIA", full_name: "DI Issue Analyst", role: "Issue Analyst", parent: "[ORG]POD-DL", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DIA", cases: "61" }, ai_in: ["problem report by ID", "the living design and the logs"], ai_out: ["problem record draft", "issue list order"], bot: { allowed_actions: ["draft problem records and order issues by their effect on processes"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DRK", full_name: "DI Rhythm Keeper", role: "Rhythm Keeper", parent: "[ORG]POD-DO", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DRK", cases: "62-64, 72" }, ai_in: ["forum register and review calendar", "the logs", "the measures", "the value register", "notes submitted by a participant position"], ai_out: ["forum pack", "minutes draft", "notices of items off track", "priority drafts"], bot: { allowed_actions: ["build forum packs, draft minutes and quarterly priorities, list items off track"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DMB", full_name: "DI Measures Builder", role: "Measures Builder", parent: "[ORG]POD-DO", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DMB", cases: "65, 66, 91" }, ai_in: ["the measures of the design", "records of work through the projection"], ai_out: ["measure and dashboard drafts"], bot: { allowed_actions: ["draft measures and dashboards at process, step and unit level"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DVT", full_name: "DI Value Tracker", role: "Value Tracker", parent: "[ORG]POD-DO", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DVT", cases: "9, 67, 68" }, ai_in: ["the value case carried", "the plan, proposals and measures", "decisions of the finance position"], ai_out: ["value register version", "value warnings"], bot: { allowed_actions: ["keep the initiative and value register from sources and decisions"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DPA", full_name: "DI Process Analyst", role: "Process Analyst", parent: "[ORG]POD-DCI", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DPA", cases: "13, 75, 76, 88" }, ai_in: ["records of work through the projection", "the living design"], ai_out: ["conformance record", "findings"], bot: { allowed_actions: ["analyse records of work through the projection at process level, and write findings"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DCP", full_name: "DI Change Proposer", role: "Change Proposer", parent: "[ORG]POD-DCI", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DCP", cases: "77, 78" }, ai_in: ["findings", "problem records", "change notices", "the living design"], ai_out: ["proposal drafts", "return drafts"], bot: { allowed_actions: ["draft proposals and returns from their triggers"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DTD", full_name: "DI Trial Designer", role: "Trial Designer", parent: "[ORG]POD-DCI", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DTD", cases: "79" }, ai_in: ["decided proposal", "the measures"], ai_out: ["trial design draft"], bot: { allowed_actions: ["draft each trial's rules before it starts"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DTJ", full_name: "DI Trial Judge", role: "Trial Judge", parent: "[ORG]POD-DCI", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DTJ", cases: "14, 80" }, ai_in: ["the trial design as decided", "the trial's data"], ai_out: ["trial judgement"], bot: { allowed_actions: ["judge a trial it neither proposed nor designed, by its decided rules"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-DCM", full_name: "DI Capability Mentor", role: "Capability Mentor", parent: "[ORG]POD-DCI", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-DI-DCM", cases: "82, 90" }, ai_in: ["the living design", "the logs", "the skills library", "a request for advice"], ai_out: ["hand-over record", "drill plan", "advice record"], bot: { allowed_actions: ["draft the hand-over list and plan, prepare the drill, draft advice from the skills library"], ask_first_actions: ["anything outside its role card"] } }
  pods:
    - { code: "[ORG]POD-DD", full_name: "DI Diagnosis", type: "AI Pod", inner_units: ["[ORG]CELL-DDM", "[ORG]CELL-DGA", "[ORG]CELL-DHC", "[ORG]CELL-DLD"], top_cell: "[ORG]CELL-DGA", test: { id: "TEST-DI-DD", cases: "2, 3, 5, 23, 24, 26-29, 49, 52-54, 81, 93" }, ai_in: ["Input Pack version"], ai_out: ["design map", "light design", "gap report", "health check", "return draft"] }
    - { code: "[ORG]POD-DP", full_name: "DI Preparation", type: "AI Pod", inner_units: ["[ORG]CELL-DPW", "[ORG]CELL-DBW", "[ORG]CELL-DTP"], top_cell: "[ORG]CELL-DPW", test: { id: "TEST-DI-DP", cases: "6, 8, 30-35, 50, 85-87" }, ai_in: ["design map", "decided gap routes"], ai_out: ["procedures", "briefs and drafts", "transition plan", "go-live criteria"] }
    - { code: "[ORG]POD-DA", full_name: "DI Answers", type: "AI Pod", inner_units: ["[ORG]CELL-DAG", "[ORG]CELL-DCV"], top_cell: "[ORG]CELL-DAG", test: { id: "TEST-DI-DA", cases: "7, 36-38, 91" }, ai_in: ["question by ID", "drafts with citations"], ai_out: ["verified answer", "verification record"] }
    - { code: "[ORG]POD-DR", full_name: "DI Review", type: "AI Pod", inner_units: ["[ORG]CELL-DBRA", "[ORG]CELL-DBRB", "[ORG]CELL-DBRC"], top_cell: "[ORG]CELL-DBRA", test: { id: "TEST-DI-DR", cases: "39" }, ai_in: ["review packet"], ai_out: ["review cards and positions"] }
    - { code: "[ORG]POD-DL", full_name: "DI Launch", type: "AI Pod", inner_units: ["[ORG]CELL-DIP", "[ORG]CELL-DCA", "[ORG]CELL-DLB", "[ORG]CELL-DRA", "[ORG]CELL-DIA"], top_cell: "[ORG]CELL-DIP", test: { id: "TEST-DI-DL", cases: "8, 56-61" }, ai_in: ["filed launch package", "problem reports by ID"], ai_out: ["implementation plan", "change impact", "learning paths", "readiness record", "go or no-go package", "problem records"] }
    - { code: "[ORG]POD-DO", full_name: "DI Operations", type: "AI Pod", inner_units: ["[ORG]CELL-DRK", "[ORG]CELL-DMB", "[ORG]CELL-DVT"], top_cell: "[ORG]CELL-DRK", test: { id: "TEST-DI-DO", cases: "9, 62-68, 72, 91" }, ai_in: ["the living design", "the logs", "the measures", "the value register"], ai_out: ["forum packs", "minutes drafts", "measures and dashboards", "value register version", "priority drafts"] }
    - { code: "[ORG]POD-DCI", full_name: "DI Continuous Improvement", type: "AI Pod", inner_units: ["[ORG]CELL-DPA", "[ORG]CELL-DCP", "[ORG]CELL-DTD", "[ORG]CELL-DTJ", "[ORG]CELL-DCM"], top_cell: "[ORG]CELL-DCP", test: { id: "TEST-DI-DCI", cases: "13, 14, 75-80, 82, 88, 90" }, ai_in: ["records of work through the projection", "the living design", "change notices"], ai_out: ["findings", "proposals", "trial records", "hand-over records"] }
```

- **Accountability.** Every Pod and Cell of this AIOC is `accountable_to` `[ORG]CELL-DDL`. The AIOC itself and the Delivery Lead are `accountable_to` the Cell carrying `[ORG]HOAC-TM`.
- **Bots.** Each AI Cell's bot (twenty-six) has its own identity card, its own credential, `never_signs: true`, and its memory sealed on a change of filler (Protocol §10, item 3). The credential IDs in `cards/bots/` are placeholders.
- The Requesting Authority, the deciding positions, the Chief of Staff of `[ORG]AIOC-SL` and the Cells of `[ORG]AIOC-PPD` and `[ORG]AIOC-TOM` are not Cells of this AIOC.

**Code checks** (Naming Standard R15, R16 and §5), recorded on 15 and 18 October 2026; the Chief of Staff's COS code on 19 October 2026. Each organisation repeats the check of §5.2 against its own register before first use.

| Code | Initials of the full name (R15) | §5.1 | §5.2: no match among this blueprint's codes, nor with `[ORG]AIOC-DI` | §5.3 |
|---|---|---|---|---|
| `[ORG]CELL-DDL` | **D**I **D**elivery **L**ead | pass | pass | pass |
| `[ORG]CELL-COSDI` | R16, item 2 (`49GAION/DR-0028`): COS and the initials of `[ORG]AIOC-DI` → COSDI. It replaces `[ORG]CELL-DCS`, retired at v0.2.1 (R5) and kept in the card's lineage | pass | pass (distinct from the COS codes of the other mothers: `COSSL`, `COSOER`, `COSPC`, `COSPPD`, `COSTOM`, `COSCH`) | pass |
| `[ORG]POD-DD` / `[ORG]CELL-DDM`, `-DGA`, `-DHC` | DI Diagnosis / Design Mapper, Gap Auditor, Health Checker | pass | pass | pass |
| `[ORG]POD-DP` / `[ORG]CELL-DPW`, `-DBW`, `-DTP` | DI Preparation / Procedure Writer, Brief Writer, Transition Planner | pass | pass | pass |
| `[ORG]POD-DA` / `[ORG]CELL-DAG`, `-DCV` | DI Answers / Answer Guide, Citation Verifier | pass | pass | pass |
| `[ORG]POD-DR` / `[ORG]CELL-DBRA` to `-DBRC` | DI Review / Blind Reviewer A to C | pass | pass | pass |
| `[ORG]CELL-DLD` | **D**I **L**ight **D**esigner | pass | pass | pass |
| `[ORG]POD-DL` / `[ORG]CELL-DIP`, `-DCA`, `-DLB`, `-DRA`, `-DIA` | DI Launch / Implementation Planner, Change Analyst, Learning Builder, Readiness Assessor, Issue Analyst | pass | pass (`-DRA` is distinct from `-DBRA`) | pass |
| `[ORG]POD-DO` / `[ORG]CELL-DRK`, `-DMB`, `-DVT` | DI Operations / Rhythm Keeper, Measures Builder, Value Tracker | pass | pass | pass |
| `[ORG]POD-DCI` / `[ORG]CELL-DPA`, `-DCP`, `-DTD`, `-DTJ`, `-DCM` | DI Continuous Improvement / Process Analyst, Change Proposer, Trial Designer, Trial Judge, Capability Mentor | pass | pass | pass |

No code of this blueprint uses the suffix `DI` alone, so no part can be read as the AIOC itself.

---
## Annex A. The launch package and the service records: their parts and field lists

Every part is a versioned, content-addressed object. Every element carries an ID, its provenance (`stated`, `inferred`, `unresolved` or `assumed`, as in TOM Annex B, carried), its basis (design element IDs and source atom IDs, at least one) and, after T4, its decision reference. JSON Schemas are made from these lists before the first run and may add nothing.

**A.1 Design map** (run record, summarised in the package). Mode A: one row per element in scope: `element_id`, `part`, `state` (`used`, `returned`, `out of scope`), `return_id`, `reason`, `priority` (as the release decided it, or none). The value case carried (**New** in v0.1.2): per entry of the TOM Release's value case, `entry_id` (`VC-n`), `outcome_ref`, `measures` (each with its baseline and target references, or `unknown` and `not set`, as the release states them) and `elements`, by reference, unchanged. Mode B: one row per element of the outside design: `source_atom`, `read_as` (process, step, decision, position, unit, forum, policy, measure), `maps_to` (an ID in this map's own structure), `state` (`mapped`, `not mapped`, `out of scope`), `reason`.

**A.2 Gap report** (package part). Per check: `check_id` (Annex F), `tier`, `result` (`met`, `gap`, `unknown`), `evidence`. Per gap: `gap_id` (`GAP-n`), `check_id`, `tier` (`blocking`, `completeness`), `elements`, `consequence`, `evidence`, `proposed_fix`, `route` (`return` with its ID; `decision` with its row; `prepare` with the S3 output that answers it), `state`.

**A.3 Health check** (package part; in the service, a record each quarter). Per item: `item_id`, `heading` (strategy, structure, processes, measures, rhythm, controls), `question`, `result` (`met`, `not met`, `unknown`), `evidence`. A summary per heading, counts only. In the service (**New** in v0.2.0): `run` (`entry`, or the quarter) and, per item, `earlier` (its results in the organisation's own earlier checks). Never a person, and never another organisation.

**A.4 Procedures** (package part; one per process). `procedure_id`; `process_id`; `version`; `owner_position`; `steps[]`: {`step_id` (the process step it traces to), `position`, `instructions`, `form_or_template` (IDs), `record_left`, `done_when`, `worst_error`, `controls`}; `forms_and_templates[]`: {`id`, `name`, `fields` (position placeholders only)}; `citations`.

**A.5 Briefs** (package part). Per brief: `brief_id` (`BRF-n`); `kind` (`policy`, `pay structure`, `contract and offer templates`, `authority instruments`, `obligations register`, `control matrix`, `systems, data and suppliers`); `entity`; `jurisdiction` (or `unknown`, then `outline only`); `serves` (design element IDs); `what_it_must_achieve`; `known`; `open_questions`; `decisions_needed` (never an amount); `addressed_to` (a position code from `deciding_positions`); `mark` ("Draft, not legal advice"); `citations`. **Drafts** (**New** in v0.2.0): per draft: `draft_id` (`DRF-n`), `kind` (as for a brief), `template_ref` (the template's source and the counsel position's decision that approved it), `entity`, `jurisdiction`, `serves`, `text_ref`, `mark`, `addressed_to`, `reviewed_by` (the counsel position's review reference; a pay range carries it too), `citations`. **The cost draft:** `entity`; `jurisdiction`; `mark`; `lines[]` {`what`, `traces_to` (a position, a process or a need), `amount` {value, `source` or `decision`} or `not given`}; `totals`; `authority_check` (its result against the authority matrix); `addressed_to` (the finance position).

**A.6 Transition plan and go-live criteria** (package part). Plan: `waves[]` {units, processes, order, `priority` (the highest decided priority of what the wave starts), `departs_because` (when it departs from the order of priority)}; `cut_over[]` {step, position, rollback}; `parallel_run` (decided or none); `communication[]` {to position, what, when}; `consultation` {required by (per counsel), before which notice}; `review_chair` (position). Criteria: per criterion: `criterion_id` (`GLC-n`), `what_must_be_true`, `measure`, `evidence_source`, `threshold` (decision reference), `kind` (`blocking gaps closed`, `adoption`, `readiness`, other); `go_no_go_position`.

**A.7 Answer record** (run record). `question_id`; `asking_position`; `answer` or `I do not know`; `citations[]` {`element_id`, `version`, `span_sha256`}; `verifier` {engine family, result}; `sent_at`.

**A.8 Decision Package** (package part). A plain summary; the elements for decision, each with its deciding position and row; the blocking gaps and their routes; the unknowns, the assumptions and the open returns, in plain words; the review findings and their choices.

**The manifest.** `package_id` (`DIP-` + SHA-256 of the manifest body); `run_id`; `mode`; `design` {PPD and TOM release IDs and manifest hashes, or the outside design's source reference}; `parts[]` {name, sha256}; `input_packs[]`; `returns[]` (return IDs with their end states); `decided_at`; `final_status`.

**A.9 Implementation plan** (service record; **New** in v0.2.0). `plan_id`; `version`; `tasks[]` {`task_id` (`TSK-n`), `what`, `owner_position`, `depends_on` (task IDs), `date`, `traces_to` (a wave, a cut-over step, a gap route or a criterion of the launch package), `state` (`open`, `done`, `late`, or `dropped` with its decision)}; `milestones[]` {`id`, `date`, `date_changes[]` {`from`, `to`, `approved_by` (the review chair's decision reference)}}; `decided_by` (decision reference).

**A.10 Change impact and stakeholder register** (service record). Per position: `position_id`, `changes[]` {`kind` (`process`, `system`, `tool`, `role`, `reporting line`, `location`), `from`, `to`, `traces_to`}. Stakeholder register, per entry: `stakeholder` (a position code, or an outside party by kind), `affected_by`, `communication` {what, when, by which position}. Briefings, per manager position: `units`, `what_changes`, `when`. Adoption measures, per critical process: `process_id`, `measure` ("completes critical work unaided"), `source`, `threshold` (decision reference).

**A.11 Learning path** (service record). `path_id`; `position_id`; `version`; `rests_on` (the job description and procedure versions); `items[]` {`item_id`, `kind` (competence, step, decision), `traces_to`, `material`, `check` {question, expected}}. There is no field for a result.

**A.12 Readiness record, rehearsal scripts and defect log** (service records). Readiness, per criterion: `criterion_id`, `state` (`met`, `not met`, `unknown`), `evidence` (source reference and the time it was read). Rehearsal script: `script_id`, `process_id`, `position`, `steps[]` {`step_id`, `action`, `expected` (the step's `done_when`)}. Defect: `defect_id`, `script_id`, `step_id`, `what`, `severity`, `owner_position`, `state`.

**A.13 Go or no-go package and stabilisation record** (service records). Package: the state of each criterion with its evidence; the open defects; the open blocking gaps with their decisions; the risks of going and of not going, in plain words; `deciding_position`; `decision` (the signature record's reference, type `accept-irreversible-risk`). Rollout health view: the plan, the criteria, the defects and the problems, by process and unit. Stabilisation: per stabilisation criterion, as for readiness; `ended_by` (decision reference).

**A.14 Operating rhythm, logs and quarterly priorities** (service records). Rhythm, per forum: `forum_id` (from the decided design), `tier`, `cadence`, `chair`, `members`, `reviews`; during launch, the weekly review and its `chair`. **Action log:** `action_id`, `what`, `owner_position`, `date`, `from` (a forum's meeting or a record), `state`. **Risk and issue log:** `id`, `kind` (`risk`, `issue`), `what`, `owner_position`, `date`, `effect`, `state`. **Dependency register:** `id`, `from`, `to`, `owner_position`, `date`, `state`. **Decision log:** `decision_id`, `what`, `decided_by` (position), `date`, `forum`, `register_ref` (the entry in the Operations Event Register, where one exists). **Lessons:** `id`, `at` (a phase close or a trial end), `lesson`. **Quarterly priorities**, per position and quarter: `priority_id`, `position_id`, `quarter`, `what`, `tied_to` (a measure or an initiative), `inserted_by` (the position's act).

**A.15 Forum pack and minutes** (service records). Pack: `pack_id`, `forum_id`, `meeting`, `agenda` (decided by the chair), `pre_reads` (record references by version), `measures` (dashboard references), `log_extracts`. Minutes: `minutes_id`, `pack_id`, `text_sha256`, `preview_approved_by` (the participant positions' acts), `entered_at`. Rating, per meeting: counts per point of the scale, rolled up into the forum's quarter where fewer than `min_group` positions rated it; never per participant.

**A.16 Measures and dashboards** (service records). Per measure: `measure_id`; `process_id` or `unit_id`; `step_id` or none; `definition`; `unit`; `source`; `target` (decision reference, or `not set`); `level` (`process`, `step`, `unit`); `positions_count` (at least `min_group`, or `rolled_up_to` the parent unit). Per dashboard figure: `measure_id`, `value`, `read_at`, `source_ref`. Adoption funnel, where switched on: per step, counts that entered and completed, aggregated.

**A.17 Version register, acknowledgements and checklist runs** (service records). Version register, per element: `element_id`, `kind` (process, procedure, policy, job description, forum), `version`, `owner_position`, `approved_by`, `re_approval_due`, `status` (`verified`, `due`), `filed_ref`. Acknowledgement: `version_ref`, `position_id`, `acknowledged_at`; the sign-in behind it is held at the gateway only. Checklist run, per case: `case_id`, `procedure_ref` (its version), `gates[]` {`gate`, `approved_by` (a position's act at the gateway)}, `trail`, `in_flight_rule` (as applied).

**A.18 Problem record and issue list** (service records). `problem_id` (`PRB-n`), `reported_by` (position code), `process_id`, `step_id`, `statement`, `evidence`, `cause`, `options[]` {option, trade-offs}, `recommendation`, `deciding_position`, `decision` (reference), `actions` (action IDs). Issue list, per forum: `problem_id`s in order, each with its `effect` on the process and its measures.

**A.19 Initiative and value register** (service record). Per initiative: `initiative_id` (`INI-n`), `what`, `owner_position`, `from` (a value-case entry `VC-n`, a plan task or a proposal), `baseline` {value, source, read_at} or `unknown`, `benefit_class`, `value_by_month[]` {month, planned, realised, source}, `gate` (`L0` to `L5`), `gate_decisions` (L2 and L5, by the finance position), `attribution`, `warnings[]` {rule, what, at}. Reports: value leaking between gates; the pipeline's coverage of the target.

**A.20 Light design** (mode C; run record, then package part). `decision_list[]` {`decision`, `decider` (position), `limit` or `not given`, `state` (`provisional`, or its decision reference)}; `process_checklists[]` {`process`, `steps[]` {step, position}, `state`}; `who_does_what[]` {position, steps}; `weekly_rhythm` {forum, chair, standing items}; `solo_note` (where one position holds every seat: the statement, and the compensating control offered as a draft); `growth_triggers` (decided); `briefs_needed` (texts with legal effect, for counsel). Every element carries its source atoms or its decision reference.

**A.21 Conformance record and findings** (service records). Conformance, per process and period: `process_id`, `rate`, `deviations[]` {`type`, `step_id`, `count`, `dimension` (step, case type, site, system), `accepted` (its entry on the accepted-deviation list, or none)}. Accepted-deviation list: `deviation`, `decided_by` (the process owner position), `times_accepted`. Finding: `finding_id` (`FND-n`), `kind` (`bottleneck`, `overload`, `rework`, `control gap`), `process_id`, `steps`, `unit` (where at unit level), `evidence`, `positions_count` (at least `min_group`), `method_ref` (a pinned reference model used as a method, or none).

**A.22 Proposal** (service record). `proposal_id` (`PRP-n`), `kind` (process, position, job description, forum, new process), `trigger` (a finding, a deviation, a problem, a change notice or the reassessment; by reference), `evidence`, `expected_effect`, `risk`, `to` (the deciding position, or a return ID), `as_trial` (yes or no), `decision`, `version_made` (the living design version, once decided).

**A.23 Trial record** (service record). `trial_id` (`TRL-n`), `proposal_id`, `process_id`, `change`, `expected_result`, `guardrail_measure`, `duration`, `rollback_trigger`, `default`, `decided_by` (before the start), `baseline_points`, `method` (`run chart`, or `plan-do-study-act`, labelled "judgement, not proof"), `side_by_side` (where two teams or sites exist), `judge` {Cell, engine family}, `judgement`, `outcome` (`adopt`, `adjust`, `roll back`; decided by the process owner position), `lessons`.

**A.24 Hand-over and drill records** (service records). Each quarter: `only_di_can_produce[]` {output, hand-over plan, learning path reference}. Drill: `drill_id`, `period`, `export_ref`, `di_stopped` {from, to}, `what_ran`, `what_failed`, `decided_by` (the Cell carrying `[ORG]HOAC-TM`), `result` (`passed`, `failed`).

**A.25 Export manifest.** `export_id` (`DIX-` + SHA-256 of the manifest body); `records[]` {kind, id, version, sha256, format}; `traces` (every artefact to its design element, deciding position and decision); `reimport_check` {instance, result}.

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

**C.1 Run states.** As §5.0. Endings other than a filed package: `closed: not admitted` (T0 failed, each failed condition named); `closed: non-response`; `closed: rejected`; `closed: withdrawn by the Requesting Authority`. Flags on any state, each with its age: `waiting`; `waiting: ruling`; `held: return open` (on the touched elements only); `held: material finding`; `held: connection revoked`; `held: no reviewers`; `held: review budget`; `stopped`. No flag releases the run slot; every ending releases it. **The service** (**New** in v0.2.0): `accompanying` → `stabilised`; `operating` and `improving` are standing. It ends only as `closed: by the Requesting Authority`. Its flags: those above, and `waiting: decision` (a row waits for its position); `held: Annex H not met` (process watching only); `stopped: drill` (while the drill runs); `rolled back` (on a change, with its reference).

**C.2 The gates.** T0 to T5 as in §5.0. A gate passes only on its settled review (§5.9) and its done-test. T0 has these conditions: (a) the run request carries references only; (b) its mode is in `modes_enabled`; (c) mode A: the release check passes for the PPD Release and the TOM Release it names; mode B: the outside design is a source held in Source Lifecycle; (d) the connections are signed and in scope; (e) the engine register holds eligible engines for the highest confidentiality level in scope, of two families; (f) `requesting_authority_cell` and `deciding_positions` are set; (g) RP0 is settled; (h) mode C only: `modes_enabled` holds C, after H-21. T1C and T6 to T10 are as §5.0; each passes only on its settled review and its done-test.

## Annex D. What this AIOC never does

1. Change, merge, split or drop an element of a design release, or rewrite an outside design.
2. Decide anything for the organisation, the go or no-go included, or take silence as a decision.
3. Give legal, tax, employment or pay advice, write a final legal text, or state an amount that no source or decision gives.
4. Ask any person anything about the organisation, or send a request that names a person.
5. Name a person, read who occupies a position, or prepare a named offer.
6. Rank, score or watch the occupant of a position, infer emotion, or show a measure for a single position.
7. Read records of the organisation's work outside the projection, or before Annex H holds.
8. Insert a draft into a live record, log or plan; apply a change outside a class signed at level 2 (Annex G).
9. Answer a question from outside the decided design, or send an answer or draft whose citation failed verification.
10. Mark a go-live criterion met on its own report.
11. Grade its own work: no Cell reviews its own output, and the Chief of Staff rules on nothing.
12. Act on a type of the Human Floor signature list, at any level.
13. Change a value case, or set a baseline, a target or a priority of its own (TOM blueprint `v0.6.0`, Annex H.6, H.7).
14. Keep, read or report a learner's check result.
15. Show a measure, finding or view for a single position, or one that rests on fewer than `min_group` positions.
16. Judge a trial it proposed or designed, or judge the drill.
17. Issue a statement or transition notice on the organisation's behalf to staff, authorities or customers; its own notices to positions about records are not such statements.
18. Propose a change to its own ladder, tests or measures of success.

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

## Annex G. The permission ladder

**New** in v0.2.0. As the product requirements set it (`PRD-[ORG]AIOC-DI-001` v0.4, the permission ladder), read with the Standard's Human Floor signature list.

| Level | This AIOC may | Examples |
|---|---|---|
| 0 · Read | read its connected sources, records of work through the projection (Annex H), and the design | watch a process; build a dashboard |
| 1 · Propose | draft and recommend; a draft enters a record, log or plan only when a position inserts it; nothing changes until a position decides | a procedure draft; a proposed change to a job description; draft minutes; a suggested quarterly priority |
| 2 · Apply within a standing approval | apply a change of a class the owner position signed in advance, only where it is reversible and has no legal, pay or employment effect; as a new version with rollback, reported the same day | refresh a dashboard's layout; reword an internal form that is not an HR or legal form; reschedule a review reminder |
| Never | no level allows it; the gateway refuses every type on the Human Floor signature list | sign; pay or commit money; hire, move or dismiss; be named owner or accountable; delegate authority or be named in a power of attorney or mandate; connect a new port; change a test, threshold, target or go-live criterion; mark a physical step done; issue statements to staff, authorities or customers; export or purge personal data; roll back outside a signed class; grant access; change its own permissions |

**Rules.**
1. **Per class.** The owner position sets each class's level; every class starts at level 1, and a read-only class at level 0.
2. **Moving up.** A class moves up one level only by the owner position's signed decision and a fixed-test score at or above its recorded threshold (§13, H-07).
3. **Level 2 is a signed class.** The owner position signs the class once as `sign-standing-action-class`, for reversible actions only (§13, H-18). It never covers any type of the Human Floor signature list.
4. **Dropping back.** Any error, complaint or change of engine drops the class to level 1 at once; the drop is recorded and reported to the owner position.
5. **Never.** A trial that changes a position or a job description never runs at level 2 (§5.23, rule 6).
6. **Who approves.** A process owner position decides changes inside its process, within its limits; a change that crosses processes or touches a position goes to the position the authority matrix names.
7. **Enforcement.** Inside an `[ORG]AION`, the tool gateway enforces the ladder and the stop. Standing alone, this AIOC's own gateway fails closed, with one negative case for every Human Floor type passed before each release.
8. **Over-trust.** Time-to-approve and approve-all rates are logged by class, and rubber-stamping is flagged to the owner position (NFR-03); neither is logged or shown by position.

**Default classes.**

| Class | Example | Default level | Highest level |
|---|---|---|---|
| Read the design and this AIOC's own records | — | 0 | 0 |
| Read records of work | through the projection, under Annex H | 0, only once Annex H holds | 0 |
| Draft | procedures, briefs, plans, packs, minutes, proposals, priorities | 1 | 1 |
| Dashboard layout | refresh a dashboard's layout | 1 | 2 |
| Internal form wording | reword an internal form that is not an HR or legal form | 1 | 2 |
| Reminder schedules | reschedule a review reminder | 1 | 2 |
| Anything with legal, pay or employment effect | a policy, a pay range, a contract template | 1 | 1 |
| A change to a position or a job description | — | 1 | 1 |
| A type of the Human Floor signature list | sign, pay, hire, connect a port, grant access | never | never |

## Annex H. Records of work: the projection and its conditions

**New** in v0.2.0 (FR-19, FR-39, FR-44; NFR-04, NFR-05; Protocol §20, item 7).

1. **Off by default.** `process_watching` stays off until every condition of rule 2 is recorded (§13, H-17). The rest of this AIOC runs without it.
2. **Before it is switched on:**
   - the data-protection position records an impact assessment for the records in scope, and a lawful basis other than staff consent;
   - workers or their representatives are informed, and consulted where the law requires it, as the counsel position confirms for each jurisdiction;
   - the projection is built and owned by the Cell carrying `[ORG]HOAC-TM`, and its connection is signed as `connect-external-port`;
   - the negative cases of rule 7 pass.
3. **The projection removes who did the work.** It passes records by process, step, case type, site and system. Every field that identifies a person or the occupant of a position is removed: author, assignee, approver, sender, user, device and the like. A record that cannot be cleared is refused whole, and this AIOC keeps nothing of it.
4. **Kept briefly.** Records of work are held by reference, and only as long as the cycle that uses them. Conformance records and findings keep counts, never the records.
5. **No figure for one position.** Every measure, finding and view is at process, step or unit level. A figure that would rest on fewer than `min_group` positions rolls up to the parent unit. Nothing is ranked, scored or allocated to any person, and no emotion is inferred.
6. **Not a high-risk employment system.** The provider documents why this AIOC is not one, or meets the duties of one where a law makes it so (NFR-05); counsel confirms for each jurisdiction.
7. **Negative cases, before use:** a record with a person field is refused; a question about one position over time is refused and recorded to the data-protection position; a figure on fewer than `min_group` positions rolls up; a stop reaches the projection's connection at once.
8. **Switched off** at once by a stop, by the data-protection position, or by revocation of the connection. Work in flight is held, never closed.
9. **The same rules** govern the adoption funnels of guidance at the point of work (§5.18, rule 5).

*Powered by 49GAION*
