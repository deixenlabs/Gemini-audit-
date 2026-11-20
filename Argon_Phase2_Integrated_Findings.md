# Argon Phase 2 — Integrated Findings, Evidence Corrections & Legacy Disposition

**Source contribution:** Gemini Argon 4, *DEIXEN — Phase 2: Targeted Full-Text Source Verification & Strategic Relevance Assessment*, dated 19 November 2026.  
**Status:** Independent reviewer findings; not founder approval, not implementation authorization, and not a Fable handoff.  
**Provenance note:** The founder pasted the contents of Argon's full report, 34-entry evidence ledger, and source-map addendum into the conversation. This document is a normalized integration summary of that supplied text. It is not a byte-for-byte reproduction of Argon's original three generated files, and ChatGPT did not independently rerun the repository inspection.

---

## 1. Inspection coverage reported by Argon

Argon reports that all required input groups were present: the November 11 repository ZIP, the seven-file Argon Phase 1 package, all three v2.5 working documents, and explicit founder clarifications.

Reported inspection coverage across 47 repository files:

| Coverage tier | Count | Meaning |
|---|---:|---|
| Full-text inspection | 16 | Entire text read, including Amadeus reference, task map, CP-001, practitioner brief, UX/product/brand documents, CSV, execution plan, CLAUDE.md, and D98 patch files. |
| Deep targeted inspection | 10 | Large/structured documents examined via complete headings/ID scans and selected full-text ranges or selected JSON structures; not claimed as complete line-by-line reading. |
| Metadata / structure / checksum only | 21 | Not substantively read in full. Includes historical and secondary materials. |
| **Total** | **47** | All repository entries accounted for at one of the stated inspection levels. |

Argon's detailed corrected count is 16 full-text, 10 deep-targeted, and 21 metadata/structural. An earlier draft count of 14 full-text files was corrected in Argon's self-review. The exact full-text list and targeted ranges are recorded in the pasted Phase 2 report; they should not be inflated into a claim that all 47 files were fully read.

Snapshot identity reported: `deixenlabs/DEIXEN-KNOWLEDGE`, ZIP comment SHA `0e2723cb4d62962888f8d5a0d79980e18036e57f`, uniform archive timestamp 2026-11-11 08:29:50. No `.git/` history was available; live GitHub state after the snapshot is unverified.

## 2. Governance and decision provenance

### 2.1 Decision ledger correction — PV-001

Argon corrected Phase 1's count of 85. Its full ID inventory reports:

- 86 consecutive dated integer decisions D12–D97.
- 7 earlier numbered thematic decisions: D6, D7, D8A, D9, D10, D10A, D11.
- Total: **93 uniquely numbered decision identifiers**.
- 11 unnumbered thematic baseline rules/contracts.
- D93 at line 4039 was missed by the initial regex because its bullet had leading whitespace.
- Pure integers 1–5 and plain D8 are absent; D8A is present.
- Latest directly evidenced decision date in the two registers is 2026-10-28 (D97).

Do not describe all 93 IDs as active. Some are superseded or historical. This is an ID inventory, not an active-decision count.

### 2.2 Decisions and their current relevance — PV-002–PV-008, PV-010

| Finding | Historical source result | Current treatment for the working package |
|---|---|---|
| PV-002 — D7 / D12 | D7 was superseded by D12, the Amadeus verification standard. | Carry forward D12's no-invention and source-verification discipline; do not revive D7's superseded formulation. |
| PV-003 — D18 | Basic and Advanced Amadeus curriculum ambition for Saudi/Gulf entry-level work, with dated job-posting evidence. | Carry forward; do not shrink DEIXEN's ambition to Slice 1. |
| PV-004 — D91 | Kit v0.3 visual identity was historically approved. | Superseded/withdrawn by later v2.5 objectives/inventory and explicit founder clarification. Do not carry old logo, mark, tokens, or color rules into the new baseline. |
| PV-005 — D92 | Scenario Bank is a case page/library; scenario execution is a mode inside Terminal. | Carry forward as a product boundary. |
| PV-006 — D93 | Argon historically appointed Project Lead in the 2026-10-25 ledger. | Historical and superseded by the current Argon → Claude → consolidation → founder-authorized Fable route. |
| PV-007 — D96 | F-08 lesson strings L01-AN–L10-FQD were accepted; archive EN/AR JSON hashes reportedly match D96. | Preserve as historical Slice 1 lesson baseline, not proof of live app or complete curriculum. |
| PV-008 — D97 | Cumulative Ghost via real simulator on isolated demo booking, no state injection; separate clean independent assessment attempt. | Carry forward as a core demonstration/assessment-integrity safeguard; verify implementation separately. |
| PV-010 — Stage 147 | Not found in the November 11 snapshot; later appears in Workflow v2.4 and founder context. | Preserve the later founder-approved eligibility correction behavior. Snapshot absence does not invalidate later approval. |

### 2.3 D98 collision — PV-009

Two 2026-11-06 unapplied patch files both claim Decision 98:

- `D98 — Governance Insertions.md`: Home/الرئيسية and Learning direction.
- `DEIXEN_Dual_Tool_Design_Role_Amendment_Patches.md`: dual-tool visual-design collaboration roles.

Argon reports neither patch was merged into `07_DEIXEN_Canonical_Decisions_and_Current_State.md` nor `13_DEIXEN_Decision_Resolution_Register.md`; both ledgers contain zero D98 mentions. Some later framework files reference Home as D98, and four files mark the collision unresolved.

**Disposition: UNRESOLVED / requires founder confirmation if the formal historical numbering must be reconciled.** Do not choose a winner based on file name/date, and do not let the unresolved collision block unrelated product development. The dual-tool role assumptions are also superseded by the later Fable-led plan unless the founder explicitly reopens them.

### 2.4 Governance rules: keep safeguards, retire obsolete restrictions — PV-030

Preserve legitimate safeguards:

- Founder-reserved authority (D29 / Constitution §8).
- D12–D13 Amadeus source discipline and no-invention.
- Role ≠ model; recommendation ≠ decision; implementation ≠ domain validation; design intent ≠ demonstrated effectiveness.
- Evidence honesty and explicit uncertainty.
- Privacy, accessibility, and no-false-affordance principles.

Do not let obsolete rules constrain current development merely because they remain in old files:

- Old Constitution §9 / Execution Plan rules excluding Sonnet/ChatGPT or waiving independent review.
- Historical permanent Argon leadership language from D93.
- `CLAUDE.md` Slice-1-only freezes, old Kit v0.3 token hashes, and dependencies on absent `design/phase4/` or `design/identity/` paths.
- Historical Execution Plan file-creation freeze.

Recommendation only: revise or archive obsolete operating instructions after consolidation and founder authorization. No cleanup is performed by this package.

## 3. Amadeus operational truth and EV-01 — PV-011–PV-015

### 3.1 Critical method limitation — PV-011

`DEIXEN_Amadeus_Verified_Reference.md` explicitly says Service Hub blocks automated full-page reading. Argon reports V-01–V-18 rely on search-result snippets plus selected PDFs/re-hosted quick cards, not full official manual review or live Cryptic testing.

Therefore “VERIFIED” inside that reference is bounded by the source/method described there. It must not be inflated into full-manual or live operational verification.

### 3.2 Operational boundaries

| Topic | What Argon reports the reference supports | What remains unverified / must not be assumed |
|---|---|---|
| AN / FQD discovery | Bounded snippet support for flight and fare display concepts. | Several result/header interpretation details remain under U-items; do not invent display interpretation. |
| SS provisional sell | Bounded support for short/long sell and segment reservation behavior. | Carrier-side timing, waitlist/rejection status semantics, and inventory reversibility need further evidence. |
| FXP / FXX | FXP creates/stores a TST; FXX prices without storing a TST, under the reference's bounded evidence. | Full workflow context and exact persistence behavior still require EV-01. |
| RF | V-10 snippet says a PNR cannot be filed unless RF is present; RF is the Received From PNR element. | RF is not customer consent. Do not claim universal positioning or extra rules without authority. The slice handler accepting any non-empty string is not semantic validation. |
| ER / ET | Reference distinguishes ET (end transaction) from ER (end and redisplay). | Do not assume they are interchangeable or invent a universal order. |
| IG / XE | Not verified in the reference; off-path recovery remains open in the resolution register. | Do not teach or depend on IG/XE recovery until EV-01 verifies it. |
| TST after ER → FXP | Not established. | U-05 explicitly remains unverified whether the TST created after ER needs another ER/ET to persist. |
| Contact SSR / AP | U-12 contact SSR suffix and U-14 AP=PRINT Phone remain unverified. | Do not teach as facts or move them into practitioner gate closure. |

**EV-01 remains OPEN.** It requires authoritative full-manual / training-book / qualified verification for snippet-bounded claims and unresolved U-items, including U-05, U-12, U-14, IG/XE, SS semantics, and the precise ET/ER and FXP/FXX boundaries.

### 3.3 EV-01 vs EV-02 boundary correction — PV-020

Argon corrects its earlier handoff: U-12 and U-14 belong under **EV-01**, not EV-02. EV-02 is the external practitioner review of PR-CP-001's 12 professional-practice questions. Practitioner review cannot close D12 command/reference gates.

## 4. First task, CP-001, semantic validation, and EV-02 — PV-016–PV-020

### 4.1 Pre-selected itinerary nuance — PV-016

The 08 Task Map and CP-001 intentionally start with a customer who has already selected synthetic flight 6X 403. In this bounded case, AN locates the pre-selected flight's line; the case excludes broad live search, recommendation, and fare comparison. Do not generalize this pre-selected itinerary design to all future tasks: non-preselected tasks may still require discovery and quotation before advice or confirmation.

### 4.2 Task objects — PV-017

The earlier 08 Task Map uses three objects and describes Task Run as one learner's attempt. Workflow v2.4 separates five objects:

1. Case Package.
2. Scenario Variant.
3. Task Run — mutable execution context.
4. Attempt — formal opportunity and evidence record.
5. Operational Session.

Treat the five-object model as the current working model, with approval status preserved. Do not collapse Task Run and Attempt.

### 4.3 Semantic validator gap — PV-018

CP-001 documents a read-only historical handler inspection:

- `rf.ts` accepts any non-empty text and rejects a second RF.
- `fxp.ts` marks task completion when the PNR is filed and FXP occurs.
- `ss.ts` rejects a wrong flight/class against the fixture.

The reported issue is that engine acceptance can still be professionally/task-semantically wrong. A case-level semantic validator must test the requested customer facts and requester/consent requirements, not merely rely on technical handler acceptance.

This is a reported historical code observation, not proof of current app repository state. `deixen-app`/`deixen-app1` require a separate authorized read-only app audit.

### 4.4 CP-001 disposition — PV-019

CP-001 explicitly says it is a working case candidate, not approved for production content or implementation. Its self-verdict is `تنجح مع تعديل` (pass with modifications), with content release on HOLD pending, among other items, operational verification, semantic validation, safe RF recovery, and practitioner review.

### 4.5 Practitioner review — PV-020

PR-CP-001 is “READY TO SEND — REVIEW NOT YET PERFORMED.” It contains 12 professional-practice questions and Gulf context. It cannot close U-12/U-14 command-reference issues.

**EV-02 remains OPEN.** It requires an actual qualified practitioner review; the existence of a review form does not constitute validation.

## 5. Product, UX, runtime, learning, and validation — PV-021–PV-027

### 5.1 Product and runtime architecture

Argon reports convergence around:

- Five top-level areas: Home, Learning, Terminal, Scenario Bank, Growth; final Home vs Flight Deck naming remains open.
- Terminal centrality; Scenario Bank is a case library and scenarios execute inside Terminal (D92).
- Three lifecycles: Customer Journey, Professional/Learner Journey, Work Task Lifecycle.
- Frontend-first with clean seams for later Backend; this does not cancel Backend.
- Task Runtime as a lightweight coordinator, not a monolithic mega-engine.
- Recorded evidence is persisted; calculated state is derived from recorded evidence where appropriate.

`06 — DEIXEN Unified Experience & Runtime Architecture.md` is explicitly a working proposal, not a canonical approved architecture or implementation authorization. It reports an earlier app snapshot that did not satisfy D97 (session/task reuse and exposed hints); documentation of D97 does not prove implementation conformance.

An unresolved UX gap remains: dialogue-heavy / customer-service-only cases within Terminal Scenario Mode without forcing irrelevant command-entry UI.

### 5.2 Learning and competence maturity

Argon reports that `06_DEIXEN_Canonical_Curriculum_and_Coach.md` preserves useful curriculum seeds and rules:

- D18 Basic & Advanced Gulf-relevant curriculum ambition.
- Five-lesson Customer Service track seed, including an Anger Meter and Terminal/English integration, but gated pending its own contract.
- Ghost's structured demonstration schema.
- No absolute CPM benchmark for Speed Drills without booking-office evidence.
- Coach should preserve the engine's error verbatim alongside a side-by-side explanation.

LDS and LEA remain draft/non-canonical documents, useful as selective pedagogical references rather than binding specifications. The competence foundation distinguishes ambition, capability, demonstrated learning, validated competence, workplace outcomes, and external recognition.

The founder's first-learner journey is meaningful but is not enough by itself to validate usability or learning effectiveness for other beginners.

### 5.3 Evidence backlog — PV-027

Argon reports 48 CSV backlog rows across 15 workstreams and maps them to existing EV-01–EV-06 without creating extra gates:

- EV-01: Amadeus operational truth.
- EV-02: practitioner realism and professional practice.
- EV-03: job-task analysis and P1/P2 curriculum map.
- EV-04: genuine beginner usability and learning effectiveness.
- EV-05: assessment isolation, transfer, and variant comparability.
- EV-06: market/employer/commercial/partnership validation.

Additional governance/legal/quality items (GOV-01–GOV-05, LEGAL-01/02, QA-01, AI-01, VALID-01/02) are backlog concerns, not new OD or EV identifiers. Preserve exactly OD-01–OD-08 and EV-01–EV-06.

## 6. Visual identity and design system — PV-028–PV-029

Argon reports:

- The November 11 snapshot still contains `04_DEIXEN_Canonical_Design_System.md`; it was updated only through D80–D81, not D91.
- D91 Kit v0.3 was historically approved, but later v2.5 Objectives §5, Inventory §8.1–8.2, and founder clarifications withdraw the old visual identity for current/future use.
- `03 — DEIXEN Product Design Language.md` and `04 — DEIXEN Brand Strategy & Visual Identity.md` explicitly say no final logo, wordmark, palette, accent color, typography, component library, or screen composition is approved.
- The absent `DEIXEN_Identity_Closure_2026-10-22.md` cannot be reconstructed from its reference.
- The old design-system file mixes withdrawn visual execution with durable non-visual principles: WCAG 2.1 AA, responsive breakpoints, anti-patterns, and localization/accessibility guidance.

**Disposition:** do not inherit the old D91 logo/mark/tokens/visual decisions. Extract only useful non-visual accessibility/responsive principles into a clean current standard. Keep the new identity open for a separate future exploration, not as a blocker to the functional product.

## 7. Legacy source dispositions — PV-030–PV-031 and source-map addendum

### 7.1 Carry forward as current principles or useful requirements

- D12/D13 operational truth and no-invention discipline.
- D18's broader Basic/Advanced curriculum ambition.
- D92 Scenario Bank / Terminal boundary.
- D97 Ghost and independent assessment integrity.
- Founder reserved authority and evidence discipline.
- Non-visual WCAG 2.1 AA, responsive breakpoints, and anti-pattern guidance, rewritten cleanly without the old visual system.
- Useful curriculum/Coach/Ghost concepts, validation framework, CP-001 structure (after corrections), and the five-object runtime model.

### 7.2 Keep as historical context, not binding current requirements

- Full 07/13 decision ledgers except specifically retained principles.
- Older Slice 1 `slice.json`, lesson strings, and build specifications.
- LDS/LEA learning drafts.
- Strategic product direction, Part XIX, commercial hypotheses, and prior external competence review, where newer current references now govern.
- Old UX or architecture proposals that remain useful as reference but need reconciliation.

### 7.3 Revise or supersede

- `03_DEIXEN_Canonical_Product_and_Architecture.md`: retain durable product principles, sync D98/Home references, detach withdrawn design-system dependencies.
- `06_DEIXEN_Canonical_Curriculum_and_Coach.md`: retain Coach/Ghost/CS safeguards; expand curriculum using sourced P1/P2 job tasks, not an old course list.
- Constitution / AI working rules: retain authority and epistemic safeguards; revise obsolete model assignments or tool exclusions.
- `02 —`, `06 —`, `07 —` working proposals: reconcile with current v2.4 model and explicit founder direction before treating any as authoritative.
- CP-001: retain as valuable candidate; fix semantic validator, safe recovery, unresolved Amadeus facts, and practitioner review before release.

### 7.4 Candidate for archival or removal from active workspace

These are Argon's recommendations, not approved deletion instructions:

- Old `CLAUDE.md` Slice-only freezes and withdrawn token references.
- Historical Execution Plan constraints that freeze current work or obsolete model roles.
- `DEIXEN Detour Prompt Package v1.8.MD`.
- Outdated consolidation plan with many absent legacy references.
- Misplaced root README that documents only a four-file subpackage.
- Unadopted AI-collaboration v0.2 proposals that predate the Fable-led plan.
- Broken navigation/index artifacts after their useful content is replaced.

Before any deletion, determine whether useful historical or audit evidence must be retained in an archive and obtain founder authorization.

## 8. Corrections that must override earlier Argon Phase 1 wording

| Earlier Phase 1 issue | Phase 2 correction to use |
|---|---|
| Decision count was stated as 85 | Use 93 unique numbered identifiers with the exact breakdown in §2.1. |
| U-12/U-14 were placed under EV-02 in earlier wording | U-12/U-14 belong to EV-01. EV-02 covers the 12 PR-CP-001 practice-review questions. |
| `ER` and `ET` grouping could imply equivalence | Explicitly keep ET and ER distinct; no interchangeability assumption. |
| Phase A–D was used for both review and product-development phases | Always qualify Review Workstream A–D vs Product Development Phase A–D. |
| Pilot protocol preparation / variant creation could appear to close gates | Pilot build readiness, pilot execution, pilot validation, and phase-exit evidence are separate milestones. EV-04/EV-05 require real evidence. |
| CP-001's pre-selected itinerary might be generalized | It is a deliberately bounded pre-selected-flight case; general tasks may require prior discovery/quotation. |
| “Ready for Fable” language appeared in older drafts | Fable remains locked until Claude's independent work, consolidation, and explicit founder authorization. |

## 9. Current open items — retain identifiers

### Owner Decisions

OD-01–OD-08 remain the existing owner-decision set. Preserve their original definitions and provenance. Phase 2 did not create additional ODs.

### Evidence Gates

Argon reports all six remain open:

- EV-01: authoritative Amadeus verification.
- EV-02: actual qualified practitioner review of PR-CP-001.
- EV-03: P1/P2 curriculum and job-task mapping.
- EV-04: genuine beginner usability and learning tests.
- EV-05: empirical transfer and variant comparability.
- EV-06: regional employer/commercial/partnership validation.

### Other unresolved items (not new ODs/EVs)

- D98 numbering/source reconciliation.
- Final Home vs Flight Deck naming.
- Customer Service-only scenarios inside Terminal Scenario Mode.
- Missing `DEIXEN_Identity_Closure_2026-10-22.md` and D95/D96 v1.5 lesson standard.
- `standards/README.md` and absent design/ directories referenced by old docs.
- Application repository identity/state (`deixen-app` vs `deixen-app1`) — separate authorization required.
- LEGAL-01 Amadeus IP/trademark and LEGAL-02 privacy/data/voice handling review.
- Clean current governance charter and documentation navigation.

## 10. PV-001–PV-034 evidence index

The companion file `ARGON_PHASE2_EVIDENCE_TRACEABILITY_LEDGER.md` preserves the detailed PV-001–PV-034 claims, source paths, section/decision anchors, line ranges, reported verification statuses, handoff impacts, Fable relevance, and remaining evidence as reconstructed from the complete ledger text pasted by the founder. This is a normalized transcription, not a byte-identical export from Argon's environment.

| Finding ID | Topic | Core conclusion / correction |
|---|---|---|
| PV-001 | Decision ledger count | 93 unique numbered IDs; Phase 1 missed D93 leading-space bullet. |
| PV-002 | D7 / D12 Amadeus standard | D7 superseded by D12; keep the stronger evidence discipline. |
| PV-003 | D18 curriculum goal | Basic + Advanced Gulf-relevant curriculum ambition remains useful. |
| PV-004 | D91 visual identity | Historically approved but later withdrawn; do not inherit old identity. |
| PV-005 | D92 Scenario Bank | Scenario Bank is case library; execution belongs in Terminal. |
| PV-006 | D93 Project Lead | Historical Argon lead appointment superseded by current sequence. |
| PV-007 | D96 beginner lessons | Archive EN/AR lesson files reportedly match D96 hashes; Slice 1 baseline only. |
| PV-008 | D97 Ghost and assessment | Preserve isolated Ghost demonstration and independent assessment safeguards. |
| PV-009 | D98 numbering collision | Two unapplied D98 patches; unresolved; founder confirmation if formal reconciliation required. |
| PV-010 | Stage 147 provenance | Absent from snapshot but remains later founder-approved direction. |
| PV-011 | Amadeus reference method | Service Hub snippet limitation reduces verification strength. |
| PV-012 | RF / ET-ER / FXP-FXX | Preserve distinctions; RF is not customer consent; bounded snippet evidence. |
| PV-013 | ER→FXP TST / U-12–U-16 | U-05, U-12, U-14 and others remain unverified. |
| PV-014 | IG/XE recovery | Not verified; off-path recovery remains open. |
| PV-015 | slice.json rules and tasks | Slice confirms historical fixture and semantic RF gap; not real carrier data. |
| PV-016 | Pre-selected itinerary | CP-001 deliberately starts with selected 6X 403; do not generalize to all tasks. |
| PV-017 | Task Run vs Attempt | Workflow v2.4 separates five objects; use distinct lifecycle concepts. |
| PV-018 | Semantic validator gap | Engine acceptance is not professional/task correctness; add case-level semantic validation. |
| PV-019 | CP-001 release hold | Working candidate, pass with modifications, content HOLD. |
| PV-020 | PR-CP-001 / EV-02 | Practitioner review not performed; does not close U-12/U-14. |
| PV-021 | Five areas / Home naming | Five-area structure and frontend-first seams; D98 Home sync remains open. |
| PV-022 | Runtime proposal / app D97 gap | 06 — is proposal only; documented prior app did not satisfy D97. |
| PV-023 | Three lifecycles / CS scenario gap | Distinct lifecycles; CS-only flow in Terminal Scenario Mode remains open. |
| PV-024 | Curriculum / CS / Coach / Ghost | Preserve useful CS, Coach, Ghost, and Speed Drill rules; expand curriculum. |
| PV-025 | LDS / LEA authority | Both are draft/non-canonical pedagogical references. |
| PV-026 | Competence foundation | Keep six-tier distinction between ambition and proven outcomes. |
| PV-027 | Validation backlog | 48 rows map to existing EV-01–EV-06 and legal/governance concerns. |
| PV-028 | Visual vs non-visual design system | Withdraw old visuals; salvage accessibility/responsive principles. |
| PV-029 | Open brand framework | No final logo, wordmark, palette, typography, or composition approved. |
| PV-030 | Obsolete governance / slice freeze | Revise obsolete model exclusions, scope locks, token dependencies, and freezes. |
| PV-031 | README/index/path mismatches | Historical navigation defects; replace with a clean current index before archival. |
| PV-032 | Phase A–D naming collision | Qualify review workstreams vs product development phases. |
| PV-033 | Pilot readiness vs validation | Pilot build/protocol/variants do not prove EV-04/EV-05. |
| PV-034 | Case Briefing vs Coach | Keep neutral factual briefing separate from guidance and answer leakage. |

## 11. External and technical evidence still pending

- The application repositories were not inspected during Phase 2. A separate authorized read-only app audit is needed before implementation claims or engineering tickets are locked.
- The external Amadeus training book PDF was not inspected; authoritative Amadeus verification remains EV-01.
- PR-CP-001 has not been conducted; EV-02 remains open.
- Beginner learning/usability and variant transfer trials remain open (EV-04/EV-05).
- Employer, regional, commercial, and partnership validation remain open (EV-06).
- Legal/IP/privacy review items remain open in the backlog.
- Claude's independent contribution remains pending as of the supplied Phase 2 checkpoint.

## 12. Safe use in later consolidation

Treat Phase 2 as a strong independent evidence contribution. Before using a result as a current requirement:

1. Confirm its exact status in the current founder context and v2.5 working baseline.
2. Check whether Phase 2 corrected earlier Argon wording.
3. Preserve whether the evidence was direct, cross-source, snippet-bounded, targeted, or merely metadata-level.
4. Keep source-backed facts separate from Argon's recommendations and founder decisions.
5. Preserve unresolved disagreement for Review Workstream C rather than forcing consensus.
6. Do not activate Fable or edit repository files during this stage.
