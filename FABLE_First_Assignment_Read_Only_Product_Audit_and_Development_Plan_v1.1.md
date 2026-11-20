# FABLE 5.2 — FIRST ASSIGNMENT
## Read-Only Reality Inspection, Product Completeness, UX Quality & Development Direction

**Project:** DEIXEN  
**Role:** Fable 5.2 — sole Project Lead  
**Phase:** Initial takeover and product-development planning  
**Authorization:** Read-only inspection and recommendations only  
**Code/document/repository modification:** Not authorized in this phase

## 1. Mission

Take over understanding of DEIXEN and determine the strongest evidence-backed direction for developing the existing product.

**Do not treat this handoff as a frozen specification or a literal implementation checklist.** The existing product, its documents, and its prior decisions are inputs to understand and critically assess. The goal is to retain what is sound, improve what is weak, replace or remove what has no sufficient value, and identify what is not yet known.

The governing standard is: **Evidence and quality over legacy decisions. Every element must earn its place.**

The founder wants a professional training and simulated-workplace product that prepares beginners for real travel/reservations work—not a collection of lessons, disconnected screens, command memorization, or unnecessary complexity.

## 2. First phase: read-only inspection

### 2.1 Understand the handoff

Read in this order:

1. `01_GOVERNANCE/DEIXEN_Current_Founder_Authority_and_Product_Direction_v1.1.md`
2. `02_PRODUCT_BASELINE/DEIXEN_Product_Baseline_and_Documentary_Completeness_Review_v1.0.md`
3. This assignment.
4. `03_APPROVED_WORKSTREAM_C/DEIXEN_Workstream_C_Consolidation_Proposal_v0.1_2026-11-20.md`
5. `06_AMADEUS_CURRICULUM/DEIXEN_Amadeus_Curriculum_and_Cross_Company_Transferability_EN.md`
6. The two original Sonnet reports and the two selected Argon Phase 2 records when you need the original reasoning or evidence trail.
7. Consult `05_REFERENCE_ON_DEMAND/` selectively for details; do not bulk-read it merely because it is present.

The current authority register governs the interpretation of older documents. The Workstream C proposal was approved by the founder after its original preparation; preserve the original proposal unchanged, but do not treat its proposal-era “not approved” wording as current status.

### 2.2 Inspect the actual project state

Inspect the current accessible application repository, code, tests, routes, schemas, content assets, and relevant local/remote project files in read-only mode.

Report exactly:

- What repository/branch/commit or snapshot you inspected and its date/identity.
- Which files, areas, and tests were read or run; distinguish full, selective, and metadata-only inspection.
- What was inaccessible or not inspected.
- Whether the current application matches the documentation and where it differs.
- Which capabilities are implemented, partially implemented, broken, absent, or uncertain.

Do not infer implementation from a document or a past screenshot. Do not claim tests passed unless actually run and observed. Do not assume the repository provided is the latest state without recording its identity.

### 2.3 No changes during this phase

Do not edit code, product documents, Source of Truth files, branches, commits, pull requests, repository settings, deployments, production data, or external services. Do not delete or upload files. You may create a separate report, diagrams, proposed specifications, proposed diffs, tests-to-run, and a plan, but do not apply changes.

A later implementation phase requires separate explicit authorization from the founder.

## 3. Required product-level assessment

Assess the product as one connected system and each area by its actual job.

### 3.1 Product purpose and professional task

- Does the existing plan genuinely prepare a learner for integrated travel/reservations work?
- Are customer discovery, clarification, advice, confirmation/authorization, operational execution, validation, recovery, communication, and closure represented?
- Is the target occupational task scope realistic and supported by actual job-task research?
- What important capabilities are missing, overstated, duplicated, or premature?

### 3.2 Home

Determine whether Home helps a beginner understand where they are, what they have actually demonstrated, what needs attention, and the next useful action. Test whether its information hierarchy is clear and whether it duplicates Growth or becomes a generic metrics dashboard. Recommend KEEP / IMPROVE / RETHINK / REPLACE / REMOVE / VALIDATE for each material element.

### 3.3 Learning

Assess Customer Service Track and Amadeus Track together and separately:

- Are their competencies, learning outcomes, scope, and sequence defined?
- Are P1/P2 mapped to actual professional tasks?
- Does each topic teach understanding and transfer, not only command recall?
- Is each lesson traceable to practice/scenario/assessment opportunities?
- Are beginner explanations self-contained and understandable?
- Is English-first learning supported by in-product Arabic clarification without creating an unintended barrier?
- What evidence justifies a learner moving to the next dependent skill or task?
- Does the design avoid both premature progression and arbitrary, frustrating locks?

### 3.4 Terminal

Inspect the actual engine and modes:

- Practice, Scenario, and Independent Assessment remain distinct.
- Operational output is genuine to the implemented engine and never falsely presented as live Amadeus.
- DEIXEN explanation is clearly separate from system output.
- System/syntax correctness is distinct from customer/task and professional correctness.
- Task context, state, validation, errors, recovery, changed requests, pause/resume, and attempt boundaries work coherently.
- Identify current operational coverage and a justified expansion path. Do not invent Amadeus behavior or infer current truth from the 2019 book alone.

### 3.5 Ghost

Does Ghost teach the screen and workflow clearly, using the same operational engine? Does it explain why a step occurs, what the system returns, what state changes, and why the result matters? Does the learner control pace, pause, replay, and depth without cognitive overload? Does it transition toward learner execution? Does it create no independence evidence and remain excluded from protected independent assessment?

### 3.6 Scenario Bank and cases

Assess case discovery, taxonomy, case briefing, prerequisites, case dossier, customer interaction, terminal handoff, variants, professional criteria, failure/recovery, and closure. Identify missing job situations without inventing category sprawl. Preserve CP-001 as HOLD until required modifications and professional/operational verification are complete.

### 3.7 Growth and evidence

Does Growth show what the learner demonstrated, under what conditions, and how independently? Are assistance, errors, recovery, transfer, and limitations clear? Is the main view understandable while detailed records remain accessible? Does the evidence distinguish simulated performance, practitioner review, and external certification? What is the smallest useful Evidence Summary without unsupported claims?

### 3.8 Coach

Does Coach function as a context-aware professional learning supervisor rather than a generic tooltip or answer machine? Define its permitted behaviour by mode, triggers, guidance levels, questions, recurring-error support, debrief, next-step recommendation, and fading assistance. Separate Coach from customer simulation and Ghost. It must not rescue Independent Assessment.

## 4. End-to-end UX and simplicity audit

**Complexity belongs in the system, not in the learner's experience.**

Map real learner journeys across Home, Learning, Ghost, Terminal, Scenario Bank, assessment, and Growth. Include first-time use, return use, normal completion, misunderstanding, wrong command, accepted-but-wrong task, customer changes, warnings, help requests, help actually delivered, interruption, pause/resume, unsuccessful tasks, corrected results, and next learning action.

Evaluate:

- Cognitive load and information hierarchy.
- Navigation, labels, terms, mode/state clarity, and next-step clarity.
- Progressive disclosure without hiding essential operational/evidence information.
- Unnecessary steps, duplicated explanations, dead ends, and confusing transitions.
- Accessibility, desktop/laptop-first design, tablet/phone constraints, language support, reduced motion, and text alternatives.
- Whether the interface helps learners understand instead of performing work for them.
- Whether UX changes preserve assessment fairness, independence, traceability, and evidence meaning.

Do not use click count, speed, visual polish, or user enjoyment alone as proof of good UX or learning effectiveness.

## 5. Learning progression and understanding

The founder expects learners not to advance to genuinely new dependent material without the necessary understanding of the current stage. Design a fair and skill-specific model that distinguishes content exposure, comprehension, supported performance, independent performance, transfer, and valid assessment.

Do not use lesson completion or one correct answer as sufficient proof. Do not invent global readiness percentages or excessive repetition. Explain what blocks a dependent task, why, what evidence is missing, and what the learner can do next. Allow progression where a gap is non-critical or can safely be developed later.

## 6. Cross-company transferability and Amadeus

Use the 2019 Amadeus book as a broad curriculum coverage reference—not as automatic proof of current command syntax or behaviour. Teach verified transferable foundations. Clearly label simulated information that varies by airline, market, date, fare, agency/company policy, office/PCC configuration, permissions, or employer workflow. Never present simulated values as live data or universal company policy.

Preserve the verification gates. Separate source-backed command truth, actual authorized environment testing, and practitioner assessment. Do not close an operational or professional evidence gate without appropriate evidence.

## 7. Every element must earn its place

For every page, capability, feature, workflow, rule, learning object, visual component, Coach behaviour, AI/model use, or proposed addition, evaluate the problem solved, beneficiary, objective advanced, evidence of value, alternative, UX impact, complexity, dependencies, maintenance, risk, and opportunity cost.

Use these dispositions:

- **KEEP** — useful and sound; no change justified.
- **IMPROVE** — retain purpose; improve implementation or experience.
- **RETHINK / REPLACE** — current mechanism is weak; propose a stronger one.
- **COMBINE / SIMPLIFY** — reduce duplication and cognitive load without losing necessary meaning.
- **REMOVE** — no sufficient value or net harm; explain dependencies and consequences.
- **VALIDATE** — insufficient evidence to decide.

Propose stronger alternatives when genuinely better. Do not add features merely for novelty, competitor imitation, AI usage, or sophistication. Prefer the smallest coherent solution with the strongest useful outcome.

Any material product-level change must be presented to the founder. Technical decisions remain delegated to you.

## 8. Team and execution planning

Fable is the sole project lead. You may form a task-appropriate team of approximately three to five assistants/contributors, potentially including Opus, Sonnet, Haiku, ChatGPT, Gemini, or others available. Choose assignments based on capability and task, not a rigid permanent role chart. No contributor can override your authority or make product-level decisions. You own coherence, review, and integration.

## 9. Required deliverables

Produce a concise but sufficiently detailed **Read-Only Reality, Product Quality & Development Direction Report** containing:

1. Inspection coverage and limitations.
2. Current product reality: implemented / partial / broken / absent / unknown.
3. Product purpose and occupational task completeness assessment.
4. Area-by-area assessment of Home, Learning, Terminal, Ghost, Scenario Bank, Growth, and Coach.
5. End-to-end learner journey and integration maps.
6. UX/cognitive-load findings and specific simpler/better alternatives.
7. Learning progression/understanding gate proposal.
8. Amadeus scope and verification gaps; cross-company variable-data handling.
9. KEEP / IMPROVE / RETHINK / REPLACE / COMBINE / REMOVE / VALIDATE register, with evidence, impact, alternatives, dependencies, risk, and priority.
10. Proposed definition and acceptance criteria for a complete local Core.
11. An ordered development roadmap with dependencies and validation gates.
12. A model delegation plan for approximately three to five contributors, with Fable retaining integration ownership.
13. A separate Founder Decision Queue: only unresolved product-level questions that genuinely require founder authority. For each, provide evidence, alternatives, consequences, and your recommendation. Do not repeat decisions already answered in the current authority register.
14. A separate Technical Decisions Log: decisions you can resolve within your delegated authority.
15. An Evidence/Validation Register: matters requiring current Amadeus sources, authorized testing, practitioner input, learners, or market research.

Do not turn the report into an unbounded wishlist. Prioritize what is necessary for the product's professional and educational purpose, what materially improves UX, and what can be proven.

## 10. Acceptance standard for this phase

This phase is complete when:

- You can explain the current state of DEIXEN from inspected evidence, not only documents.
- You have distinguished owner directions, hypotheses, reviewer proposals, technical decisions, and evidence gaps.
- Every existing major area and cross-product capability has a reasoned disposition.
- The end-to-end learner and professional-task journey is coherent and its gaps are visible.
- The UX direction is demonstrably simpler for beginners without weakening learning or evidence integrity.
- Stronger alternatives have been considered where useful.
- The proposed local Core has scope, dependencies, and observable acceptance criteria.
- Product-level decisions are isolated for founder approval; technical matters are handled by you.
- No code or source files were modified during this first phase.

**Do not ask the founder to repeat decisions already documented. Do not treat historical approval as immunity from criticism. Do not silently change product direction. Do not begin implementation until separately authorized.**
