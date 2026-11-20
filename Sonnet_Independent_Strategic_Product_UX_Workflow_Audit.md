# DEIXEN — Independent Strategic, Product, UX & Workflow Audit

Claude Sonnet 5.5 · Second independent reviewer · Nov 18, 2026 · Prepared for @Adam

*Status: advisory findings and proposed alternatives only. Nothing in this report is a project decision until the owner explicitly agrees to it.*

## 1. Reading and Coverage Confirmation

All three core documents were read completely, in the required order, and no repository or application code was inspected. This is a documentary, product, UX and workflow review. Nothing in it is a decision.

**Reviewer:** Claude Sonnet 5.5, second independent reviewer. **Review date:** 2026-11-18 to 2026-11-20.

### 1.1 Files read

| # | File (exact name) | Short code | Lines | Read |
| --- | --- | --- | --- | --- |
| 1 | DEIXEN\_Objectives\_and\_Founder\_Goals\_Reference\_v0.2.md | D1 | 427 | Complete, first |
| 2 | DEIXEN\_Product\_Feature\_Ideas\_Inventory\_v0.2.md | D2 | 852 | Complete, second |
| 3 | DEIXEN\_UX\_Workflow\_Proposal\_Register\_v2.4.md | D3 | 1,561 | Complete, third (Stages 1–155 as the file records them) |
| 4 | README\_Review\_Handoff.md | README | 75 | Complete, after the three core files |
| 5 | SONNET\_5.5\_INDEPENDENT\_AUDIT\_BRIEF.md | Brief | 336 | Complete, after the three core files |
| 6 | SONNET\_REVIEW\_REPORT\_TEMPLATE.md | Template | 180 | Complete, after the three core files |
| 7 | START\_HERE\_PROMPT\_FOR\_SONNET\_5.5.txt | Start-here | 22 | Complete, after the three core files |
| 8 | SHA256SUMS.txt | – | 7 | Complete |

Anchors in this report use D1, D2 and D3 with section (§) and stage numbers. “D3 Stage 141” means the Stage 141 text in D3. Every short code stands for the exact file name in the table.

### 1.2 Integrity and scope

- **Checksums:** all 7 files listed in SHA256SUMS.txt match (7 of 7 OK). The zip file and the attached review prompt have no listed checksum, so they were not checksum-verified.
- **Source files:** used as read-only copies. None was edited.
- **Repository and code:** none requested, opened or inspected. No branch, commit or test was looked at. Statements in the documents about localStorage, snapshots, CP-001 and similar items are read as history only.
- **External sources:** none used. No web search was made.
- **Baseline file:** D3 line 6 names a source baseline, “DEIXEN\_UX\_Workflow\_Decision\_Register\_v2.3.md”. That file is not in the package and was not reviewed.
- **Not verified here:** current repository status, real Amadeus behaviour, learner or practitioner evidence, legal or licensing status, market facts.

### 1.3 Granularity limits on the stages

| Stages | What the source gives | How this report treats them |
| --- | --- | --- |
| 1–33 | One consolidated row, “Steps 1–33” (D3 §8). The row says the numbering “remains thematically consolidated, not reconstructed one by one”. | Reviewed as one theme group. No individual stage detail is invented. |
| 34–89 | 15 rows, each covering one theme or range (D3 §8). No per-stage text. | Reviewed by range. |
| 90–155 | 66 individual rows (D3 §8), plus detailed text in D3 §4.2 and §5.13–§5.23. | Reviewed stage by stage, grouped where the same reasoning applies. |

### 1.4 Which instructions were followed

The attached review prompt and the packaged SONNET\_5.5\_INDEPENDENT\_AUDIT\_BRIEF.md are not identical. A word-level comparison found 92 differing chunks. The packaged Brief and Template also use 15 and 16 sections, and START\_HERE says to read the README first.

Following the prompt’s own rule, the prompt wins. This report uses the prompt’s 14 sections, its evidence labels and its reading order (three core documents first). The Template’s registers and the Brief’s severity scale are kept as sub-tables inside the 14 sections.

| Template part | Where it is in this report |
| --- | --- |
| Audit integrity statement | §1 |
| Executive verdict; document-by-document assessment | §2 |
| Priority and scope matrix | §3 and §10 |
| Cross-document traceability matrix; contradiction register | §8 |
| Coverage and missing-workflow register | §7 |
| Stage proposal review | §9 |
| Vertical slice; Backend-later; Future boundaries | §10 |
| Needs-evidence backlog | §11 |
| Final disposition summary | §12 |
| Open owner decisions | §13 |
| Handoff note; final statement | §14 |

### 1.5 Legend

**Evidence labels** (used in the Evidence field of findings):

- **\[Doc\]** documented statement in D1, D2 or D3.
- **\[Owner\]** owner-provided constraint from the review prompt.
- **\[Interp\]** my interpretation of a document.
- **\[Infer\]** my inference from documented facts.
- **\[Hyp\]** hypothesis, not yet tested.
- **\[Unknown\]** the package does not say.
- **\[Ext\]** external validation required.

**Four independent axes** (no scores, no percentages):

- **Design maturity:** Defined · Mostly defined · Partly defined · Concept only · Missing.
- **Product priority:** P1 · P2 · P3, or “Unmapped” where the documents never say.
- **Development timing:** NOW · LATER · FUTURE · OUT OF SCOPE.
- **Validation status:** Unvalidated · Locally testable · External evidence needed · Backend needed. A row may carry two.

**IDs:** C- contradiction or ambiguity (§8) · G- gap (§7) · R- recommendation to simplify, merge, defer, remove or redesign (§6) · S- smaller change (§12) · V- validation need (§11) · D- owner decision (§13).

**Severity:** Blocker · High · Medium · Low, each with confidence High · Medium · Low. **Stage dispositions:** Retain as proposed · Retain with clarification · Rewrite · Merge · Split · Defer · Remove · Needs owner decision · Needs external validation.

**Every material change** carries 10 fields: reference, current proposal, problem, evidence, recommended action, specific alternative, reason, trade-offs, timing, owner decision. Full cards are in §6 and §7. Smaller items group the 10 fields into six table columns.

### 1.6 Mentioned but not read, by instruction

The owner’s latest message names an Amadeus training book in PDF form. I did not open, read, extract, summarise, map or evaluate it. It is noted again in §14.

## 2. Executive Assessment

The package is a strong strategic base with uneven depth. The rules that protect assessment are far more detailed than the learning content, the first case and the learner screens they protect. No Blocker was found.

### 2.1 Verdict

| Question | Answer |
| --- | --- |
| Overall coherence | **Mixed to strong.** The mission, the scope rules and Stages 90–106 are coherent. Depth is uneven. |
| Ready for Fable 5.2 final review? | **Yes, with conditions.** No Blocker. Several High findings need Fable’s direction (see §14). |
| Ready for implementation? | **Not assessed. A document review cannot show it.** What remains: owner decisions D-01 to D-12 (§13) and external evidence for the first slice (V-01 to V-05, §11). |
| Highest severity found | High |

### 2.2 Three strongest aspects

1. **A clear identity with honest limits.** D1 §1 says: “DEIXEN must not claim that course completion or simulation guarantees employment, full workplace readiness, or expert status.” D1 §6 lists 15 non-goals. D1 §2.4 keeps four kinds of correctness apart. \[Doc\]
2. **Strict NOW / LATER / FUTURE discipline.** D3 §0 says its rules prevent “an accepted future requirement from being mistaken for work that should be built now.” D3 §5.0 gives a table by product function. D3 §10.1 keeps Backend checks visible without making them build tasks. \[Doc\]
3. **The professional-task logic in Stages 90–106.** It separates customer confirmation from authorization (Stages 95–96). It handles changed requests before, during and after execution (97–99). It accepts a correct stop as a valid outcome (100–101). It separates Task Outcome from Performance Outcome (102) and Not Assessed from Not Demonstrated (103–104). This is the best part of the package. \[Doc\]\[Interp\]

### 2.3 Five highest-impact concerns

| # | Concern | Severity / confidence | Main anchors | Detail in |
| --- | --- | --- | --- | --- |
| 1 | **Assessment machinery is ahead of the content and screens it protects.** Stages 107–155 (49 stages) define assessment, result-correction and attempt-start rules. The competency map, the first case and the learner page flows are still open or missing. | High / High | D3 §8 Stages 107–155; D2 §14 Q2, Q4; D2 §2.4 (“Practitioner review remains pending.”); D2 §13.8 | R-01 to R-06; G-01, G-02, G-06 |
| 2 | **The result-correction logic has a gap.** Stage 142 replays a result with the original rule version, so a replay can only reproduce the original result. Stage 141 then offers “Result Corrected”, which needs a decision that replay cannot make. | High / High | D3 Stages 141–143 | C-11; R-02 |
| 3 | **English and the customer-dialogue method are missing from the working register.** D1 §2.7 calls English “a major product objective”. D3 never uses the word “English”. No document says how a non-native writer talks to the simulated customer. | High / High | D1 §2.7; D2 §3.4, §14 Q13, Q18; D3 §5.7, §5.13 | C-01; G-03, G-04 |
| 4 | **P1 and P2 are named but never mapped.** D3 §2.3 restates the two priorities in words. Nothing links them to skills, cases or stages, so “core now” cannot be tested. | High / High | D1 §2.6; D2 §10; D2 §14 Q2; D3 §2.3 | C-09; G-01 |
| 5 | **Overlapping entities and vocabularies will cause build ambiguity.** Task Run, Attempt and Task Runtime overlap. D2 lists 6 sources of truth, D3 lists 7. Several status lists overlap. One “Program Engine” bundles 12 responsibilities. | Medium / High | D3 §0.1; D3 §5.4; D3 §5.6; D2 §6 | C-02, C-03, C-04, C-12, C-14; R-04, R-05, R-08 |

### 2.4 Document-by-document assessment

| Document | Purpose and value | Main problems | Disposition |
| --- | --- | --- | --- |
| **D1** Objectives Reference | Says why DEIXEN exists. Gives the mission, 16 objectives, founder ambitions, non-goals and a status table. Good base for judging every feature (D1 §8). | §2 mixes outcomes, principles, features and commercial items at one level (C-20). P1 and P2 have one-line definitions and no map (C-09). §2.7 frames English around DEIXEN World, which D3 §0.4 puts in FUTURE (C-01). §2.9 sets the Coach as a “Virtual Professional Supervisor”, while D3 §5.2 makes an elaborate Coach persona FUTURE (C-19). It never defines the first learner. | Retain with clarification |
| **D2** Feature Ideas Inventory | Lists the five areas, shared capabilities, open questions and the UX workstream. D2 §1.3 and §13 are strong. | Vision and prior-snapshot notes are interleaved (C-17). §11 tool allocation is superseded (C-05). The §15 journey leaves out practice and assessment and relies on World steps (C-06). It uses “Stage 2” in a different sense from D3 (C-04). Its 30 open questions sit at one level; Q2 and Q4–Q7 remain open. | Retain with clarification. Separate vision from history. |
| **D3** UX/Workflow Register | The detailed proposal set, the NOW/LATER rules and the stage history. Stages 90–106 are the strongest content. | Stages 107–155 are over-specified for a local single-user prototype (R-01 to R-06). Stages 61–89 are out of scope but still in the register (R-07). No English policy (C-01). No competency map (G-01). Overlapping entities and statuses (C-03, C-12). D3 §9.4 repeats many “Still open” paragraphs. A stray sentence sits at line 1473 (C-15). | Retain the structure and Stages 90–106. Rewrite, merge, defer or remove specific groups (see §9). |

### 2.5 What must be resolved before Fable’s review

Nothing blocks the handoff. Two quick owner answers would let Fable start faster: D-01 (first learner and first task) and D-02 (archive Stages 61–89). Until the owner agrees, no R-, S- or G- item in this report is a decision.

## 3. Completion and Scope Matrix

Most areas have a clear direction, but only a few are ready to hand to an implementer. The four axes are independent: a high-priority area can be only partly designed, and a well-designed area can be deferred.

Values marked \[Interp\] are my reading. D1 and D2 define P1 and P2 in one line each and never map them to areas (see C-09). “Unmapped” means the documents give no basis for a P-level.

| Area | Design maturity | Product priority | Development timing | Validation status | Main remaining issue |
| --- | --- | --- | --- | --- | --- |
| Mission, identity, non-goals (D1 §1, §6; D3 §2) | Defined | All | NOW (as rules) | Unvalidated | The first learner is never defined (D-01). |
| Five-area structure (D2 §2; D3 §3) | Mostly defined | P1/P2 \[Interp\] | NOW | Locally testable; external evidence needed (usability) | No page-level flows (G-06). “Explore” is undefined (G-17). |
| Learning tracks and content (D2 §2.2; D3 §5.1) | Partly defined | P1/P2 \[Interp\] | NOW | External evidence needed (learning effect) | No competency map or skill list (G-01). No language path (G-03). |
| Terminal: one workspace, three modes (D2 §2.3; D3 §5.3) | Mostly defined | P1 \[Interp\] | NOW | Locally testable | “Guided” and “Independent” Practice are undefined (C-07). See R-09. |
| Operational truth and engine scope (D2 §2.3; D3 §5.4, §6 A1) | Partly defined | P1 \[Interp\] | NOW | External evidence needed (Amadeus) | Canonical command scope is open (D2 §14 Q5). The repository check in D3 A1 is outside this review. |
| First professional task (D3 Stages 90–106) | Mostly defined | P1 \[Interp\] | NOW | External evidence needed (practitioner); locally testable | No Case Dossier (G-02). No advice step (G-14). Closure criteria missing (G-05). |
| Customer simulation (D3 §5.7, §5.13; Stages 92–94) | Partly defined | P1/P2 \[Interp\] | NOW (text, deterministic) | External evidence needed (non-native writers); locally testable | Input method and intent catalogue undefined (G-04). |
| Case Package and Scenario Bank (D2 §2.4; D3 §5.6) | Mostly defined | P1/P2 \[Interp\] | NOW | Locally testable; external for content | Task Run and Attempt overlap (R-05). Lifecycle metadata missing (G-15). CP-001 still pending. |
| Ghost (D2 §3.1; D3 §5.2) | Partly defined | P1/P2 \[Interp\] | NOW (verified demonstrations) | Locally testable | No content model (G-08). |
| Coach (D1 §2.9; D3 §5.2) | Partly defined | P1/P2 \[Interp\] | NOW (rule-based); FUTURE (persona) | Locally testable | No minimum Coach per mode (G-07, R-12). D1 and D3 differ (C-19). |
| Assessment core: eligibility, independence, validity (D3 §5.8, §5.16–§5.18) | Mostly defined | P1/P2 \[Interp\] | NOW | Locally testable; Backend needed (integrity) | Status lists overlap (R-04, C-12). Protected content on the client is readable (see §10). |
| Exposure and variant holds (Stages 125–138) | Defined, but over-complex | Unmapped | NOW (simplify) | Locally testable; Backend needed (tamper) | Simplify to one exposure record (R-01). |
| Result issue and rule correction (Stages 139–149) | Partly defined (logic gap) | Unmapped | NOW | Locally testable | “Result Corrected” needs a decision a replay cannot make (C-11, R-02, R-03). |
| Attempt start boundary (Stages 150–155) | Mostly defined | Unmapped | NOW (local); LATER (concurrency) | Locally testable; Backend needed | Merge Stages 153–155 into 150 (R-06). |
| Evidence, Growth, recommendations (D3 §5.9; D2 §2.5) | Partly defined | P1/P2 \[Interp\] | NOW | Locally testable; external for employer format | Growth page content and competency rules undefined (G-01, G-06). |
| Home and first-session flow (D2 §2.1; D3 §4.1) | Concept only | P1/P2 \[Interp\] | NOW | Unvalidated | D2 §14 Q1 is still open. Diagnostic route should wait (R-10). |
| Language policy: English, Arabic support (D1 §2.7; D2 §3.4) | Missing for NOW | Unmapped | NOW decision needed | External evidence needed | D3 has no language policy (C-01, G-03). |
| Accessibility baseline (D3 §5.12, check 9) | Partly defined | Unmapped | NOW | Locally testable; external evidence needed | No standard or test plan named (G-11). |
| Founder-Learner Pilot and usability tests (D1 §4.2; D2 §13.9) | Partly defined | n/a (validation) | NOW | External evidence needed | No pilot protocol; contamination risk (G-09, G-10). |
| Backend (D3 §0.2, §6 B–C, §10.1) | Concept only (list of guarantees) | n/a | LATER | Backend needed | Keep visible, not built (see §10). |
| DEIXEN World (D2 §4; D3 §0.4) | Concept only | Unmapped | FUTURE | External evidence needed | Must stay a non-prerequisite (see §10). |
| LLM and voice (D2 §3.4, §5.2; D3 §0.4) | Concept only | Unmapped | FUTURE | External evidence needed | Must not fill engine gaps. |
| Human, trainer, HR, institutional workflows (D3 §0.5, §5.10; Stages 61–89) | Documented, out of scope | n/a | OUT OF SCOPE | n/a | Archive the stage detail (R-07). |
| Commercial and institutional ambitions (D1 §2.15, §3; D2 §9) | Hypotheses | n/a | FUTURE | External evidence needed (market, legal) | Test willingness to pay first (V-07). |

## 4. What Is Sufficiently Complete

These items are stated clearly enough that an implementer would not need to guess. I found no contradiction that touches them. Keep them as written unless the owner decides otherwise.

| # | Item | Why it is sufficiently complete | Anchors |
| --- | --- | --- | --- |
| 1 | Identity, mission and non-goals | The mission, the 15 non-goals and the list of what DEIXEN is not agree across the documents. They rule out a generic LMS, command-only teaching, readiness scores and employment claims. | D1 §1, §6; D3 §2.2 |
| 2 | Four levels of correctness | Input/syntax, operational, customer/task and professional/business correctness are kept apart in all three documents. D3 adds customer experience as a fifth dimension (see C-18). | D1 §2.4; D2 §1.3; D3 §2.5 |
| 3 | NOW / LATER / FUTURE / OUT OF SCOPE rules | Every later proposal is read through these rules. D3 §5.0 maps each product function to NOW or LATER. It also says: “the product rule is current while production infrastructure is deferred”. | D3 §0.1–§0.5, §5.0; README §3 |
| 4 | No LLM in the engine | Stated without hedging: “No LLM is used to fill gaps in rules or generate operational truth.” The same rule appears in D1 and D2. | D3 §0.1, §2.6; D1 §2.10, §6; D2 §5.2, §10 |
| 5 | Professional-task logic, Stages 90–106 | Bounded first task, success rule, error classes, discovery, confirmation versus authorization, changed requests, valid no-reservation outcomes, skill evidence and next-step choice. Stage 91 states that “reservation creation and ticket issuance are separate outcomes”. | D3 §4.2, §5.13–§5.15 |
| 6 | Evidence fairness rules | Lack of opportunity, delay and content shortage are never treated as learner failure. Stage 103: “lack of opportunity is not negative evidence”. Stage 114: “delay is not negative competence evidence”. Stage 124: “content shortage is not learner failure”. D1 §2.12: “Avoid numerical readiness percentages or a single score that hides critical failures.” | D3 §8 Stages 103, 114, 124; D1 §2.12 |
| 7 | Recovery rule for independent assessment | An independent assessment may resume only when attempt identity, history, operational state and assistance conditions can be verified. Otherwise the product must “not award unverified independent evidence”. | D3 §5.12 |
| 8 | The Backend-later list | Six production guarantees are named and kept out of the current build. One of them is “protection against client-side tampering with assessment results, evidence, rule versions, and exposure records”. | D3 §10.1, §6 Phase C |
| 9 | Honest status labelling | D3 says the owner’s stage approval means “provisionally accepted for inclusion and continued review only”. D2 separates four states of an idea. D1 gives a status table. | D3 §8; D2 §0; D1 §7 |
| 10 | Validation checks as testable questions | D3 §10 gives 32 checks, each a question a test can answer. The form is good. The weight is not: checks 13–32 (20 of 32) concern assessment, correction and attempt-start rules, and checks 1 and 9 are the only ones named for beginner usability and for fairness and accessibility (see R-01 to R-06). | D3 §10 |

## 5. What Is Nearly Complete

These items have a sound core. Each needs one small, named step before it can be handed to an implementer. None needs a redesign.

| # | Item | What is already right | The small step that remains | Anchors | Related |
| --- | --- | --- | --- | --- | --- |
| 1 | First professional task (Stages 90–106) | A bounded scope, a success rule, error classes and a clear task chain. | Write a Case Dossier. Add closure criteria. Say how the task covers an advice or option decision. Get practitioner review. | D3 §4.2, Stages 90–106; D2 §2.4 | G-02, G-05, G-14, V-01 |
| 2 | Terminal and its three modes | One workspace, three modes, one operational engine. | Define “Guided Practice” and “Independent Practice” as assistance presets. D3 uses these two names on only two lines (§4.1 and Stages 105–106) and never defines them. | D2 §2.3; D3 §4.1, §5.3 | C-07, R-09 |
| 3 | Case Package and Scenario Bank | A versioned case, a preview, a handoff to Terminal, and “a small number of structured cases” first. | Merge Task Run into Attempt. Add case lifecycle metadata. CP-001 still awaits practitioner review. | D3 §5.6; D2 §2.4 | R-05, G-15, G-02 |
| 4 | Attempt lifecycle | Start, binding of case, version and rules, and duplicate-start protection are all described. | Describe one Attempt lifecycle in one place and merge Stages 153–155 into Stage 150. | D3 Stages 116, 150–155 | R-05, R-06 |
| 5 | Ghost and Coach roles | The roles are distinct and mode-aware. Ghost is demonstration, not evidence. Coach must not rescue the learner in protected assessment. | Define the minimum Coach behaviour per mode and a Ghost content model. | D3 §5.2; D2 §3.1, §3.2 | G-07, G-08, R-12 |
| 6 | Recovery and continuity | Pause, resume, reload and interruption states are required in the local build. Assessment resumes only when it can be verified. | Add a short state table for local tests. Treat “loses connection” (D2 §13.6) as LATER, because the local prototype has no network (see C-16). | D3 §5.12; D2 §13.6 | C-16, G-13 |
| 7 | Evidence model | Three evidence levels (step, task, transfer) and a clear split between result, independence and validity. | Collapse the overlapping status lists into three fields. | D3 §5.8, §5.9 | R-04, C-12 |
| 8 | Result issue reporting | The learner can report a possible result error and keep learning. The product does not pretend a human is reviewing. | Fix the logic gap in Stages 141–143 so each status has a deterministic meaning. | D3 Stage 140–143 | R-02, C-11 |
| 9 | UX principle and workstream | D1 §2.16: “Complexity belongs in the system, not in the learner’s experience.” D2 §13 makes UX a first-class workstream. | Produce the outputs D2 §13.8 lists. None is in the package as a page-level specification. | D1 §2.16; D2 §13 | G-06 |
| 10 | Backend-later requirements | Production guarantees are listed and kept out of the build. | Add the effect of client-side storage on assessment trust (see §10). Define the persistence boundary so local storage can be replaced. | D3 §0.3, §10.1 | G-13 |
| 11 | Founder-Learner Pilot | A clear personal and product value. D1 §4.2 says it “must not replace testing with independent beginners and professional practitioners”. | Write a pilot protocol, including how to avoid contaminating the founder’s own assessment evidence. | D1 §4.2; D2 §13.9; D3 line 1473 | G-09, C-15 |

## 6. What Is Unnecessary, Redundant, or Overcomplicated

I found 12 recommended changes: 7 structural and 5 smaller. Each is a recommendation, not a decision. Most keep the owner's intent and reduce the number of rules, objects and words the build must carry. Nothing is removed from the owner's history: "Remove" means move to an archive.

| ID | Bucket | Change | Main anchors | Owner decision |
| --- | --- | --- | --- | --- |
| R-07 | Remove | Archive Stages 61–89 | D3 §7.2, §8 | D-02 |
| R-03 | Merge | Merge the propagation rules into three | D3 Stages 144–149 | D-03 |
| R-04 | Merge | Replace overlapping status lists with three fields | D3 §5.8; Stages 102, 103, 130, 138, 139, 141 | D-03 |
| R-05 | Merge | Merge Task Run into Attempt | D3 §3.2, §4.4, §5.6; Stages 116, 150–152 | D-06 |
| R-06 | Merge | Merge Stages 153–155 into Stage 150 | D3 §5.23 | D-03 |
| R-01 | Simplify | Replace the exposure model with one reveal record | D3 Stages 125–138 | D-03 |
| R-02 | Simplify (rewrite) | Define the recheck outcomes and separate rule-defect corrections | D3 Stages 140–143 | D-03, D-11 |
| R-10 | Defer | Diagnostic route | D3 §4.1; D2 §13.5 | D-12 |
| R-11 | Defer | Five small items | see the table in 6.4 | D-03 |
| R-08 | Retain but redesign | Bounded modules with one writer per record | D3 §0.1, §5.4; D2 §6 | D-06 |
| R-09 | Retain but redesign | Modes as assistance presets; assessment launched from Scenario Bank | D2 §2.3, §3.2; D3 §4.1 | D-07 |
| R-12 | Retain but redesign | Minimum Viable Coach by mode | D1 §2.9; D3 §5.2 | D-07 |

### 6.1 Remove

**R-07 — Archive Stages 61–89 (and the trainer parts of Stages 59–60 and 64–73)**

- **Reference:** D3 §7.2 ("Steps 61–89"), §7.3, §8 rows 59–89, §0.5, §5.10.
- **Current proposal:** 29 stages on trainer access, notes, learner disputes, second review, institutional oversight and intervention records. All are marked outside current scope. They remain in the active register.
- **Problem:** They are out of scope under the owner's constraints, yet they fill 7 rows of the stage table and two sections. They invite quiet reintroduction. The README warns: "Do not quietly reintroduce these as Backend features."
- **Evidence:** \[Doc\] D3 §8 row 61–63: "Human/trainer review flows are outside current scope." Row 74–78: "Outside current product scope; any reconsideration requires a separate owner decision". \[Doc\] D3 §0.5 lists the same exclusions.
- **Recommended action:** Move Stages 61–89 to a separate archive file marked OUT OF CURRENT SCOPE. Keep four residual principles in the active register, because the rows themselves say to keep them: (1) evidence is private by default; (2) original records are never overwritten; (3) system recommendations are advisory and "never substitute for performance evidence"; (4) least privilege and clear disclosure for the learner's own record.
- **Specific alternative:** Keep one summary row for 61–89 in §8 and point to the archive.
- **Reason:** The history is preserved. The live register shows only what could be built.
- **Trade-offs:** The owner approved these stages provisionally ("موافق"). Moving them may feel like a loss. They are archived, not deleted. Rows 59–60 and 64–68 still need a careful split.
- **Timing:** NOW (document housekeeping, no build effect).
- **Owner decision:** D-02.

### 6.2 Merge

**R-03 — Merge Stages 144–149 into three rules**

- **Reference:** D3 §5.21, Stages 144–149; §9.4 last question.
- **Current proposal:** Six stages: the corrected result becomes current for the same Attempt (144); recalculate only dependent outputs (145); supersede stale recommendations (146); apply corrected eligibility only to activities not yet started (147); do not invalidate completed attempts (148); recalculate competency from all valid evidence (149).
- **Problem:** Six stages describe one idea: Growth, recommendations and eligibility are derived views. Written as six rules, they suggest six mechanisms and a dependency-tracking system.
- **Evidence:** \[Doc\] Stage 145: "Recalculate only dependent Growth, recommendation, and future eligibility/access outputs after a correction". \[Doc\] Stage 149: "Recalculate competency from all relevant valid evidence". \[Doc\] D3 §9.4 asks: "What explicit dependency links or recalculation triggers are needed in the implementation". \[Infer\] Recomputing from the evidence log makes dependency links unnecessary.
- **Recommended action:** Replace with three rules. (1) An Attempt has one current result. A correction supersedes the earlier result and keeps it as linked history (144). (2) Growth, recommendations and eligibility are derived views, recomputed from all valid evidence under current rules whenever evidence changes. Superseded recommendations stay in history (145, 146, 149). (3) An Attempt freezes its start snapshot. A later prerequisite change does not invalidate a completed Attempt (147, 148).
- **Specific alternative:** Keep 144 and 148 as separate rules because they protect evidence. Merge only 145, 146, 147 and 149.
- **Reason:** One principle, three testable rules, no dependency graph to build.
- **Trade-offs:** Needs a complete, deterministic evidence log. D3 already requires one. Recomputation costs little at prototype scale.
- **Timing:** NOW.
- **Owner decision:** D-03.

**R-04 — Replace overlapping status lists with three fields**

- **Reference:** D3 §5.8; §5.7 (line 435); Stages 102, 103, 130, 138, 139, 141; D1 §2.12.
- **Current proposal:** At least seven status lists: performance labels and "what happened" labels (§5.8); assessment outcomes (§5.8); Task Outcome and Performance Outcome (102); skill evidence (103); variant eligibility states (130); validity (139); report states (141).
- **Problem:** The lists overlap and use different words for related ideas. §5.8 calls a failed attempt "Invalidated"; Stage 139 says "Invalid". Stage 103 uses "Not Assessed"; §5.7 says "Not Applicable". An implementer must guess which list owns which fact.
- **Evidence:** \[Doc\] D3 §5.8: "independent, hint-assisted, Coach-assisted, system-assisted, or contaminated"; "correct, self-corrected, assisted correction, incorrect, incomplete, or invalidated". \[Doc\] D3 §5.7: "mark it Not Applicable rather than Not Demonstrated". \[Doc\] D3 §5.8: "These are working labels; final status definitions and criteria must be specified and validated before implementation."
- **Recommended action:** Define three independent fields once, in one table, and derive every display label from them. (1) Completion: Completed or Incomplete. (2) Validity: Valid, Limited or Invalid, plus a reason code such as assistance delivered or technical interruption. (3) Per-skill result: Demonstrated, Not Demonstrated or Not Assessed, plus an independence flag. Keep Task Outcome (102) separate from Performance Outcome. Retire "Not Applicable".
- **Specific alternative:** Keep the §5.8 labels as display text and add a mapping table to the three fields.
- **Reason:** Independent fields prevent impossible combinations and keep tests simple.
- **Trade-offs:** The owner must accept new definitions. Some familiar labels become display-only.
- **Timing:** NOW.
- **Owner decision:** D-03.

**R-05 — Merge Task Run into Attempt**

- **Reference:** D3 §3.2 (line 226), §4.4 (lines 272, 274), §5.6 (line 408) versus Stages 116 and 150–152; D2 §6.
- **Current proposal:** D3 §5.6 keeps five objects apart: Case Package, Scenario Variant, Task Run, Attempt and Operational Session. Stages 116 and 150–152 speak only of the Attempt.
- **Problem:** Task Run and Attempt both begin at "start" and both bind to the case, variant, mode and rules. Two names for one lifecycle invite two records that must be kept in sync. The word "attempt" (any letter case) appears on 157 lines of D3. "Task run" (any letter case) appears on 4.
- **Evidence:** \[Doc\] D3 line 408: Task Run is "one initialized case/variant under a particular mode and support policy". Line 409: Attempt is "the learner's performance history and evidence for that opportunity". Stage 150: "the Attempt is bound to the applicable eligibility/rule/version snapshot".
- **Recommended action:** One entity. An Attempt is one run of one case or variant in one mode. It is bound at start to the case version, variant, rule versions, assistance policy and eligibility snapshot, and it owns the evidence log. The Case Package contains its Variants. The Operational Session is created and owned by the engine and referenced by the Attempt. Remove "Task Run" from D3 §3.2, §4.4 and §5.6.
- **Specific alternative:** Keep "task run" only as a verb for the start step inside Attempt creation.
- **Reason:** Fewer objects. Stages 150–155 already treat the Attempt as the thing that is created.
- **Trade-offs:** "Attempt" can sound like a test to a learner. Use a learner-facing word such as "Session" for Practice, as display text only.
- **Timing:** NOW.
- **Owner decision:** D-06.

**R-06 — Merge Stages 153–155 into Stage 150**

- **Reference:** D3 §5.23, Stages 153–155; §5.22 Stage 150; §6 A2 (line 1156); §10 checks 30–32.
- **Current proposal:** Three stages: resolve a correction and a start request at one boundary (153); refresh an open case when eligibility is lost (154); make a case available again without auto-start (155).
- **Problem:** All three follow from one rule: eligibility is checked when the Attempt is created. Stage 153 is a concurrency problem, and a single-user local prototype has one writer. D3 admits local tests cannot prove it.
- **Evidence:** \[Doc\] Stage 153 row: "enforce cross-client ordering and transaction safety through Backend". \[Doc\] D3 §10.1: "Local Frontend tests for Stages 150–155 do not prove these Backend guarantees."
- **Recommended action:** Write one rule in Stage 150: eligibility is evaluated at the Attempt-creation point; open views are advisory and refresh when eligibility changes; restored eligibility never starts an Attempt. Keep checks 31 and 32 as two local test scenarios. Move the Stage 153 race to the LATER list. Test the two event orders one after the other.
- **Specific alternative:** Keep 154 and 155 as separate learner-visible rules. Merge only 153.
- **Reason:** One principle, fewer stages, the same tests.
- **Trade-offs:** The race rule is only a specification until a Backend exists.
- **Timing:** NOW (rule and sequential tests); LATER (concurrency).
- **Owner decision:** D-03.

### 6.3 Simplify

**R-01 — Replace the exposure model with one reveal record**

- **Reference:** D3 §5.19, Stages 125–138; D3 §5.18 and §5.19 "Still open" paragraphs (lines 795, 843).
- **Current proposal:** Fourteen stages: record delivered versus displayed content (131–133); classify every feedback fragment as General Feedback, Sensitive Detail or Protected Solution (134); map sensitive fragments to skills (136); limit the impact to affected skills (137); hold a variant for one learner (128–130); four eligibility states (130).
- **Problem:** This is a large classification system for one safeguard: do not give a learner an assessment whose answer they have already seen. It needs authored metadata on every feedback fragment, on top of the variant metadata in Stage 111, before one real case exists. D3 forbids "a complex adjudication engine" yet this design moves toward one. In a client-only prototype the protected content is also readable by the learner (see §10), so the machinery cannot give real integrity locally.
- **Evidence:** \[Doc\] D3 line 795 lists as still open: "the simplest way to record learner-specific variant exposure". \[Doc\] D3 line 843: "Do not build browser/device surveillance, automated proctoring, an LLM-based exposure classifier, a complex adjudication engine, or broad investigation case management for launch." \[Infer\] Stages 134 and 136 multiply the authoring work per case.
- **Recommended action:** Keep two content pools per case: a protected assessment pool and an open practice pool. Record one event per learner and variant: what was revealed (nothing, general feedback only, or the full solution) and when. A variant whose full solution was revealed is not offered again to that learner (Stages 123, 124 stay). Mark post-assessment feedback as "general" or "solution" when it is authored. Defer partial-exposure grading (126–127), skill-level impact (136–137) and learner-specific holds (128–130) until real variants and real learners show a need.
- **Specific alternative:** Keep the full model but build it after the first vertical slice passes beginner testing. Or keep 125, 131–133 and 138 and drop only 126–130 and 134–137.
- **Reason:** One reveal record answers the real question with one testable field and keeps the fairness promise of Stages 123 and 124.
- **Trade-offs:** Less granular. A learner who saw only part of a solution may lose a variant that would have been safe. Unaffected skill evidence is less finely preserved. Authoring effort falls sharply.
- **Timing:** NOW (simple rule); the detailed model waits for evidence.
- **Owner decision:** D-03.

**R-02 — Define the recheck outcomes and separate rule-defect corrections**

- **Reference:** D3 §5.20, Stages 140–143; §5.10; §7.2.
- **Current proposal:** The learner reports a possible result issue (140). Statuses: Received, System Check in Progress, Result Corrected, No Change, Unable to Verify Automatically (141). The recheck uses the original attempt data and the original rule version (142). A confirmed rule defect leads to a new rule version and additive corrected-result records (143).
- **Problem:** The documents never say who or what establishes a rule defect. A recheck under the original rule can confirm or reject the stored result, so it can catch a calculation or data mismatch. It cannot find that the rule itself is wrong. "Result Corrected" therefore mixes two cases: a deterministic mismatch, and a rule defect that needs a human decision. D3 denies any human review.
- **Evidence:** \[Doc\] Stage 142: "It must not silently substitute a newer rule version when reproducing the original outcome." \[Doc\] Stage 143: "If a software defect is established in an assessment rule:" (by whom is not stated). \[Doc\] Stage 141: "The current product does not introduce a human-review workflow behind these statuses." \[Infer\] The path from a learner report to a rule correction has an undefined step.
- **Recommended action:** (1) Keep Stage 140 and the "Unable to Verify Automatically" outcome. (2) Define the recheck: recompute from the original data and rule version. Same result: No Change. Different result: Result Corrected, as a calculation or data error. Missing data: Unable to Verify Automatically. (3) State plainly that a recheck cannot find a wrong rule. A wrong rule is established by the product team, outside the engine, who then release a corrected rule version (143) as an ordinary software release. The learner is told when an Attempt is re-evaluated. (4) Drop "System Check in Progress" from the first slice, because a local check is immediate. (5) Replace the applicability framework in 143 with a developer-run script (see R-11).
- **Specific alternative:** If the owner wants no product-team step at all, keep immutable rule versions, the report, and the recomputation check, and list rule-defect correction as a LATER item.
- **Reason:** Every status then has a deterministic cause or an honest, named human step outside the software.
- **Trade-offs:** The product team must read learner reports (D-11). This is a developer fix path, not a trainer or HR review. The learner gets a less dramatic answer than "corrected".
- **Timing:** NOW (recheck, three outcomes, rule-version retention); LATER (release practice for rule defects).
- **Owner decision:** D-03, D-11.

### 6.4 Defer

**R-10 — Defer the diagnostic route**

- **Reference:** D3 §4.1; D2 §13.5 (last bullet), §14 Q24; D3 §5.1.
- **Current proposal:** The learner journey starts with a "relevant baseline/diagnostic where useful".
- **Problem:** A diagnostic needs a competency map, test items, scoring and routing rules. None exists (G-01). The documents themselves say it should not widen the launch.
- **Evidence:** \[Doc\] D2 §13.5: "This should not expand launch scope without evidence." \[Doc\] D3 §4.1: "A diagnostic or lesson completion does not prove independent competence."
- **Recommended action:** For NOW, offer a self-declared starting point at first entry, for example "new to Amadeus" or "used it before". It only changes the suggested first lesson. It carries no score and no evidence value. Keep the full diagnostic as LATER.
- **Specific alternative:** No starting-point choice at all in the first slice. Every learner follows the same first path.
- **Reason:** It avoids building assessment content before the competency map exists.
- **Trade-offs:** Experienced learners repeat some basics. That is acceptable for a beginner-first slice.
- **Timing:** NOW (self-declared choice); LATER (diagnostic).
- **Owner decision:** D-12.

**R-11 — Five small items to defer or trim** (the 10 fields are grouped into six columns)

| Item and reference | Current proposal | Problem and evidence | Action and alternative | Reason and trade-offs | Timing / owner decision |
| --- | --- | --- | --- | --- | --- |
| R-11a · D2 §4.4 | A transition time of "approximately 180–260 ms" | A number for a feature that does not exist in NOW. D2 says it "was only a tentative idea and should be usability-tested". | Move to the FUTURE World list. Alternative: a one-line note under World. | Stops a guess from looking like a requirement. No cost. | FUTURE. Confirm with D-03. |
| R-11b · D2 §3.4 | Open voice option: "Clone the owner's voice for the Coach." | A voice choice before any voice feature. D2 calls it "a hypothesis to test". | Keep under FUTURE. Alternative: drop the idea. | No cost now. | FUTURE. None. |
| R-11c · D2 §3.6 | A speed or time-to-correct-work concept | D2: "This remains a validation idea, not a finalized scoring system." Timing can pressure learners. | Keep as FUTURE. Alternative: record elapsed time as a silent event with no score. | A silent event keeps data for later and adds no pressure. | FUTURE. None. |
| R-11d · D3 Stage 143, steps 3–5 | A framework to "Define the correction's applicability and the conditions under which prior attempts are eligible for rechecking" | Heavy for a prototype with no rule versions yet. D3 line 988 lists the details as still open. | A developer-run script that lists the Attempts stored under a given rule version and re-evaluates them. Alternative: defer all rule-defect correction (see R-02). | Simple and testable. It depends on D-11. | NOW (script); LATER. D-03, D-11. |
| R-11e · D3 Stage 114 | "recheck only affected prerequisites after material changes" | Event-driven rechecks are not needed if eligibility is recomputed when it is read (R-03). | Drop the separate machinery. Keep the principle that delay is not negative evidence. | Fewer triggers. Recompute cost is small. | NOW. D-03. |

### 6.5 Retain, but redesign

**R-08 — Bounded modules with one writer per record**

- **Reference:** D3 §0.1 (line 31), §5.4; D2 §6.1–§6.4, §14 Q16.
- **Current proposal:** The "Program Engine" covers: "task states, conversation/task/operational separation, deterministic case rules, command execution through the verified training engine, validation, assistance rules, eligibility, attempts, results, evidence, corrections, and derived-state recalculation". D2 §6 describes a "Task Runtime" coordinator instead.
- **Problem:** That is 12 responsibilities under one name. It is the unbounded engine that D2 warns against. D3 has no "Task Runtime" (0 matches), so D2 and D3 name the same area differently. No document names module boundaries, who may write which record, or what the screens may call. D2 lists 6 sources of truth; D3 lists 7 (C-02).
- **Evidence:** \[Doc\] D2 §6.2: Task Runtime "must not invent their truths or become one unbounded “mega-engine.”" \[Doc\] D2 §14 Q16: "Should Task Runtime be one module or a set of smaller components?" \[Interp\] D3 §0.1's Program Engine covers the same area.
- **Recommended action:** Define six bounded modules and one rule: each record has exactly one writer. (1) Content store: Case Packages, Variants, lessons; read-only at runtime. (2) Operational engine: owns booking and PNR state. (3) Conversation module: owns customer dialogue state. (4) Task validator: compares operational state with the confirmed request; owns task state and Task Outcome. (5) Assistance policy: decides what help the mode allows; owns help events. (6) Evidence log and projections: append-only events; Growth, recommendations and eligibility are derived views. Attempt creation (the old "Task Runtime") is a function that wires the modules, not a seventh module. Merge the source-of-truth lists into three layers: A definitions, B attempt state, C evidence. Presentation state for World is a FUTURE layer D.
- **Specific alternative:** One deterministic rules package with internal folders, if one unit is preferred. Keep the one-writer rule either way.
- **Reason:** It makes testing simple and turns module boundaries into the future service contracts for the Backend.
- **Trade-offs:** More design effort up front. The owner must accept that "Task Runtime" is not a module. Too much structure can slow a prototype, so use folders and files, not services.
- **Timing:** NOW (design); LATER (service contracts).
- **Owner decision:** D-06.

**R-09 — Modes as assistance presets; assessment launched from Scenario Bank**

- **Reference:** D2 §2.3, §3.2, §14 Q7; D1 §2.3; D3 §4.1, §5.3, Stages 105–106, 113, 118.
- **Current proposal:** Four overlapping vocabularies for "what help am I getting": Terminal modes (Practice, Scenario, Independent Assessment); journey steps (Guided Practice, Independent Practice); assistance levels (High Guidance, Guided Independence, Reduced Assistance, Independent Assessment); evidence labels (independent, hint-assisted, Coach-assisted, system-assisted, contaminated).
- **Problem:** A learner and a developer can get different answers to "what mode am I in and what help can I get?". The open question is still open. Where an independent assessment starts is also unclear (C-08).
- **Evidence:** \[Doc\] D2 §14 Q7: "What exact conditions define guided practice versus independent assessment?" \[Doc\] D2 §2.4: "Opening a case should launch Terminal in Scenario Mode—not Learning Mode." \[Doc\] Stage 113: "DEIXEN determines and explains eligibility; the learner chooses when to start".
- **Recommended action:** Keep the three Terminal modes as the learner's mental model. Define each as an assistance policy carried by the Attempt. Guided Practice: hints, Coach and Ghost available; no independence evidence. Independent Practice: no help unless asked; every help request recorded. Scenario: the policy is set per case in the Case Package. Independent Assessment: no Coach hints and no Ghost; only ordinary interface functions and operational output (Stage 118). Launch assessments from Scenario Bank on an eligible case, with the variant not shown to the learner.
- **Specific alternative:** One Practice mode with a visible help-level switch instead of two named practice modes.
- **Reason:** One policy field replaces four vocabularies, and tests can check it.
- **Trade-offs:** The owner must confirm the presets. Later modes, such as World, must fit the same policy field.
- **Timing:** NOW.
- **Owner decision:** D-07.

**R-12 — Minimum Viable Coach by mode**

- **Reference:** D1 §2.9; D2 §3.2, §14 Q12; D3 §5.2.
- **Current proposal:** D1 sets the Coach as a "Virtual Professional Supervisor" with nine behaviours. D3 limits NOW to "only the deterministic assistance types needed" and makes the persona FUTURE.
- **Problem:** Nothing connects the owner's objective to the NOW scope. It is unknown which of the nine behaviours are deterministic and testable now, and what the Coach may do in each mode.
- **Evidence:** \[Doc\] D1 §2.9: "Cinematic scenes are a high-priority way to express the Coach's supervisory role". \[Doc\] D3 §5.2: "a highly elaborate Coach persona, autonomous AI coaching, or LLM-driven interaction is not a current requirement". \[Doc\] D2 §14 Q12: "What should the Coach say, know, observe, and be allowed to do in each mode?"
- **Recommended action:** Write a one-page table: for each mode, the allowed Coach actions, each drawn from authored content. Examples: task framing text, a hint ladder with fixed hints per step, a post-task review built from the evidence record, and a next-step suggestion from the Stage 105–106 rules. No free conversation. Persona, avatar and cinematic expression stay FUTURE.
- **Specific alternative:** Call the NOW feature "Guidance" and keep "Coach as supervisor" as the FUTURE name.
- **Reason:** It makes D1 §2.9 testable and consistent with D3.
- **Trade-offs:** A rule-based Coach may feel thin next to the vision. That is the honest NOW scope.
- **Timing:** NOW (minimum); FUTURE (persona).
- **Owner decision:** D-07.

## 7. What Is Missing (Prioritised)

Gaps are ordered by what stops a testable first slice. None blocks handing the package to Fable. All of G-01 to G-06 stop a first slice that a real beginner could test. Each gap below is a genuine gap for NOW unless the card says it is an intentional deferral.

### 7.1 High-priority gaps

**G-01 — A P1/P2 competency map with skill statements and an evidence ladder (first task only)**

- **Reference:** D1 §2.6; D2 §10, §2.2, §14 Q2–Q3; D3 §2.3, Stages 103–106, 145–149.
- **Current proposal:** P1 and P2 get one line each. D3 §2.3 restates them in words. Stage 149 says skill position depends on "the defined competency rules".
- **Problem:** Stages 103–106, 107 and 145–149 all depend on skills, skill evidence and skill position. No document lists one skill, its observable criteria, or how evidence adds up. Without it, Demonstrated and Not Demonstrated cannot be assigned, and "core now" cannot be tested.
- **Evidence:** \[Doc\] D2 §14 Q2: "What is the complete P1/P2 professional competency map?" \[Doc\] D2 §2.2 lists as still open: "Final curriculum map, exact Customer Service Track structure, learning outcomes, lesson-to-task traceability, language levels, and evidence-based instructional design validation." \[Infer\] No skill list exists anywhere in the package.
- **Recommended action:** Write a short competency map for the first task only. Start from the abilities in D1 §2.1 (understand the request, clarify, advise, execute, verify, correct or escalate, communicate and close). For each skill give the observable behaviour, the evidence the engine can capture, and the rule for Demonstrated, Not Demonstrated and Not Assessed. Mark each skill P1 or P2.
- **Specific alternative:** Derive the map from a practitioner task analysis (V-01) instead of from D1 §2.1.
- **Reason:** Every later rule for evidence, next step, eligibility and Growth points at skills.
- **Trade-offs:** It needs practitioner time. A small first map will change after the first learners. That is expected.
- **Timing:** NOW, before Growth and eligibility are built.
- **Owner decision:** D-01 first (first learner and first task), then this map.

**G-02 — A Case Dossier for the first case and a practitioner validation path**

- **Reference:** D2 §2.4 (CP-001); D3 §4.2 Stages 90–91, §5.6, §6 A1, Stage 111.
- **Current proposal:** Stage 90 proposes a simple new reservation. D3 §5.6 lists what a case should define. No case is written.
- **Problem:** No document holds the case itself: customer script, known and hidden facts, expected operational state, permitted outcomes, criteria and recovery routes. Practitioner access is not arranged. Stage 111's quality gate cannot be applied to a case that does not exist.
- **Evidence:** \[Doc\] D2 §2.4: "It was identified as a working candidate, not approved production case content." and "Practitioner review remains pending." and "Operational questions U-12 and U-14 were recorded as unresolved." \[Doc\] D3 line 258: "Exact scope and supported operations must be checked against the current implementation and authoritative operational references before the case is finalized." That check is outside this review.
- **Recommended action:** Write one Case Dossier for the first task: scenario script; facts known at the start and facts to discover; allowed customer responses; expected operational state; permitted outcomes, including a valid no-reservation outcome (Stages 100–101); criteria; recovery routes; two controlled variants for later assessment; source-backed operational notes. Add a practitioner review before activation.
- **Specific alternative:** Build on Stage 90 as provisional, and label every NOW build "pending practitioner validation" until the review is done.
- **Reason:** The whole first proof rests on one case.
- **Trade-offs:** It needs a real practitioner (D-08) and authoritative operational references (V-02). The review may change the task scope.
- **Timing:** NOW.
- **Owner decision:** D-08, D-01.

**G-03 — A NOW language policy and communication criteria**

- **Reference:** D1 §2.7; D2 §2.2, §3.4, §14 Q13; D3 §5.7, §5.12, §10 check 9.
- **Current proposal:** D1 and D2 set English-first for DEIXEN World. D3 never uses the word "English". It mentions accent fairness (§5.7, check 9) and Arabic/RTL tests (§5.12).
- **Problem:** D1 calls English a major product objective. In NOW there is no World, and nothing says what language the lessons, Coach, customer text and Terminal explanations use, whether Arabic support exists, what English level is assumed, or how communication is judged. The first slice could test English by accident.
- **Evidence:** \[Doc\] D1 §2.7: "A major product objective is to help learners improve the English used in travel operations and customer service through meaningful work situations". \[Doc\] D2 §2.2: "English should be the primary language of the DEIXEN World experience." \[Doc\] D3 §5.12: "Test readable controls, keyboard use, Arabic/RTL behavior, captions/text alternatives where relevant, and reduced motion within the actual Frontend." \[Doc\] D3 has 0 matches for "English".
- **Recommended action:** Add a short NOW language policy: (1) interface and task text in English; (2) optional Arabic support for explanations and instructions only, not for operational output or customer dialogue; (3) the English level assumed for the first learner; (4) the communication criteria that are judged, and how (clarity and completeness, never accent; see G-05); (5) Arabic/RTL layout tests as in §5.12.
- **Specific alternative:** English-only first slice with plain-English wording rules and an Arabic glossary panel, and no Arabic lessons.
- **Reason:** English is a daily work language in the target job. Leaving it undefined hides a major design choice.
- **Trade-offs:** English-only may exclude weaker beginners. Bilingual content adds authoring and review cost. It needs input from an English-teaching specialist (V-06).
- **Timing:** NOW (policy); a fuller language path later.
- **Owner decision:** D-05.

**G-04 — A customer dialogue contract**

- **Reference:** D3 §5.7, §5.13 (Stages 92–94); D2 §5.1, §14 Q18; D1 §2.10.
- **Current proposal:** The customer is text-first, with authored text and deterministic response rules. Unclear questions may get a request for clarification.
- **Problem:** No document says how the learner talks to the customer: free typing, chosen questions, or a mix. Free typing needs intent matching. That is itself a rule system, and it may reject valid questions from non-native writers. Menus lower the value of the discovery skill. There is no intent catalogue, no fallback behaviour and no handling of misspelling.
- **Evidence:** \[Doc\] D3 §5.7: "customer dialogue uses authored text and predefined deterministic response rules". \[Doc\] D3 §5.13: "unclear questions may receive a request for clarification". \[Doc\] D2 §14 Q18: "How will customer facts and dialogue remain deterministic and testable while still sounding natural?" \[Infer\] No input method is defined in D2 or D3.
- **Recommended action:** Define a dialogue contract for each case: a list of customer intents, each with accepted question forms, the authored answer and the fact it reveals; a fallback reply and a limit on repeated fallbacks; text clean-up (case, spelling); "suggested questions" in Guided Practice only; and a log of unmatched inputs so the team can extend the catalogue. Choose the default input: typed text with intent matching, or a hybrid with a menu in Guided Practice.
- **Specific alternative:** Menu-based questions in the first slice (cheap and fair). Add free text after testing shows the catalogue is stable.
- **Reason:** The no-LLM rule pushes all the difficulty into this contract. It is the heart of the discovery skill (Stages 93–94).
- **Trade-offs:** Free typing is more realistic but fragile. Menus are robust but weaken the evidence for "ask relevant questions". A hybrid costs the most to author.
- **Timing:** NOW.
- **Owner decision:** D-04.

**G-05 — Professional communication and closure criteria**

- **Reference:** D3 §4.2 Stage 91, §2.5, Stages 100–106; D1 §2.1.
- **Current proposal:** Success needs the learner to communicate "the outcome professionally" (Stage 91). D1 §2.1 adds: manage expectations, close tasks, follow up.
- **Problem:** "Professionally" is not defined. With no LLM, the engine can check only observable, structured items. How a closing message is judged is unknown, and "follow up" has no defined action.
- **Evidence:** \[Doc\] D3 Stage 91: "the learner communicates the outcome professionally". \[Doc\] D3 §2.5: "Accent, personality stereotypes, or vague impressions must not substitute for observable professional behavior." \[Doc\] D1 §2.1: "Communicate outcomes, manage expectations, close tasks, and follow up where needed."
- **Recommended action:** Use a short structured closure note that the learner completes. Items: reservation reference stated; passenger and itinerary confirmed; what is not included (no ticket, no payment); the customer's next step; any open risk. The engine checks each item against the case facts. Free-text remarks are stored and not scored.
- **Specific alternative:** The learner picks the correct closure statements from a list. This is more rigid.
- **Reason:** It makes "professionally" observable and deterministic. It also teaches the reservation-versus-ticket distinction in Stage 91.
- **Trade-offs:** A form is less natural than a message, and it may teach to the form. A practitioner must say what a closure must contain (V-01).
- **Timing:** NOW.
- **Owner decision:** D-04.

**G-06 — Learner-facing flows and page specifications**

- **Reference:** D1 §2.16; D2 §13.8, §2.1, §14 Q1, Q23–Q29; D3 §3.1, §4.
- **Current proposal:** D3 §4 gives text journeys and D3 gives many state rules. D2 §13.8 lists the UX outputs still required: journey maps, navigation maps, task flow maps, mode transition maps, state transitions and a usability plan.
- **Problem:** The five areas have no screen-level definition. Home is still open. The rules cannot be tested through a screen path that nobody has specified.
- **Evidence:** \[Doc\] D1 §2.16: the sequence "is a pedagogical framework, not a complete UX specification". \[Doc\] D2 §2.1 lists as still open: "Exact Home layout, widgets, information hierarchy". \[Doc\] D2 §13.8: "Stage 2 should provide evidence and recommendations—not implement or silently finalize the UX." \[Unknown\] Whether those outputs exist elsewhere. None is in the package.
- **Recommended action:** Write six short flow specs for the first slice only: first session; Home to next step; Learning to understanding check to Practice; Scenario Bank browse, preview and start; the Terminal task with Coach and Ghost per mode; result to Growth view. For each: entry, exit, states, errors, empty states, and what the learner sees. Use plain boxes and arrows, not visual design.
- **Specific alternative:** Prototype the flow with the owner first and record it afterwards. This is faster and less reviewable.
- **Reason:** It is the missing bridge between the rules and a testable product. D1 §2.16 asks for it before implementation.
- **Trade-offs:** The specs will change after the first usability test.
- **Timing:** NOW.
- **Owner decision:** D-01.

### 7.2 Medium and low gaps (the 10 fields are grouped into six columns)

| ID and reference | Current proposal | Problem and evidence | Action and alternative | Reason and trade-offs | Timing / owner decision |
| --- | --- | --- | --- | --- | --- |
| **G-07** Minimum Viable Coach by mode. D1 §2.9; D3 §5.2; D2 §14 Q12 | Coach as supervisor (D1) versus rule-based assistance (D3) | Not connected. See card R-12. | See R-12. | See R-12. | NOW (minimum). D-07. |
| **G-08** Ghost content model. D2 §3.1; D3 §5.2 | D2: "Ghost should explain rationale and resulting state, not only replay command syntax." | No format for a demonstration. D2 §3.1 also says: "Ghost should not be available as assistance inside a protected independent assessment." | Define Ghost as an authored, replayable sequence of verified engine inputs with captions for rationale and state. One per supported workflow. Alternative: static worked examples first. | Ghost output must equal engine output. Scripts need re-validation when the engine changes. | NOW. None. |
| **G-09** Founder-Learner Pilot protocol and contamination. D1 §4.2; D2 §13.9; D3 line 1473 | The pilot goals are listed. D3 holds one stray sentence: "The founder can be an early pilot learner, but one person's experience is not sufficient proof that the product works for all beginners or target markets." | The founder also authors and reviews cases and variants, so he knows the answers. His independent-assessment results cannot be independent evidence. Local records can be edited. D1 §4.2: "Seek independent practitioner review of professional actions and outcomes". | A pilot protocol: record the baseline before use; have someone else author or review the pilot cases, or treat the founder's results as usability data only; keep a friction log; label pilot data "founder pilot"; get practitioner review. Alternative: usability tester only. | Protects the credibility of the evidence. Needs a second person for case review. | NOW. D-09. |
| **G-10** Usability and learning validation plan; Backend-preparation exit criteria. D3 §6 A3, §10 | D3 §6 A3: "Test with genuine beginners and relevant practitioners, not only the founder." The exit condition says "the owner has enough evidence that the core Frontend and Program Engine behave as intended". | "Enough evidence" has no measure. Only checks 1 and 9 of 32 are named for usability and accessibility. | A small test plan: named target beginners; tasks; measures such as completion without help, validator results, confusion points; practitioner review of closure notes. Alternative: expert walk-through first. | Makes the Phase A exit testable. Recruiting costs time. | NOW. D-01, D-09. |
| **G-11** Accessibility baseline. D3 §5.12, check 9; D1 §2.16 | A list of things to test: keyboard use, Arabic/RTL, captions, reduced motion | No standard or test method is named, so "accessible" cannot be tested. | Pick a baseline standard and a short test list for the first slice. One option is WCAG 2.2 level AA \[Ext: confirm\]. Alternative: a minimal checklist for the prototype. | A named standard can be audited. It adds test effort. | NOW. External check. |
| **G-12** Neutral interim UI baseline. D2 §8; D1 §5 | The earlier design system and identity are rejected. New identity work starts fresh. D1 §5: "The current logo and visual identity are not approved." | A NOW build needs some visual baseline. Without one, work may stall or revive the rejected identity. | Adopt a plain, temporary baseline (system fonts, basic spacing, no brand marks), labelled non-identity. Identity work continues apart. Alternative: wait for the new identity, which blocks the build. | Keeps the build moving and the identity open. The prototype will look plain. | NOW. D-10. |
| **G-13** Event catalogue and persistence adapter contract. D3 §0.1, §5.12, §6 A2 | D3 §6 A2: "Keep its boundary replaceable and do not describe it as secure production storage." | Evidence is a log of events, but no event list or fields exist. The "replaceable boundary" has no contract. | Define an event catalogue (name, fields, writer module) and a small storage interface: append event, read events by Attempt, read derived view. Local storage implements it now. Alternative: an in-memory interface only. | Protects the later Backend with little extra scope. Some design effort now. | NOW. D-06. |
| **G-14** Task-chain coverage. D1 §2.2; D3 §4.2, Stage 90 | D1 §2.2 chain includes "advice / decision / confirmation" and "closure / follow-up". Stage 90 excludes "no assumed payment, ticket issuance, live availability search, or fare comparison". | The first task has no real advice or option decision. The learner collects given details. "Follow-up" has no defined action. | Decide on purpose: (a) accept that the first task covers discover, confirm, execute, verify and close, with advice in a later case; or (b) add one authored choice inside the customer dialogue, without engine availability search. Define follow-up as a closure-note item (G-05). | Keeps the chain honest. Option (b) adds authoring. | NOW. D-01. |
| **G-15** Content lifecycle metadata. D3 §5.6, Stage 111, §9.4 | D3 §5.6: "The case must be versioned." Stage 111 requires complete versioned content and validation metadata. | No states (draft, practitioner-reviewed, engine-verified, active, retired) or required fields are defined. | Define the lifecycle states and the fields each needs. Alternative: a simple flag: validated yes or no, date, reviewer. | Gives Stage 111's gate something to check. Slight overhead. | NOW. None. |
| **G-16** Target device and connectivity. No anchor | \[Unknown\] No document states the main device or connectivity. | The Terminal and typed dialogue assume a keyboard. Layout and tests depend on the device. | Ask the owner to state the main device and any offline need. Alternative: assume desktop or laptop for the first slice and say so. | Avoids a wrong layout. May limit early reach. | NOW. D-01. |
| **G-17** "Explore", first buyer, employer acceptance. D1 §2.15, §2.14; D2 §14 Q20 | D1 §2.15: "Provide a meaningful entry-level free Explore experience where appropriate." | "Explore" is not defined and is not one of the five areas. Who pays first, and whether employers accept simulated evidence, are unknown. | Name Explore later, or drop it. Test willingness to pay (V-07) and employer expectations (V-08). | Prevents commercial guesses from shaping the build. | FUTURE (intentional deferral). None now. |

## 8. Cross-Document Consistency Matrix

The three documents agree on purpose and limits. They differ mostly in depth, in timing language and in a few naming choices. I found 20 items to resolve. None is a Blocker.

### 8.1 Traceability matrix

Alignment values: Aligned · Partly aligned · Conflicting · Missing by scope · Not enough evidence.

| Topic | D1 anchor | D2 anchor | D3 anchor | Alignment | Finding and disposition |
| --- | --- | --- | --- | --- | --- |
| Mission and professional competence | §1, §2.1 | §1.1 | §2.1, §2.4 | Aligned | Retain. |
| P1 / P2 / P3 | §2.6 | §10 | §2.3 (no P-labels) | Partly aligned | Three wordings of P2; no mapping to skills or cases (C-09, G-01). |
| Five product areas | §2.16 | §2 | §3.1 | Aligned on names | Home’s role is still open (D2 §14 Q1; G-06). |
| Learning and Customer Service | §2.1, §2.5 | §2.2 | §5.1; Stage 34 | Partly aligned | D2 names a Customer Service Track and lists its structure as open. D3 gives principles only (G-01). |
| Terminal and operational truth | §2.11 | §2.3 | §5.3, §5.4 | Aligned | Engine scope is open (D2 Q5). Modes need presets (R-09). |
| Scenario Bank and case model | §2.2 | §2.4 | §5.6 | Partly aligned | Object model differs: Task Run versus Attempt (R-05). No first case is written (G-02). |
| Ghost and Coach | §2.9 | §3.1, §3.2 | §5.2 | Partly aligned | Supervisor versus rule-based assistance (C-19, R-12). No Ghost content model (G-08). |
| Customer simulation and AI boundary | §2.10, §6 | §5.1–§5.3 | §5.7, §0.4 | Aligned on the boundary | The dialogue method is missing (G-04). |
| Assessment and independence | §2.3, §2.12 | §3.5 | §5.8, §5.16–§5.21 | Partly aligned | D1 and D2 state the direction. D3 adds 49 stages (107–155). Over-specified (R-01 to R-06). |
| Evidence, Growth and privacy | §2.12 | §2.5, §3.5 | §5.9, §5.11 | Partly aligned | D2 keeps employer and trainer views open. D3 §5.11 bans portals now (C-13). Status words overlap (R-04). |
| UX, workflow and recovery | §2.16 | §13 | §4, §5.12 | Partly aligned | Principles agree. Page-level outputs are missing (G-06). Connection loss is a timing issue (C-16). |
| Founder-Learner Pilot and validation | §4.2 | §13.9 | line 1473; §6 A3 | Partly aligned | D3 holds one stray sentence and no protocol (G-09, C-15). |
| World, cinematic, language, voice | §2.7–§2.9 | §3.4, §4 | §0.4, §5.2, §7.4 | Partly aligned (timing difference) | D1 treats English-first World and cinematic Coach scenes as high priority. D3 puts World in FUTURE and has no English policy (C-01, C-19). |
| Visual identity and Coach avatar | §5 (last bullet), §2.9 | §3.3, §8 | not covered (named in §13.2) | Missing by scope (intentional) | Separate workstream. A neutral UI baseline is needed for NOW (G-12). |
| Commercial and institutional ambitions | §2.14, §2.15, §3 | §9 | §0.5, §7.2–§7.3; Stages 61–89 | Missing by scope (intentional) | Business ambitions are not software scope. Archive Stages 61–89 (R-07). |
| NOW / LATER / FUTURE / OUT OF SCOPE | §7 (status words only) | §10, §11 | §0, §5.0 | Partly aligned | Only D3 has timing rules. D2 §15 and §13.4 assume World (C-06). |
| Model roles and sequence | §5 (“Opus-ready execution package”) | §11 | §13.2, §13.3; README §3 | Conflicting (superseded history) | D2 §11 is replaced by the owner’s later instruction (C-05, S-02). |

### 8.2 Contradiction and ambiguity register

Types used: contradiction · scope difference · timing difference · objective-versus-feature difference · superseded history · ambiguity · genuine gap. I found no pure contradiction. Most items are ambiguity or scope and timing differences.

| ID | Severity / confidence | Type | Exact anchors | What conflicts or is unclear | Why it matters; resolution |
| --- | --- | --- | --- | --- | --- |
| C-01 | High / High | Genuine gap; scope difference | D1 §2.7; D2 §2.2, §3.4; D3 (0 matches for “English”) | D1 and D2 frame English as an objective, mainly for DEIXEN World. D3, the NOW register, never uses the word. | A major objective has no NOW home. The first slice may test English by accident. Add a NOW language policy (G-03, D-05). |
| C-02 | Medium / High | Ambiguity | D2 §6.2 (6 items); D3 §5.4 (7 items) | D2 lists six sources of truth, including narrative and cinematic presentation state. D3 lists seven: it splits out task state, separates assessment rules from the evidence record, and has no presentation state. | Two lists invite two data models. Use three layers (R-08). |
| C-03 | Medium / High | Ambiguity | D3 §3.2 (line 226), §4.4 (lines 272, 274), §5.6 (line 408); Stages 116, 150–152; D2 §6 | Task Run, Attempt and Task Runtime overlap. | Duplicate lifecycle. Merge (R-05, R-08). |
| C-04 | Low / High | Ambiguity | D2 §6.4, §8.1, §13.8; D3 §7.2, §8 | D2 uses “Stage 2” and “Stage 1” for audit rounds. D3 uses “Stage” for numbered proposals and sometimes “Steps” (“Steps 61–89”). | Readers can mix them up. Rename (S-01). |
| C-05 | Low / High | Superseded history | D2 §11; README §3; D3 §13.2 | D2 §11 still lists Fable for 3D and scenes, and Opus for architecture. D3 §13.2 says the owner’s later instruction “supersedes that tentative split for the present project plan”. | Only a risk if D2 is read alone. Add a marker in D2 §11 (S-02). |
| C-06 | Medium / High | Scope difference; timing difference | D2 §15 steps 5, 6, 8; D2 §13.4; D3 §0.4, §4.1 | D2’s recommended journey leaves out practice and independent assessment. Three of its ten steps depend on World, which D3 puts in FUTURE (step 5 reads “World introduction (future immersive mode)”). | Two journeys are in circulation. Use D3’s NOW journey plus a FUTURE overlay (S-03, G-06). |
| C-07 | Medium / High | Ambiguity | D1 §2.3; D2 §14 Q7; D3 §4.1, Stages 105–106 | “Guided Practice” and “Independent Practice” are journey steps that are never defined. D2 Q7 asks for the conditions and is still open. | Modes cannot be built or tested (R-09, D-07). |
| C-08 | Medium / Medium | Ambiguity | D2 §2.4 (line 160); D3 Stages 113, 150 | D2: opening a case launches Terminal in Scenario Mode. D3: the learner chooses when to start an assessment, and the start request is mode-specific. It is not stated whether an assessment starts from the same case card. | The entry to the highest-stakes mode is unclear (R-09, D-07). |
| C-09 | Medium / High | Genuine gap; ambiguity | D1 §2.6; D2 §10; D3 §2.3 | P2 has three wordings: D1 “work more confidently, reliably, and professionally”; D2 “perform more confidently and stand out professionally”; D3 “improve confidence and professional reliability”. None maps P1 or P2 to skills, cases or stages. | “Core now” cannot be tested. “Stand out” adds a market aim (G-01, D-01). |
| C-10 | Medium / Medium | Ambiguity | D3 Stage 90, §4.2, §6 A1 (line 1143); D2 §2.3 | Stage 90 excludes “live availability search, or fare comparison”. The historical command list in D2 §2.3 and D3 §6 A1 includes AN, TK and FXP. The documents do not say whether those fall under the exclusions. \[Unknown\] | The first task’s command scope is unclear. Needs operational references, not repository access (G-02, V-02). |
| C-11 | High / High | Genuine gap (logic) | D3 Stages 141–143 | A recheck under the original rule can find a calculation or data mismatch. It cannot find a wrong rule. Who establishes a rule defect is not stated, and no human review is allowed. | One status path has an undefined step (R-02, D-11). |
| C-12 | Medium / High | Ambiguity | D3 §5.8; §5.7 (line 435); Stages 102, 103, 130, 138, 139, 141 | Status lists overlap and use different words: “Invalidated” and “Invalid”; “Not Assessed” and “Not Applicable”. | Implementers must guess (R-04). |
| C-13 | Low / Medium | Scope difference | D2 §2.5 (line 221), §14 Q20; D3 §5.11 (line 518) | D2 keeps “employer view, trainer view” open. D3 says: “Do not build trainer portals, employer portals, staff dashboards, broad sharing, or marketing analytics in the current phase.” | No conflict if D2’s views are read as FUTURE. Mark them (S-04). |
| C-14 | Medium / High | Ambiguity | D3 §0.1; D2 §6 | D3 says “Program Engine”. D2 says “Task Runtime”. D3 has no “Task Runtime”. | One area, two names, 12 responsibilities (R-08). |
| C-15 | Low / High | Ambiguity (placement) | D3 line 1473, between §10.1 and §11 | One sentence about the founder as pilot learner sits outside any section. | Easy to lose. It belongs in the pilot protocol (G-09, S-05). |
| C-16 | Low / High | Timing difference | D2 §13.6 (line 735); D3 §5.12 (line 528) | D2 lists “loses connection” as a flow to design. D3 says “recovery after server/network failure require Backend”. The local prototype has no network. | Avoids building network-failure screens now (S-06). |
| C-17 | Low / High | Superseded history | D2 §2.2–§3.2, §12; README §6 | Prior-snapshot notes (localStorage, D96, D97, CP-001) are mixed in with the vision. README says they need fresh verification. | Readers may treat history as current fact (S-07). |
| C-18 | Low / High | Scope difference | D1 §2.4; D2 §1.3; D3 §2.5 | D1 and D2 name four correctness levels. D3 lists five dimensions and adds “Customer experience”. D3 §5.7 calls customer reaction “one evidence input, not the sole evaluator”. | The owner keeps four correctness levels. Treat customer experience as an observation input (S-08). |
| C-19 | Medium / High | Objective-versus-feature difference; timing difference | D1 §2.9; D3 §5.2 | D1 sets the Coach as a “Virtual Professional Supervisor” with cinematic scenes as high priority. D3 makes an elaborate Coach persona FUTURE. | The NOW Coach is undefined (R-12, G-07, D-07). |
| C-20 | Low / High | Objective-versus-feature difference | D1 §2.1–§2.16; D1 §8 | D1 §2 puts learner outcomes, design principles, features and business aims at one level (for example §2.5 method, §2.12 evidence, §2.15 business). | Hard to trace features to objectives, which D1 §8 asks for (S-09). |

### 8.3 What D3 leaves out from D2: intentional or not?

D3 §13.2 asks reviewers to say what is “intentionally outside this workflow register” and what was omitted unintentionally. My reading:

| D2 idea | D2 anchor | In D3? | Intentional? | Disposition |
| --- | --- | --- | --- | --- |
| Visual identity reset | §8 | No (named in §13.2) | Intentional | Separate workstream. Neutral NOW baseline (G-12). |
| Coach avatar and voice | §3.3, §3.4 | No (avatar named in §13.2) | Intentional | FUTURE (R-11b). |
| Speed or time-to-correct-work | §3.6 | No (named in §13.2) | Intentional | FUTURE (R-11c). |
| DEIXEN World, cinematic systems, story | §4 | FUTURE only (§0.4, §7.4) | Intentional | FUTURE. |
| Virtual Company and shift assessment | §7 | FUTURE only (§7.4, Phase D) | Intentional | FUTURE. D2 says: “This is future scope.” |
| Market, commercial, institution | §9 | Excluded (§0.5, §7) | Intentional | FUTURE or outside software. |
| Employer and trainer views | §2.5 | Excluded (§5.11) | Intentional | FUTURE (S-04). |
| English learning path and Arabic support | §2.2, §3.4 | No | Unintentional | Genuine gap (G-03). |
| Customer Service Track structure | §2.2 | Only as Stage 34's theme | Unintentional | Genuine gap (G-01). |
| Founder-Learner Pilot | §13.9 | One stray sentence | Unintentional | Genuine gap (G-09). |
| Diagnostic route | §13.5 | Mentioned in §4.1 | Open | Defer (R-10). |

## 9. UX/Workflow Stage Review (Stages 1–155)

Every stage from 1 to 155 sits in exactly one row below. Most of the foundation is sound, Stages 90–106 are the strongest part, and Stages 107–155 need the simplification described in §6.

**Limitation on Stages 1–33.** D3 §8 holds one consolidated row, “Steps 1–33”. I review it as one theme group. I do not invent individual stage detail. Stages 34–89 exist only as range rows. Stages 90–155 are individually defined.

| Stages | Main proposal (from D3 §8) | Disposition | Rationale and anchors | Timing | Dependencies; evidence or decision needed |
| --- | --- | --- | --- | --- | --- |
| **1–33** | Foundational principles: professional task first, real independence, assistance integrity, evidence levels, customer correctness, case definition, source-of-truth separation, progressive learning, area roles, World boundaries, recovery | Retain with clarification (limited review) | One row only. It says the numbering “remains thematically consolidated, not reconstructed one by one”. The themes match D1 §1–§2. | NOW | A stage-level review needs the 33 stage texts \[Unknown\]. |
| **34–35** | Learning tracks and hierarchy; one central Terminal with distinct modes | Retain with clarification | Consistent with D2 §2.2–§2.3. Tracks need a map (G-01). Modes need presets (R-09). | NOW | D-07; G-01 |
| **36–42** | Terminal responsibilities; separate conversation, task and operational states; learner-initiated closure with DEIXEN validation; mode-specific review; information-source separation; command lifecycle; history, state and progress separation | Retain with clarification | Sound. Matches D3 §5.4. Merge the two sources-of-truth lists (C-02, R-08). | NOW | D-06 |
| **43** | Interruption, continuity and recovery | Retain with clarification | D3 already splits local NOW from durable LATER. Add a state table for local tests (§5 item 6). | NOW (local); LATER (durable) | None |
| **44–48** | Scenario Bank organisation; case brief; skill-based access; versioned case, run, attempt, session; Scenario-to-Terminal handoff | Retain with clarification | The row says “keep first implementation small”. Merge “run” into Attempt (R-05). | NOW | D-06; G-02, G-15 |
| **49–51** | Case-grounded customer behaviour; text and optional voice; continuity across channels; fairness | Split | Keep text-first, case-grounded behaviour and fairness in NOW. The row says “voice can wait”. Move voice and channel continuity to FUTURE. | NOW (text); FUTURE (voice) | D-04; G-04; V-05 |
| **52–58** | Task outcome, review, debrief and evidence kept separate; competency-led Growth; evidence set, not an average; learner-facing and internal evidence; corrections; currency; development history | Retain with clarification | Core evidence principles. They depend on a competency map (G-01) and one status vocabulary (R-04). The row says “final presentation can be staged”. | NOW | D-01, D-03 |
| **59–60** | Private-by-default evidence; separate sharing routes; trainer review additive | Split | Keep “private-by-default product design and no broad sharing” in NOW. Accounts and enforceable access are LATER. Trainer review is OUT OF SCOPE (R-07). | NOW / LATER / OUT OF SCOPE | D-02 |
| **61–63, 69–89** | Trainer access and notes; learner response; disputes and second review; institutional oversight, sampling and safeguards; notifications; interventions and verification; role-based access to institutional information | Remove (archive) | Outside current scope under D3 §0.5 and §7.2. Keep only the four residual principles (R-07). | OUT OF SCOPE | D-02 |
| **64–68** | Recommendations advisory; learner response is not proof; performance evidence required; recommendation status separate from competency; attributable actions | Split | Keep system recommendations as advisory, deterministic logic. They “never substitute for performance evidence”. Archive the human-trainer parts (R-07). | NOW (system); OUT OF SCOPE (human) | D-02 |
| **90–91** | First task: simple new reservation (one adult, one segment, one fare context). Success: a saved, retrievable reservation that matches the latest confirmed request, with professional closure | Retain with clarification; Needs external validation | Strong, bounded scope. D3 §4.2 itself says it is “not a final launch-scope decision”. Needs a Case Dossier (G-02), closure criteria (G-05) and an advice or option step (G-14). Command scope versus exclusions is unclear (C-10). | NOW | D-01, D-08; V-01, V-02 |
| **92** | Separate blocking errors, warnings and unknown or unsupported behaviour | Retain as proposed; Needs external validation | Good rule: “do not treat PNR presence alone as success”. The classes must match verified engine behaviour. | NOW | V-02 |
| **93–94** | Customer discovery and clarification; a simulated customer that is natural but bound to authored facts | Retain with clarification | The core of the professional task. Row 94: “must not validate assumptions or invent unknown facts”. Needs the dialogue contract (G-04). | NOW | D-04; V-05 |
| **95–96** | Confirm essential details; separate confirmation from authorization to create | Retain as proposed | A clear consent boundary. Row 96: “reservation authorization does not authorize payment or ticket issuance”. | NOW | V-01 |
| **97–99** | Request changes before, during and after execution | Retain as proposed | Strong state-integrity rules. Row 98: “no assumptions or blind command retries”. Row 99 keeps post-creation changes outside the first task. | NOW | V-01 (check recovery steps) |
| **100–101** | Customer withdrawal; a valid professional outcome without a reservation | Retain as proposed | Fair and realistic. Row 100: “a correct stop may be a valid outcome, not learner failure”. | NOW | G-02 (allowed outcomes per case) |
| **102–104** | Task Outcome versus Performance Outcome; Demonstrated, Not Demonstrated, Not Assessed; do not repeat a whole scenario | Retain with clarification | The best evidence-fairness rules in the package. Need one status vocabulary (R-04) and a skill list (G-01). | NOW | D-03; G-01 |
| **105–106** | Pick the next activity by need; match the step to understanding, practice, transfer or assessment | Retain with clarification | Row 106 says to “validate simple rules before any complex adaptive engine”. Define practice presets (R-09). | NOW | D-07; G-01 |
| **107–109** | Assessment eligibility from preparation evidence; practice errors do not block; an unsuccessful assessment leads to development | Retain with clarification | Fair. No fixed attempt counts. “Task-related understanding” needs a skill list (G-01). | NOW | G-01 |
| **110–111** | Controlled variants to test transfer; complete versioned variant data before activation | Retain with clarification | The right quality gate. Row 111 says “no automated LLM-based variant generation”. Define lifecycle states and fields (G-15). | NOW | G-15; V-01 |
| **112–116** | Assessment at the first eligible moment; learner chooses when; eligibility kept on delay; briefing; an explicit start creates the Attempt | Retain with clarification | Good learner control. The recheck in 114 is covered by recomputing eligibility on read (R-11e). Stage 116 treats the Attempt as the created object (R-05). | NOW | D-06, D-07 |
| **117–119** | Help requested versus delivered; operational information versus instructional help; permitted external references | Retain with clarification | Honest: row 119 says “track only resources made available or usage DEIXEN can actually verify; no unsupported monitoring claims”. References must be written into each case (G-02). | NOW | D-07; G-02 |
| **120–122** | Review after the result; separate performance review from teaching; protect active variants | Retain with clarification | A good split of review and teaching. Needs the “general” or “solution” tag on authored feedback (R-01). | NOW | D-03 |
| **123–124** | Do not reuse a fully exposed variant for the same learner; handle variant exhaustion | Retain as proposed | Core fairness. Rests on the single reveal record (R-01). Row 124: “content shortage is not learner failure”. | NOW | D-03 |
| **125** | A minimal learner-specific exposure record | Retain with clarification | Becomes the single reveal record (R-01). | NOW | D-03 |
| **126–130** | Complete versus partial disclosure; sensitive elements; learner-specific hold; hold notice; four eligibility states | Defer | Detailed grading and holds need real variants first (R-01). Stage 123’s rule covers the first slice. | LATER (after first slice) | D-03 |
| **131–133** | Delivered versus displayed; no, partial or complete display; count exposure only when visible in the DEIXEN interface | Merge | Log one reveal event when content becomes visible (R-01). Row 133 already rules out “external browser/device monitoring”. | NOW (simplified) | D-03 |
| **134–135** | Classify fragments as General Feedback, Sensitive Detail or Protected Solution; mode-specific visibility rules | Rewrite | Replace with two content pools and a “general” or “solution” tag set when feedback is authored (R-01). | NOW (simplified) | D-03; G-15 |
| **136–137** | Map sensitive fragments to skills; limit the impact to affected skills | Defer | Needs per-fragment metadata that does not exist yet (R-01). | LATER | D-03 |
| **138** | Separate overall assessment validity from skill-level evidence | Retain with clarification | Right idea. Implement as the Validity and Per-skill fields (R-04). | NOW | D-03 |
| **139** | Show Valid, Limited, Invalid; keep unaffected valid skill evidence | Retain with clarification | Good learner transparency. Use the shared Validity field (R-04). | NOW | D-03 |
| **140** | Report Result Issue, linked to the original Attempt | Retain as proposed | A narrow channel, “not a ticketing, complaints, or institutional case-management system”. Who reads reports needs a decision. | NOW | D-11 |
| **141–142** | Five deterministic report states; recheck with original data, case version and rule version | Rewrite | The path from a report to “Result Corrected” has an undefined step (C-11, R-02). Drop “System Check in Progress” for local checks. | NOW | D-03, D-11 |
| **143** | Immutable rule versions; corrected-result records under a new rule version | Split | Keep immutable versions and preservation of the original result in NOW. Replace the applicability framework with a developer-run script (R-11d). Treat rule-defect releases as later practice. | NOW / LATER | D-11 |
| **144–149** | Corrected result is current for the same Attempt; recalculate dependent outputs; supersede recommendations; prospective eligibility; keep completed attempts; recompute competency from all valid evidence | Merge | Six stages express one idea: derived views are recomputed from the evidence (R-03). | NOW | D-03 |
| **150** | Previewing is not starting; eligibility is checked at the start boundary; the Attempt is bound to a snapshot | Retain with clarification | Clear and important. It absorbs Stages 153–155 (R-06). | NOW | D-06 |
| **151–152** | No attempt-governed work until the Attempt exists; duplicate-start protection | Retain with clarification | Good. The rows already split local idempotency (NOW) from server guarantees (LATER). | NOW (local); LATER (server) | D-06 |
| **153–155** | Correction and start race; refresh an open case when eligibility is lost; restore without auto-start | Merge into 150 | One rule at the start boundary (R-06). The race is a concurrency requirement for LATER. | NOW (rule); LATER (concurrency) | D-03 |

### 9.1 Dependencies of Stages 140–155

These stages rest on six things that do not exist yet:

1. One Attempt entity (R-05). Stages 150–155 and 116 all assume it.
2. Three shared status fields (R-04). Stages 139, 141 and 146 all use status words.
3. A rule-version ID stored on every finalized result (Stage 143).
4. An event catalogue and a storage interface (G-13) so that results and exposure can be recomputed.
5. A competency map (G-01) so that recalculation (Stage 149) has rules to apply.
6. A single reveal record (R-01) so that exposure rules have one input.

Downstream, Growth, recommendations and eligibility become derived views (R-03). If R-05 and R-04 are not settled first, Stages 141–155 will be built on names that keep shifting.

## 10. NOW / LATER / FUTURE Scope Assessment

The owner’s sequence is sound: Frontend and a deterministic engine first, Backend kept visible but unbuilt, World and LLM out of the critical path. The main addition I recommend is a clear line between what local testing can prove and what only a Backend, or evidence from outside the software, can guarantee.

### 10.1 What a local prototype can and cannot validate

| A local single-user prototype can validate | Only a Backend, or outside evidence, can guarantee |
| --- | --- |
| Rules and state transitions, run the same way every time | Tamper-proof results, evidence and rule versions |
| Sequential duplicate-start handling, reload and resume | Simultaneous starts from two tabs or two devices |
| That an evidence log can rebuild what the learner did | Durable records that survive a cleared browser or a new device |
| Screen flows, error states and empty states | Account ownership and private access |
| Recompute-from-evidence for Growth and eligibility | That protected assessment content stays hidden from the learner |
| Whether a beginner can follow the flow (with real testers) | Whether the learning transfers to real work (outside evidence, V-04) |

The last row on the left and the last row on the right both need people, not code. One point needs the owner’s attention. In a Frontend-plus-local-engine prototype, every case fact, variant and criterion the engine uses must be available to the browser. A learner with browser tools could read them. \[Infer\] D3 §10.1 already lists “protection against client-side tampering with assessment results, evidence, rule versions, and exposure records” as a Backend item. The same limit applies to confidentiality of protected content.

**Recommendation:** in NOW, label independent assessment as a prototype assessment. It tests the flow and the rules. It is not tamper-proof evidence of independence, and the screens should not claim it is. This also protects claim integrity (D3 §10 check 10) and the founder’s own pilot data (G-09).

### 10.2 NOW: the sequence I recommend

| Step | What happens | Who | Anchors |
| --- | --- | --- | --- |
| 0 | Owner decisions and the first-slice documents: first learner and task (D-01), language policy (G-03), dialogue contract (G-04), closure criteria (G-05), competency map (G-01), Case Dossier (G-02), flow specs (G-06) | Owner, practitioner, reviewers | §7, §13 |
| 1 | Check the operational foundation: command scope, states and exclusions against the real engine and authoritative references. This is Phase A step A1 in D3. It needs repository and engine access, so it is outside this review. | Project team | D3 §6 A1 |
| 2 | Build the engine as bounded modules with one writer per record, an event catalogue and a storage interface | Implementers | R-08, G-13 |
| 3 | Build the screens for the first slice only | Implementers | G-06 |
| 4 | Validate locally: scripted scenarios first, then real beginners and a practitioner | Owner, testers | D3 §6 A3; G-10 |

### 10.3 The smallest coherent vertical slice

**Target learner and task.** The first learner is a beginner with little or no operational GDS knowledge. This echoes D2 §2.2, “someone with little or no operational GDS knowledge”, and the first customer group in D1 §2.14, “Trainees / learners”. I assume this learner types English as a second language on a laptop or desktop with a keyboard. That is an assumption for the owner to confirm (D-01, G-16). The task is Stage 90’s simple new reservation, provisional until the Case Dossier and practitioner review (G-02).

**End-to-end journey.**

1. First entry: a short orientation and an optional self-declared starting point (R-10).
2. Home shows one next step.
3. Learning: the concepts for the first task, plus customer-service basics.
4. An understanding check.
5. Ghost demonstration of the verified workflow (optional).
6. Guided Practice: the task with Coach hints.
7. Independent Practice: the task with help only on request.
8. Independent Assessment on a variant, launched from Scenario Bank (prototype assessment, see 10.1).
9. Result and review, with the option to report a result issue.
10. Growth: evidence by skill, conditions, and a next step. No score.

**Minimum pages and capabilities.** Home (next step only). Learning (one short track). Terminal with three modes as assistance presets (R-09). Scenario Bank with one case family, preview and start. Growth as an evidence view. Across them: Ghost for one workflow, the Minimum Viable Coach (R-12), the result-issue report (R-02), a neutral UI baseline (G-12), and Arabic/RTL and keyboard checks (G-11).

**Deterministic engine responsibilities.** The six modules in R-08: content store, operational engine, conversation module, task validator, assistance policy, and evidence log with derived views.

**Required structured data.** Versioned Case Package with variants; customer intent catalogue; skill map; assistance policies; versioned assessment rules; content pools (protected and open); event catalogue; Attempt record with start snapshot; evidence log; reveal record.

**State transitions: the Attempt lifecycle.**

| From | Event | To | Rule source |
| --- | --- | --- | --- |
| Previewed (no Attempt exists) | Learner presses Start | Start requested | Stage 150 |
| Start requested | Eligibility check fails | Blocked (no Attempt created) | Stages 150, 154 |
| Start requested | Eligibility passes and the record is stored | Created (start snapshot frozen) | Stages 116, 150 |
| Start requested | Storage result is unknown | Uncertain: recover the existing record or retry; no commands run | Stage 151 |
| Start requested | Start pressed again | The same Attempt is recovered | Stage 152 |
| Created | First command or dialogue turn | In progress | Stage 151 |
| In progress | Reload or interruption | Paused; resume only if identity and history can be verified | D3 §5.12 |
| In progress | Learner submits | Completed | D3 §4.4 |
| Completed | Validator and rules run | Finalized: validity, per-skill results, independence flag, rule-version ID | Stages 102–103, 139, 143 |
| Finalized | Learner reports an issue | Recheck: No Change, Result Corrected or Unable to Verify | Stages 140–142 as rewritten (R-02) |
| Finalized | Team releases a corrected rule version | Re-evaluated: an additive corrected-result record | Stage 143 |
| Blocked | Eligibility is restored | Available again; never auto-started | Stage 155 |

**Error and recovery cases.** Invalid command. Ambiguous customer question. Accepted-but-wrong booking. Request changed before, during or after execution. Uncertain command outcome. Reload mid-task. Double-click on Start. Eligibility lost or restored before start. Attempt creation fails or is uncertain. Independent assessment interrupted. Result recheck cannot verify.

**Evidence captured.** D3 §5.4 describes the evidence record as “observable events, source, attempt conditions, assistance exposure, and results”. For the slice this means: the start snapshot; commands and responses; conversation turns; confirmation and authorization events; help requested and delivered; validator results; the closure note; the result (validity, per-skill results, independence flag); reveal events; and the rule-version ID.

**Test scenarios.** Twenty deterministic scenarios, each tied to a documented rule.

| # | Scenario | Expected result | Rule source |
| --- | --- | --- | --- |
| T-01 | Complete the task correctly in Independent Practice, with a correct closure note | Task Outcome met; skills Demonstrated; independent | Stages 91, 102–103 |
| T-02 | The engine accepts a booking with a passenger name that differs from the confirmed request | Command accepted, but Task Outcome not met | Stage 91; D3 §10 check 4 |
| T-03 | Create the reservation after confirming details but before explicit authorization | Flagged: professional correctness not met | Stage 96 |
| T-04 | The customer changes the request before execution: learner reconfirms; or proceeds on the old request | Reconfirm passes; the old request fails | Stage 97 |
| T-05 | The customer changes the request during execution | Dependent steps pause; engine state verified; supported recovery only | Stage 98 |
| T-06 | The customer withdraws before execution; learner stops without creating | Valid outcome, not failure | Stages 100–101 |
| T-07 | The engine returns an unknown or unsupported result | Classed as unknown; not success; no guess | Stage 92 |
| T-08 | A skill has no opportunity in the case | Not Assessed, not Not Demonstrated; targeted next step without a full replay | Stages 103–105 |
| T-09 | Help is denied in assessment; then help is delivered by accident | Denied: still independent. Delivered: flagged assisted | Stage 117 |
| T-10 | Reload in the middle of Practice | The same Attempt resumes with the same state | D3 §5.12 |
| T-11 | Reload in assessment where history cannot be verified | No independent evidence awarded; not labelled a failure | D3 §5.12 |
| T-12 | Double-click on Start | One Attempt; the second click recovers it | Stage 152 |
| T-13 | Attempt creation fails or is uncertain | No commands run; no attempt consumed; existing record recovered | Stage 151 |
| T-14 | Eligibility lost after preview, then restored | View refreshes; start blocked; later available again, never auto-started | Stages 154–155 |
| T-15 | Full solution revealed after an assessment | The variant is not offered again to that learner; if none is left, assessment is deferred and practice offered | Stages 123–124 |
| T-16 | Result recheck: stored result matches; stored result differs; data missing | No Change; Result Corrected (additive); Unable to Verify | Stage 142 as rewritten (R-02) |
| T-17 | A new rule version is added | A result finalized under the old version still reproduces exactly | Stages 142–143 |
| T-18 | A correction is recorded | Growth, recommendations and eligibility are recomputed from evidence; completed attempts stay; nothing is double-counted | Stages 144–149 (R-03) |
| T-19 | A valid customer question is typed with a spelling error | Matched, or a clarification reply; never a wrong fact | Stages 93–94; G-04 |
| T-20 | Complete the first task with keyboard only; check Arabic/RTL text and reduced motion | Task completable; layout correct; motion reduced | D3 §5.12 |

**Explicit exclusions.** Ticketing, payment, availability search and fare comparison (Stage 90). Changes after reservation creation. Multiple customers or shifts. World, 3D, cinematics, voice and LLM. The diagnostic route. Trainer, HR and institutional workflows. Partial-exposure grading and learner-specific holds (R-01). Accounts, sharing and employer portals. More than one GDS. Explore and any commercial features.

**Exit criteria before Backend preparation.** D3 says the move to Backend “is made only when the owner decides”. I suggest the owner decide when all of these hold: (1) the 20 scenarios pass on repeated runs; (2) a small group of target beginners finishes the first task without developer help, and their confusion points are logged and fixed; (3) a practitioner has reviewed the Case Dossier, the closure note and a sample of Attempt records; (4) the competency map is agreed; (5) the event catalogue and storage interface are stable; (6) the screens say plainly that assessment is a prototype assessment.

**Risks that cannot be validated locally.** Tamper-proof evidence and hidden content. Concurrency. Durable cross-device storage. Account ownership. Whether the learning transfers to real work (V-04). Employer acceptance of simulated evidence (V-08). Amadeus operational truth (V-02). Matching of non-native typing (V-05). Legal and data-protection fit (V-09).

### 10.4 Backend-later requirements

Backend is deferred, not cancelled. I name no database, provider or architecture.

| Production guarantee | Why a local prototype cannot guarantee it | Trigger for Backend implementation | Required acceptance test |
| --- | --- | --- | --- |
| Durable storage and recovery of all required records | Local storage is per browser and can be cleared | The owner decides to prepare for production (Phase A exit) | Stop a client mid-Attempt on one device and resume on another with the same Attempt |
| Authentication, ownership and least-privilege access | There are no accounts | Same | One user cannot read or change another user’s records |
| Transaction-safe Attempt creation and idempotency across clients | A local prototype has one writer | Same | Two simultaneous start requests create exactly one Attempt |
| Protection against client tampering with results, evidence, rule versions and exposure records | Client-held data can be edited | Same, and before any claim of independent evidence | An edited client payload is rejected or flagged; results are computed or checked server-side |
| Confidentiality of protected assessment content | Whatever the browser needs, the learner can read \[Infer\] | Same, and before real assessment use | Protected content is absent from client traffic until the moment it is displayed |
| Cross-device synchronisation of progress and eligibility | Local state is per browser | Same | An eligibility change reaches all devices; a stale client cannot start |
| Backup, restore, monitoring, security logging, incident recovery | None exist locally | Same | A restore reproduces the records; alerts fire on faults |
| Safe migration, or explicit exclusion, of local prototype data | Prototype formats will change | Before external learners | A migration dry run, or a clear notice that local data is not carried over |
| Rule releases and re-evaluation at scale (R-02, R-11d) | A developer script is enough locally | Learners exist whose results a rule defect could affect | A release re-evaluates only the affected Attempts and notifies those learners |
| Privacy and data-protection compliance for real learners | Not applicable to one local user | Before external learners | Legal review passes (V-09); a deletion request is honoured |

### 10.5 FUTURE boundaries

| Topic | Keep / revise / defer / separate workstream / reject | Reason | Trigger to reconsider |
| --- | --- | --- | --- |
| DEIXEN World and Virtual Company | Defer; separate workstream | D3 §0.4: “Neither World nor LLM should delay the core Frontend/Engine.” D1 §6 lists “Building a large virtual world before proving the value of the core professional task experience” as a non-goal. D2 §14 Q19 warns that recurring characters could contaminate assessment variants. | The first slice passes beginner tests and practitioner review; learning-value evidence for World (V-12) |
| LLM, customer personality and voice | Defer | D3 §0.4 and §5.7 keep case facts and rules deterministic. Voice must keep an equivalent text path. | Unmatched-input logs show the deterministic catalogue is not enough; accessibility parity and safety are shown (V-11) |
| Multi-customer shift and Shift Evidence Record | Defer | D2 §7: “This is future scope.” | Single-task evidence is validated |
| Coach avatar and visual identity | Separate workstream | D1 §5: “The current logo and visual identity are not approved.” | A neutral baseline is in use and the new identity exploration is complete |
| Speed or time-to-correct-work | Defer; log time silently | D2 §3.6 calls it a validation idea. See R-11c. | Enough data to show time adds meaning without pressure |
| Additional GDS platforms | Defer | D3 §2.3: “Do not add other GDS platforms until the first operational foundation is validated.” | P1 and P2 are validated |
| Commercial and institutional ambitions | Separate workstream (not software) | D1 §3 and §2.15 are unvalidated; prices are hypotheses | Willingness-to-pay evidence (V-07); licensing research (V-13) |
| Human, trainer, HR and administrative workflows | Reject for the current product; archive (R-07) | D3 §0.5 and §8 rows 74–78: “any reconsideration requires a separate owner decision” | A separate, explicit owner decision |
| Practitioner and beginner validation | Keep, and do it in NOW | It is evidence work, not a software feature | Not applicable: it starts now (G-10, V-01, V-03) |

### 10.6 What can be kept from World now, without 3D

Three World ideas carry real learning value and need no 3D, no cinematics and no LLM. They are my suggestions, not decisions.

- **A written customer observation** in the case brief: what the learner can notice about the customer, with no hidden answers.
- **A Coach briefing and debrief** as authored text inside the Minimum Viable Coach (R-12).
- **A short context card** that sets the workplace situation before a case.

Recurring characters, cutscenes, 3D scenes and voice stay FUTURE.

## 11. Critical External Validation Needs

A document review cannot settle these items. Each needs evidence from people, references or tests outside the three files. I did not invent any of that evidence. Two items block the conceptual completion of the first case: V-01 and V-02. V-03 to V-14 do not block the concept itself. V-05, V-06 and V-11 partly affect a design choice. Several others block a claim or a release.

| ID | What needs validating | Why the documents are not enough | Evidence source and method | Blocks conceptual completion? |
| --- | --- | --- | --- | --- |
| V-01 | That the first task, its success rule, customer script, closure note and error classes match real entry-level work | D2 §2.4: “Practitioner review remains pending.” D1 §4.2 says the founder’s own confidence is not enough | A practising reservations agent or supervisor reviews the Case Dossier. Written review notes. A second reviewer for any dispute | **Yes**, for the first case |
| V-02 | That every command, response, warning and state taught or assessed matches real Amadeus behaviour, and that use of Amadeus names and materials is permitted | D3 §10 check 3 asks it as a question. D1 §3.3 requires respect for “permission, licensing, and affiliation boundaries”. D2 §12 is history only | Authoritative operational references named by the owner. Written permissions. A command-by-command table with a source for each row | **Yes**, for the first case’s operational content |
| V-03 | Beginner usability: can a genuine beginner find the next action without hidden assumptions? | D3 §10 check 1 asks it. No user evidence exists. The founder pilot is one learner | Moderated sessions with a small group of target beginners. Observation logs and fixes | No. It gates the Phase A exit (D3 §6 A3) |
| V-04 | Learning effectiveness: does the path improve performance on changed tasks? | D1 §2.5 asks to “distinguish usability, learner satisfaction, learning effectiveness, professional validity, and commercial viability”. Nothing measures it | A before-and-after measure on unseen task variants, rated by practitioners | No. It blocks any claim of effectiveness |
| V-05 | That a deterministic intent catalogue recognises valid questions from non-native English writers and never returns a wrong fact | D2 §14 Q18 is open. No input data exists | A corpus of real typed questions per case; match rate and wrong-fact rate; the unmatched-input log | Partly. It decides D-04, not the concept |
| V-06 | The NOW language policy: level, Arabic support, instruction wording, communication criteria | D1 §2.7 says criteria must be “defined and validated”. D3 is silent | Review by a qualified English-for-work teacher. Comprehension checks with target learners | Partly. A provisional policy can proceed |
| V-07 | Market, first buyer and willingness to pay | D1 §2.14: “a strategic direction to evaluate, not a fully validated go-to-market plan”. D1 §2.15: “Test willingness to pay before treating proposed prices or subscriptions as settled.” | Interviews or pre-sales with learners and training providers | No (FUTURE) |
| V-08 | Employer expectations, and whether employers accept simulated evidence | D2 §14 Q20 is open. D3 §10 check 10 forbids implying employer acceptance | Interviews with hiring managers in target markets. A review of the Growth evidence format | No for the slice. It blocks any employer-facing claim |
| V-09 | Legal: data protection, claims language, use of the Amadeus name | D1 §6 bars claiming “employment guarantees, official Amadeus affiliation”. D3 §11 repeats the safeguard | Legal opinion for each target country. A review of all public claims | No now. It blocks release to external learners |
| V-10 | Accessibility: the chosen standard and test results | D3 §5.12 lists things to test but names no standard (G-11) | Automated and manual tests. Sessions with users of assistive technology | No now. It blocks external release |
| V-11 | Technical research: intent-matching quality without an LLM; whether the engine can support the recovery in Stages 98 and 151–152; faithful Ghost replay | The documents assume these abilities and do not show them | Small, time-boxed technical spikes by the project team. They need engine access, so they are outside this review | Partly. They affect parts of the design, not the concept |
| V-12 | World: feasibility and learning value | D1 §7 calls it a “Strategic design hypothesis” “requiring validation of learning value and production feasibility” | Small prototype tests, later | No (FUTURE) |
| V-13 | Institution, licensing and accreditation | D1 §3.2: licensing, accreditation and legal requirements “must be researched before making commitments” | Regulatory research per country | No (FUTURE, outside software) |
| V-14 | Target device and connectivity | No document states them (G-16) | A short survey of target learners | No. An assumption can be flagged |

## 12. Proposed Changes and Alternatives

This section is an index. The full 10-field cards for R- and G- items are in §6 and §7. Here the smaller S- changes carry their 10 fields in six columns. Every item is a recommendation. None is a decision until the owner agrees.

### 12.1 Structural changes (change what the build is made of)

| ID | Change | Smaller alternative | Timing | Owner decision |
| --- | --- | --- | --- | --- |
| R-01 | One reveal record replaces the 14-stage exposure model | Keep Stages 125, 131–133 and 138; drop only 126–130 and 134–137 | NOW | D-03 |
| R-02 | Define recheck outcomes; separate rule-defect corrections | Keep rule versions, the report and the recheck; defer rule-defect correction | NOW / LATER | D-03, D-11 |
| R-03 | Three rules replace Stages 144–149 | Merge only 145, 146, 147 and 149 | NOW | D-03 |
| R-04 | Three status fields replace seven overlapping lists | Keep old labels as display text with a mapping table | NOW | D-03 |
| R-05 | Task Run merges into Attempt | Keep “task run” only as a verb | NOW | D-06 |
| R-08 | Six bounded modules, one writer per record | One rules package with internal folders | NOW | D-06 |
| R-09 | Modes become assistance presets; assessment starts from Scenario Bank | One Practice mode with a help-level switch | NOW | D-07 |

### 12.2 Smaller changes (rules, scope and wording)

| ID | Change | Smaller alternative | Timing | Owner decision |
| --- | --- | --- | --- | --- |
| R-06 | Merge Stages 153–155 into 150 | Merge only 153 | NOW / LATER | D-03 |
| R-07 | Archive Stages 61–89 | One summary row and a pointer | NOW (documents) | D-02 |
| R-10 | Defer the diagnostic route | No starting-point choice at all | NOW / LATER | D-12 |
| R-11 | Defer or trim five small items (a to e) | Per item, see §6.4 | FUTURE / NOW | D-03 |
| R-12 | Minimum Viable Coach by mode | Call the NOW feature “Guidance” | NOW / FUTURE | D-07 |

**Additions.** G-01 to G-06 are High-priority additions (§7.1). G-07 to G-17 are Medium and Low additions (§7.2).

### 12.3 Documentation changes (the 10 fields grouped into six columns)

| ID and reference | Current proposal | Problem and evidence | Action and alternative | Reason and trade-offs | Timing / owner decision |
| --- | --- | --- | --- | --- | --- |
| **S-01** D2 §6.4, §8.1, §13.8; D3 §7.2, §8 (C-04) | D2 uses “Stage 1” and “Stage 2” for audit rounds. D3 uses “Stage” for proposals and sometimes “Steps”. | Two meanings of one word. \[Doc\] D2 §6.4: “Stage 2 should test whether it should be a distinct module/service”. | Add a short glossary to each file. Alternative: rename in a new version with a dated addendum, because D2 §8.1 says history must not be silently rewritten. | Avoids misreading. A glossary changes no history. | NOW. None. |
| **S-02** D2 §11 (C-05) | A tentative model allocation, labelled a hypothesis. | The owner’s later instruction replaces it (README §3; D3 §13.2). | Add one line in D2 §11: “Superseded by the owner’s later role instruction.” Alternative: move §11 to a history appendix. | Prevents a wrong read. No cost. | NOW. None. |
| **S-03** D2 §15 (C-06) | A ten-step journey that omits practice and assessment and relies on World. | Two journeys circulate (see C-06). | Replace with the NOW journey (§10.3) plus a FUTURE overlay for World steps. Alternative: tag steps 5, 6 and 8 FUTURE and add practice and assessment steps. | One journey. Needs G-06 first. | NOW. None. |
| **S-04** D2 §2.5, §14 Q20 (C-13) | “employer view, trainer view” left open. | D3 §5.11 bars portals in the current phase. | Tag both “FUTURE / outside current scope”. Alternative: remove them from §2.5. | Removes a false conflict. | NOW. None. |
| **S-05** D3 line 1473 (C-15) | One loose sentence about the founder as pilot learner. | It sits outside any section. | Move it into the pilot protocol (G-09) or into §6 A3 as a numbered point. Alternative: delete it, as D1 §4.2 and D2 §13.9 say the same. | Keeps the point from being lost. | NOW. None. |
| **S-06** D2 §13.6 (C-16) | “loses connection” is a flow to design. | D3 §5.12 puts network recovery in LATER. | Mark it “(LATER, needs Backend)”. Alternative: split the bullet into reload (NOW) and connection loss (LATER). | No network screens built too early. | NOW. None. |
| **S-07** D2 §2.2, §2.3, §3.1, §3.2, §12 (C-17) | Prior-snapshot notes sit inside the vision. | README §6 says they need fresh verification. This review did not verify them. | Collect them in one appendix headed “Historical observations, not current facts”. Alternative: add a visible “\[HISTORICAL\]” tag in place. | Readers will not mistake history for fact. Some inline context is lost. | NOW. None. |
| **S-08** D3 §2.5, §5.7 (C-18) | Five “dimensions”, with customer experience as the fifth. | D1 and D2 name four correctness levels. | Reword: four correctness levels, plus customer experience as an observation input. Alternative: keep five dimensions but never call them levels. | Matches the owner’s four levels. | NOW. None. |
| **S-09** D1 §2.1–§2.16, §8 (C-20) | Outcomes, principles, features and business aims at one level. | Hard to trace a feature to an objective. | Tag each subsection: Outcome, Principle, Feature or Business. Alternative: split §2 into two lists and move §2.13–§2.15 to a business list. | Makes the D1 §8 traceability test usable. Some items fit two tags. | NOW. None. |
| **S-10** D3 §9.4 (lines 1375–1397); “Still open” paragraphs (lines 795, 843, 988) | Two lists of the same open questions. | Many items repeat. | Keep one list. Mark questions that this report answers as “answered, pending owner decision”. Alternative: keep §9 as the only list and delete the paragraphs. | Shorter and clearer. | NOW. None. |

### 12.4 Suggested order of work

1. Owner answers D-01 and D-02. Apply the S- changes, which are documentation only.
2. Settle entities and vocabularies first: R-05, R-04, R-08, R-09. The assessment rules use them.
3. Then simplify the assessment rules: R-01, R-02, R-03, R-06.
4. In parallel, write the first-slice documents: G-01 to G-06, with practitioner input (V-01, V-02).
5. Only then build the slice (§10.3).

### 12.5 Final disposition summary

A stage can appear under two dispositions, for example Retain with clarification and Needs external validation.

| Disposition | Stages and items | Short rationale |
| --- | --- | --- |
| Retain as proposed | 92, 95–96, 97–99, 100–101, 123–124, 140 | Clear, testable rules that need no change. |
| Retain with clarification | 1–33, 34–35, 36–42, 43, 44–48, 52–58, 90–91, 93–94, 102–104, 105–106, 107–109, 110–111, 112–116, 117–119, 120–122, 125, 138, 139, 150, 151–152 | Sound core. One named step remains (see §9). |
| Rewrite | 134–135, 141–142 | The model or the logic needs a new form (R-01, R-02). |
| Merge | 131–133; 144–149; 153–155 into 150 | One idea written as several rules (R-01, R-03, R-06). |
| Split | 49–51, 59–60, 64–68, 143 | Part is NOW, part is FUTURE, LATER or out of scope. |
| Defer | 126–130, 136–137; diagnostic route; items R-11a to R-11e | Needs real variants, learners or a competency map first. |
| Remove (archive) | 61–63, 69–89 | Out of current scope. Keep four residual principles (R-07). |
| Reject (as software scope or as a concept) | Human trainer and institutional workflows; “Task Run” as a separate object; the “Not Applicable” label; the “System Check in Progress” status in the local build | Replaced by simpler or already existing concepts. |
| Needs owner decision | 49–51 (D-04); 59–89 (D-02); 105–106 and 112–119 (D-07); 140–143 (D-11) | The choice is the owner’s (§13). |
| Needs external validation | 90–92 (V-01, V-02); 95–99 and 110–111 (V-01); 49–51 and 93–94 (V-05) | Evidence from practitioners, references or testers is needed (§11). |

## 13. Owner Decisions Required

These are the questions that only the owner can answer. A document review cannot settle them. Each row gives the question, the options, my recommendation and what would help. Every recommendation is my interpretation \[Interp\] until the owner agrees. I do not ask about matters the owner has already fixed (see 13.3).

**Priority scale.** Priority 1: answer first. Priority 2: answer before implementation planning. Priority 3: answer before the matching build or pilot step. Priority 4: can wait.

### 13.1 The twelve decisions

| ID and priority | The question | Options and trade-offs | My recommendation, and why only the owner can decide | Evidence that would help; what it unblocks |
| --- | --- | --- | --- | --- |
| **D-01** · Priority 1 | Who is the first learner, on which device, and is Stage 90’s simple new reservation the first task? My assumption (§10.3): a beginner with little or no GDS knowledge, English as a second language, on a laptop or desktop with a keyboard. | **A.** Accept the assumption. Smallest slice. The task has no advice step, so advice moves to a later case (G-14, option a). **B.** Accept it and add one authored choice inside the customer dialogue (G-14, option b). Covers more of the task chain. More authoring. **C.** Choose another learner or device, for example a learner who already knows some Amadeus, or a phone. This changes layout, content and tests, and needs new evidence. | **A.** D1 and D2 describe the learner only in general terms, and D3 §4.2 says Stage 90 is “not a final launch-scope decision”. Only the owner knows which learner he wants to serve first. | V-14 (short survey of target learners). V-01 (practitioner view of Stage 90 as a first task). Unblocks G-01, G-02, G-06, G-10, G-14, G-16 and the vertical slice (§10.3). |
| **D-02** · Priority 1 | Move Stages 61–63 and 69–89 to an archive marked OUT OF CURRENT SCOPE, split Stages 59–60 and 64–68, and keep four residual principles in the active register (R-07)? | **A.** Archive. The live register shows only what can be built. History is kept. **B.** Keep one summary row for 61–89 and point to the archive. **C.** Leave all 29 stages in place and rely on the OUT OF SCOPE labels. No effort, but they keep inviting quiet reintroduction. | **A.** The owner approved these stages earlier (“موافق”), and D3 §8 says any reconsideration “requires a separate owner decision”. Only he can retire them. | None needed. Documents only, no build effect. |
| **D-03** · Priority 2 | Accept, change or reject the assessment simplification package for Stages 107–155: R-01 (one reveal record), R-02 (recheck outcomes), R-03 (three propagation rules), R-04 (three status fields), R-06 (merge Stages 153–155 into 150) and R-11 (five small deferrals). | **A.** Accept the package. Its parts depend on each other. **B.** Accept only the smaller alternatives in §12.1 and §12.2. **C.** Keep Stages 107–155 as written. Nothing is lost, but 49 stages of assessment rules must be planned and built before any real case or variant exists. | **A.** D3 §8 says the owner’s approval means “provisionally accepted for inclusion and continued review only”. Changing these rows is therefore his call. | A first small build (§10.3, T-01 to T-20) shows whether one reveal record and three status fields are enough. Unblocks the assessment part of planning (Stages 52–58, 102–104, 120–139, 141–142, 144–149, 153–155). |
| **D-04** · Priority 2 | How does the learner talk to the simulated customer in the first slice, and how is the closing message judged (G-04, G-05)? | **A.** Typed text matched to an authored intent catalogue, with a fallback reply, and “suggested questions” only in Guided Practice. Closure by a short structured note. **B.** Menu-based questions first. Add free text after testing. Cheap and fair, but it weakens the evidence for “ask relevant questions”. Closure by picking statements from a list. **C.** Free typing with no help. Most realistic, and most fragile for non-native writers. | **A**, tested early. Move to B if the match rate is poor. The no-LLM rule puts all the difficulty into this choice. It also sets how the product feels and how much English it demands (D-05). Only the owner can choose. | V-05 (real typed questions; match rate and wrong-fact rate). V-01 (what a closure must contain). Unblocks G-04, G-05, Stages 49–51 and 93–94. |
| **D-05** · Priority 2 | What language rules apply in the first slice: the language of lessons, Terminal explanations, customer text and Coach; Arabic support; the English level assumed; and how communication is judged (G-03)? | **A.** English interface and task text; optional Arabic for explanations only; a stated English level; communication judged for clarity and completeness, never accent. **B.** English only, with plain-English wording rules and an Arabic glossary panel; no Arabic lessons. **C.** Leave language for a later phase. D1 §2.7 calls English “a major product objective”, and the first slice could test English by accident. | **A** (B if authoring cost is a concern). It is a product-identity choice, and the owner knows his learners’ real level. A provisional policy can start before V-06 ends. | V-06 (English-for-work teacher review; comprehension checks with target learners). Unblocks G-03, the wording of all learner-facing text and the communication criteria in G-05. |
| **D-06** · Priority 2 | Do you accept three choices? (1) Task Run is merged into Attempt (R-05). (2) Six bounded modules with one writer per record. “Task Runtime” is a function that connects them, not a module (R-08). (3) An event catalogue and a small storage interface, so local storage can be replaced later (G-13). | **A.** Accept all three. **B.** Accept the smaller forms: “task run” only as a verb; one rules package with internal folders and the one-writer rule; an in-memory interface only. **C.** Keep the current terms and set module boundaries during the build. Faster to start. The 12-responsibility Program Engine and the overlapping words are then likely to cause rework. | **A**, or B for the lightest start. These words and boundaries become the project’s shared vocabulary and the future Backend contracts. The owner should approve them. | A small time-boxed engine spike (V-11) can test the six-module split. Unblocks Stages 36–42, 44–48, 112–116 and 150–152, and the data model. |
| **D-07** · Priority 2 | Do you accept three choices? (1) The three Terminal modes stay as the learner’s mental model, each defined as an assistance preset carried by the Attempt (R-09). (2) Independent assessment starts from Scenario Bank on an eligible case, and the variant is not shown (R-09). (3) A Minimum Viable Coach by mode: authored task framing, a fixed hint ladder, a post-task review from the evidence, a next-step suggestion, and no free conversation (R-12). | **A.** Accept all three. **B.** Smaller forms: one Practice mode with a visible help-level switch; call the NOW feature “Guidance” and keep “Coach as supervisor” as the FUTURE name. **C.** Keep the four help vocabularies and the Coach as the vision describes, and decide later. A learner and a developer may then get different answers to “what help can I get here?”. | **A.** These choices set what the learner sees and what “Coach” promises. They touch the owner’s vision directly (D1 §2.3, §2.9), so only he can approve them. | Beginner sessions (V-03) can compare A with B. Unblocks Stages 34–35, 105–106 and 112–119, and G-07. |
| **D-08** · Priority 2 (start early) | Can the owner arrange a practising reservations agent or supervisor, and authoritative operational references, to review the first Case Dossier? Until then, may every NOW build be labelled “pending practitioner validation”? | **A.** Arrange a practitioner and the references now. Strongest evidence. It takes time. **B.** Build on Stage 90 as provisional and label every NOW build “pending practitioner validation” until the review is done. **C.** Treat the founder’s own knowledge as enough. Not recommended: D1 §4.2 asks for “independent practitioner review”. | **B** now, and A as soon as possible. Only the owner can approach practitioners. He also knows what permission exists for using Amadeus names and materials (V-02). | V-01 and V-02 are the two items that block the conceptual completion of the first case. Unblocks G-02 and the validation of Stages 90–101 and 110–111. |
| **D-09** · Priority 3 | Which founder-pilot rules do you accept: record a baseline before use; someone else authors or reviews the pilot cases, or the founder’s results count as usability data only; keep a friction log; label pilot data “founder pilot”; get practitioner review (G-09)? Who is the second person? | **A.** The full protocol, with a second person who reviews the cases. **B.** The founder acts only as a usability tester. His results are never used as evidence of competence. **C.** No protocol. Not recommended: he writes and reviews the variants, so his independent-assessment results cannot be independent evidence. | **B** at first, and A when a second reviewer is available. It concerns the owner personally, and it depends on who can help him. | A named reviewer and a baseline note. Unblocks G-09, G-10 and the Phase A exit test (D3 §6 A3). |
| **D-10** · Priority 3 | May the first build use a plain, temporary visual baseline (system fonts, basic spacing, no brand marks), labelled “non-identity”, while identity work continues apart (G-12)? | **A.** Yes. The build keeps moving and the identity stays open. The prototype looks plain. **B.** Wait for the new identity. This blocks the build. **C.** Reuse the earlier design system. Not recommended: D1 §5 says “The current logo and visual identity are not approved.” | **A.** Visual identity is the owner’s decision. | None needed. Unblocks G-12 and the first screens. |
| **D-11** · Priority 3 | May the product team read learner result-issue reports and act on them outside the software? This is a developer fix path, not a trainer, HR or committee review (R-02). | **A.** Yes. Define three recheck outcomes. The product team finds a wrong rule outside the engine and releases a corrected rule version. **B.** No human step at all. Keep immutable rule versions, the report and the recomputation check, and list rule-defect correction as LATER. **C.** Keep Stage 141 as written. Not recommended: “Result Corrected” then needs a decision that a replay cannot make (C-11). | **A**, with B as the minimum. The owner has ruled out human review and trainer administration, so he must say whether this limited product-team step still fits that rule. | None beyond the owner’s rule. Unblocks Stages 140–143 and R-11d. |
| **D-12** · Priority 4 | Defer the diagnostic route, and offer only a self-declared starting point (“new to Amadeus” or “used it before”) that changes the suggested first lesson (R-10)? | **A.** Yes. The choice has no score and no evidence value. **B.** No starting-point choice at all in the first slice. **C.** Build the diagnostic now. It needs a competency map, test items, scoring and routing rules. None of these exists (G-01). | **A** or B. D2 §13.5 itself says “This should not expand launch scope without evidence.” The choice changes the first-session experience, which belongs to the owner. | None now. Revisit when the competency map (G-01) exists. |

### 13.2 Suggested order of answers

1. First: D-01 and D-02. They are short, and they let Fable 5.2 start.
2. Before implementation planning: D-03, D-06 and D-07 (structure), then D-04 and D-05 (how the learner works with the customer and with English). Start D-08 early, because finding a practitioner takes time.
3. Before the matching build or pilot step: D-09, D-10 and D-11.
4. Can wait: D-12.

### 13.3 What I did not ask

The owner’s constraints and the documents already settle these points. I treat them as fixed and did not reopen them.

- No LLM in the engine, and no LLM shortcut for case facts, GDS behaviour, booking state, task correctness, assessment criteria, protected answers or evidence decisions.
- The order NOW, LATER, FUTURE and OUT OF SCOPE. Backend is deferred, not cancelled. World, 3D, cinematics, voice and LLM-supported expression are FUTURE and must not be prerequisites.
- Human review committees, trainer administration, HR and institutional governance are OUT OF SCOPE.
- P1 and P2 are both current core priorities. P3 is future.
- The four levels of correctness. No job-readiness scores, employment guarantees, certification claims or Amadeus affiliation claims.
- The five-area structure. I recommend no change to it. Home needs flows (G-06), and “Explore” is undefined (G-17).

### 13.4 How to answer

For each ID, reply with one of: Agree, Agree with changes, Disagree, or Need more evidence. A short reason helps. You can answer in Arabic. Until you answer, the item stays a recommendation. A short Egyptian Arabic summary of this section is available on request.

## 14. Recommendation for Claude Fable 5.2

This section is for Claude Fable 5.2, the final reviewer and project leader. It is a recommendation. It is not an instruction to any model, and it is not a decision. Only the owner decides what becomes a decision.

### 14.1 Read these five findings first

| # | Finding | Severity / confidence | Detail in |
| --- | --- | --- | --- |
| 1 | **Assessment machinery is ahead of the content and screens it protects.** Stages 107–155 (49 stages) define assessment, correction and attempt-start rules. The competency map, the first case and the page flows are open or missing. | High / High | §2.3; R-01 to R-06; G-01, G-02, G-06 |
| 2 | **The result-correction logic has a gap.** A recheck under the original rule version can only repeat the original result. “Result Corrected” needs a decision that a replay cannot make, and no human review is allowed. | High / High | C-11; R-02 |
| 3 | **English and the customer-dialogue method are missing from the working register.** D1 §2.7 calls English “a major product objective”. D3 never uses the word. | High / High | C-01; G-03, G-04 |
| 4 | **P1 and P2 are named but never mapped** to skills, cases or stages. | High / High | C-09; G-01 |
| 5 | **Overlapping entities and vocabularies will cause build ambiguity.** Task Run, Attempt and Task Runtime overlap. There are 6 or 7 sources of truth, at least seven status lists, and one Program Engine with 12 responsibilities. | Medium / High | C-02, C-03, C-04, C-12, C-14; R-04, R-05, R-08 |

The package also has real strengths (§2.2, §4). The mission, the scope rules and the logic of Stages 90–106 are coherent.

### 14.2 Ready, unresolved, structural, needs the owner first

| Category | Items | Detail in |
| --- | --- | --- |
| **Ready.** Sufficiently complete as a document. Still subject to the owner’s approval. | Identity, mission and the 15 non-goals. The four levels of correctness. The NOW, LATER, FUTURE and OUT OF SCOPE rules. No LLM in the engine. The logic of Stages 90–106 (as logic, not yet as validated content). The evidence fairness rules (Stages 103, 114, 124). The recovery rule for independent assessment. The Backend-later list. Honest status labelling. The form of the 32 validation checks. Stages 92, 95–101, 123–124 and 140 are retained as proposed. | §4 (10 items); §9; §12.5 |
| **Unresolved: one small step left.** | The 11 nearly complete items: first task; Terminal modes; Case Package and Scenario Bank; Attempt lifecycle; Ghost and Coach roles; recovery and continuity; evidence model; result-issue reporting; UX principle; Backend-later effects; Founder-Learner Pilot. | §5 |
| **Unresolved: a larger gap.** | G-01 to G-06 (High): competency map, Case Dossier, language policy, dialogue contract, closure criteria, learner page flows. G-07 to G-17 (Medium and Low). Contradictions and ambiguities C-01 to C-20, led by C-01, C-09 and C-11. External evidence V-01 and V-02, which block the first case. | §7; §8.2; §11 |
| **Structural alternatives for Fable’s attention.** | R-01 (one reveal record), R-02 (recheck outcomes), R-03 (three propagation rules), R-04 (three status fields), R-05 (Task Run into Attempt), R-08 (six bounded modules), R-09 (modes as presets). Each has a smaller alternative. The smaller items R-06, R-07, R-10, R-11, R-12 and S-01 to S-10 can be endorsed or rejected quickly. | §6; §12 |
| **Needs the owner first.** | D-01 to D-12. Ask D-01 and D-02 first. Then D-03, D-06 and D-07, then D-04 and D-05. Start D-08 early, because it takes time. | §13 |
| **Must not enter implementation planning yet.** | See 14.3. | §14.3 |

### 14.3 Must not enter implementation planning yet, or must not be claimed

| Item | Why | What is needed first |
| --- | --- | --- |
| The assessment rules of Stages 107–155 as written | A simpler form is recommended, and the owner has not decided. | D-03 (R-01 to R-06, R-11) |
| Any claim that a local build gives “independent” or “protected” assessment evidence | Protected content on the client is readable, and local records can be edited. Label NOW assessments “prototype assessment”. | Backend, which is LATER (§10.1, §10.4) |
| Customer dialogue and closure judging | No input method, no intent catalogue and no closure criteria exist. | D-04; G-04, G-05; V-05 |
| Growth, eligibility, recommendations and next-step logic | They depend on skills, and no skill list exists. | D-01, then G-01 |
| The first case as valid content | No Case Dossier. Practitioner review is pending. Amadeus behaviour is unverified. | D-08; G-02; V-01, V-02 |
| Result-issue statuses and rule-defect correction (Stages 141–143) as written | The recheck logic has a gap. | D-11; R-02 |
| The diagnostic route | It needs a competency map, test items and scoring rules. | D-12; G-01 |
| Trainer, institutional, dispute, oversight and HR workflows (Stages 61–89) | OUT OF SCOPE. Do not reintroduce them as Backend features. | D-02 |
| World, 3D, cinematics, voice and LLM-supported expression | FUTURE. Not a prerequisite. Must not fill gaps in the engine. | — |
| Backend, accounts, sync and server-side enforcement | LATER. Define the storage boundary now (G-13). Build nothing else. | D-06 |
| Employer-facing claims, readiness scores, certification claims and Amadeus-affiliation claims | Barred by D1 §6 and D3 §10 check 10. | V-08, V-09 |
| The earlier visual identity and design system | Not approved. Use a neutral baseline. | D-10 |
| The Amadeus training book as a template, a curriculum or a command checklist | Not examined here. The owner says it is none of these. | §14.6 |

### 14.4 Suggested first moves (Fable 5.2 may accept, change or ignore)

1. Ask the owner for D-01 and D-02. Both are short.
2. Review the seven structural alternatives (§12.1). Endorse, change or reject each one. They decide how the assessment rules and the engine are planned.
3. Ask the owner for D-03, D-06 and D-07, then D-04 and D-05.
4. Start the item with the longest lead time: a practitioner and authoritative references for the first case (D-08; V-01, V-02).
5. Only then plan the first vertical slice (§10.3) and its first-slice documents (G-01 to G-06). Fable decides who writes them.

### 14.5 Answers to the nine reviewer questions in D3 §13.4

| # | Question (shortened) | Answer in brief | Detail in |
| --- | --- | --- | --- |
| 1 | Which proposals are correct, useful and necessary, and what supports that view? | The spine is sound: the mission and non-goals, the four correctness levels, the NOW, LATER and FUTURE rules, no LLM in the engine, the logic of Stages 90–106, the evidence fairness rules, the recovery rule and the Backend-later list. Each is supported by quoted text from the package. | §4; §5; §9 |
| 2 | Which proposals are unnecessarily complex, duplicative, or solve future infrastructure problems? | The exposure model (Stages 125–138), the correction path (140–143), six propagation stages (144–149), Stages 153–155, seven status lists, Task Run beside Attempt, the 12-responsibility Program Engine, and Stages 61–89. | §6 (R-01 to R-08, R-11) |
| 3 | Are there contradictions between the documents, inside the register, or between the user experience and the no-LLM constraint? | I found no pure contradiction. I found 20 items (C-01 to C-20) that are scope, timing, wording or gap differences. The three that matter most are C-01 (English), C-09 (P1 and P2) and C-11 (the recheck logic). The tension between a natural customer and the no-LLM rule is real. It is G-04. | §8.2 |
| 4 | Are any rules impossible to implement or test without undefined facts, hidden human decisions, unsupported behaviour or LLM inference? | Yes, six. (1) “Result Corrected” hides a human decision (Stages 141–143). (2) “Professionally” in Stage 91 has no testable definition. (3) Skill-based rules (Stages 103–106, 145–149) have no skill list. (4) A natural customer without an LLM has no intent catalogue. (5) The command scope depends on Amadeus facts that nobody has verified. (6) “Independent” assessment cannot be enforced in a client-only build. | C-11; G-05; G-01; G-04; V-02; §10.1 |
| 5 | Are NOW, LATER, FUTURE and OUT OF SCOPE applied consistently? | Mostly yes. The exceptions are small: “loses connection” (C-16), “employer view, trainer view” (C-13), World-dependent steps in D2 §15 (C-06), the mixed rows of Stages 59–60 and 64–68 (R-07), the Coach persona (C-19) and the diagnostic route (R-10). | §8.2; §10 |
| 6 | What essential journeys, error paths or state transitions are missing? Which gaps are deferred on purpose? | Missing: six learner flows (G-06), a language path (G-03), an advice or option step (G-14), a state table for local recovery (§5 item 6) and an event catalogue (G-13). Deferred on purpose: accounts, sync, concurrency, durable storage, World, voice, human workflows and commercial items. | §7; §8.3; §10.4; §10.5 |
| 7 | Which proposals need more evidence from the repository, the training engine, Amadeus references, target learners or practitioners? | Repository evidence: not assessed, by instruction. All other needs are listed in V-01 to V-14. V-01 (practitioner review) and V-02 (Amadeus operational truth and permission) block the conceptual completion of the first case. | §11 |
| 8 | What is the smallest coherent core product and vertical slice? | One beginner learner and one case (Stage 90’s simple new reservation) with controlled variants. One ten-step path: orientation, Home, Learning, understanding check, optional Ghost, Guided Practice, Independent Practice, Independent Assessment as a prototype assessment, Result and review, Growth. Six bounded modules, a 12-row Attempt lifecycle and twenty test scenarios (T-01 to T-20). | §10.3 |
| 9 | Which proposals should be rejected rather than moved to a later phase? | Stages 61–89 as software scope (archive them). “Task Run” as a separate object. The “Not Applicable” label. The “System Check in Progress” status in the local build. Everything else that I propose to defer stays visible for later. | §6.1; §12.5 |

### 14.6 The Amadeus training book (noted only, not part of this audit)

The owner has an Amadeus training book in PDF form. I did not inspect, read, extract, verify, summarise, map or evaluate it. I did not pause or widen this audit for it. The owner’s message says that its table of contents indicates these broad subject areas:

- Amadeus fundamentals, login, encode/decode, system information, and help.
- Availability, schedules, timetables, and minimum connection time.
- Passenger names, PNR creation and retrieval, itinerary elements, reservation terminology, and booking statuses.
- Optional PNR elements, frequent-flyer information, group bookings, queues, PNR copying, and printing.
- Passenger passport details and other booking information.
- Booking, pricing, fares, taxes, payment, ticket issuance, ticket components, and booking classes.
- Meals, codeshare, airline alliances, and related airline information.
- FXD pricing, EMD, and sales reports.
- Passenger and booking mismatches, additional baggage, ticket penalties, and infant additions.
- Refunds, reissues, automated reissues, ticket history, booking modifications, remarks, and debit memo reasons.
- BSP codes, ticket-status interpretation, and industry abbreviations.

Its actual contents, accuracy, currency and relevance have **not** been examined or verified. The owner describes it as a potential reference for identifying the professional knowledge and skills that are relevant to DEIXEN’s competency framework and curriculum. It is not a template to copy, not a mandatory curriculum, and not a checklist that requires every Amadeus command to be implemented. I draw no conclusion about its value or its effect on DEIXEN’s curriculum, and no finding in this report relies on it. Claude Fable 5.2 may assign a separate, properly scoped review of the book to Claude Opus or Claude Sonnet.

### 14.7 Remaining uncertainties

- **Stages 1–33.** D3 consolidates them in one row. I reviewed their themes only (§1.3, §9). A stage-level review needs the 33 stage texts \[Unknown\].
- **Stages 34–155.** D3 §8 holds short summaries. The longer reasoning behind them is not in the package. D3 line 6 names a baseline file, `DEIXEN_UX_Workflow_Decision_Register_v2.3.md`, that is not included.
- **No repository.** By instruction, I did not access or ask for any repository, branch, commit, test or application snapshot. Statements about earlier snapshots, localStorage, D96/D97 or CP-001 are historical context. I did not verify them.
- **Integrity.** The seven package files match `SHA256SUMS.txt`. The zip file and the attached prompt are not covered by that list (§1.2). The attached prompt and the packaged brief differ. I followed the prompt (§1.4).
- **External validation.** V-01 to V-14 are all pending. This review cannot show that the first task matches real work, that the Amadeus content is correct, or that learners succeed.
- **My own judgement.** Several findings are interpretation, inference or hypothesis. They are labelled in the text. I tried to avoid both confirmation bias and contrarian bias. Where the documents agree and are sound, I said so (§4).
- **Counts.** The counts in this report (49 stages, 20 of 32 checks, 15 non-goals, line counts of search matches) come from my own text searches of the package. They can be re-run.

### 14.8 Final statement

This is an independent documentary review by Claude Sonnet 5.5, the second reviewer. It is not final owner approval. It is not a verified repository audit: I did not access any repository, branch, commit, test or application snapshot. It is not an authorization to implement. No recommendation in this report becomes a decision until the owner explicitly agrees. I give no binding instruction to Claude Opus 5.5, Sonnet 5.5 or Haiku 5.5, and I did not create a Master Blueprint. I did not change any source document.

A short summary in Egyptian Arabic is available on request.
