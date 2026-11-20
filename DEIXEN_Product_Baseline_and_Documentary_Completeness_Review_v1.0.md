# DEIXEN — Product Baseline & Documentary Completeness Review

**Document ID:** DEIXEN-PRODUCT-BASELINE-001  
**Version:** 1.0  
**Date:** 20 November 2026  
**Purpose:** Give Fable one current, concise product-level orientation and a candid map of what is planned, what is not yet fully specified, and what cannot be verified from documents alone.  
**Authority:** Interpret together with `01_GOVERNANCE/DEIXEN_Current_Founder_Authority_and_Product_Direction_v1.1.md`.  
**Evidence status:** Documentary synthesis only. It is not a live application inspection, command verification, practitioner validation, or proof that a described feature is implemented.

## 1. Executive product thesis

DEIXEN aims to bridge the gap between learning reservation commands and performing travel/reservations work responsibly. Its organizing unit should be the **professional task**, not a lesson, command, page, or score in isolation.

A complete task may require the learner to understand a customer, ask and clarify, identify constraints, offer bounded alternatives, confirm the choice and authorization, execute the operation, inspect the result, recover from errors, communicate clearly, and close/follow up appropriately. The product should progressively reduce assistance and preserve evidence of what the learner actually did.

The intended result is transferable, demonstrable capability—not a promise of actual employment experience, guaranteed hiring, or universal workplace readiness. The initial core priorities are P1 and P2; P3 is advanced specialization for later consideration after P1/P2 are adequately designed and validated.

## 2. Founder problem thesis — why each product element must exist

DEIXEN was created to address four core problems: (1) expensive or inaccessible Amadeus learning and the need for better value, not simply the lowest price; (2) the gap between knowing commands and performing real travel/reservations work; (3) insufficient practical preparation that may weaken a candidate's competitiveness; and (4) superficial progress systems that reward lesson completion without proving understanding, independence, or genuine progression. Additional problems—such as not knowing where to start, difficulty understanding technical explanations, weak error-recovery practice, poor visibility into skill gaps, and limited transfer to unfamiliar tasks—are candidates to validate, not automatic feature requests.

A proposed product element should solve one or more of these problems or another evidenced learner/professional/business need. Do not equate every problem with a new feature; first test whether clearer teaching, better workflow, stronger integration, or a simpler existing capability is sufficient.

## 3. The integrated learner and professional-work journey

The current pedagogical model is:

**Learning → Demonstration (Ghost) → Guided Practice → Independent Practice → Scenarios → Independent Assessment → Evidence → Growth / continued development.**

This is a learning architecture, not yet a fully validated page-by-page UX map. It must not be turned into a rigid one-way waterfall if learners need safe return loops, targeted refreshers, reassessment, or a different path based on prior evidence.

A professional task should generally cover:

1. Customer need and context.
2. Discovery and clarification.
3. Consultation and bounded advice where appropriate.
4. Confirmation and authorization.
5. Operational execution.
6. Verification of system state and task outcome.
7. Error handling, correction, recovery, or escalation.
8. Customer communication and closure.
9. Evidence and a useful next learning opportunity.

## 4. Product-area purpose and current completeness diagnosis

### 3.1 Home

**Intended job:** orient the learner, show where they are in the journey, surface what needs attention, and make the next useful action obvious. It should connect progress across the five areas without becoming a generic metrics dashboard.

**Documented strength:** its high-level role and cross-product orientation are known.

**Known gap:** detailed information hierarchy, first-time orientation, recommended next action logic, treatment of incomplete/failed tasks, and how Home communicates evidence and prerequisites are not fully specified in the source baseline.

**Fable should test:** Is Home actually useful at first entry and on return? Does it answer “Where am I? What have I demonstrated? What needs attention? What is the next useful step?” without crowding the screen, showing unsupported scores, or duplicating Growth?

### 3.2 Learning — Customer Service Track and Amadeus Track

**Intended job:** build understanding and mental models for both customer-facing work and Amadeus operations, then connect both tracks to integrated professional tasks.

**Documented strength:** the need for both tracks, beginner-first explanations, English-first instruction with Arabic support, and lesson-to-scenario transfer is established.

**Known gaps:** a complete P1/P2 competency map, exact track structures, learning outcomes, topic sequence, lesson-to-task traceability, prerequisites, mastery/progression rules, language progression, and instructional validation are not complete.

**Fable should test:** Are the tracks complementary rather than two disconnected courses? Does Customer Service teach discovery, listening, clarification, advice, confirmation, difficult conversations, and closure? Does Amadeus Track teach operational understanding, state, outputs, pricing/ticketing concepts, error recovery, and verified procedures? Does each lesson prepare the learner for a real task and later assessment? Does the learner demonstrate understanding—not merely finish content?

### 3.3 Terminal

**Intended job:** the operational centre where the learner performs work in the training engine. Scenario execution happens here; cases opened from Scenario Bank should open Terminal in Scenario Mode.

**Documented strength:** the three distinct modes—Practice, Scenario, Independent Assessment—are explicit. Genuine engine output must be separated from DEIXEN instructional guidance. System acceptance is distinct from professional correctness.

**Known gaps:** actual current code and tests have not been inspected in this handoff preparation; Amadeus command coverage and behaviours are not comprehensively verified; initial described workflows are narrow; exact links from case facts and customer decisions to operational validation need testing; recovery, interruptions, and state restoration require implementation inspection.

**Fable should test:** Does Terminal provide a coherent operational workspace? Can a beginner understand the mode and task context without losing the command-centred reality of the work? Are commands, authentic output, system state, errors, warnings, and DEIXEN guidance clearly distinguished? Can the engine detect accepted-but-wrong work at task level? What should be expanded, and what must remain out of Core until verified?

### 3.4 Ghost

**Intended job:** demonstrate real workflows using the same training engine so learners can observe what happens, why it happens, and what state/results follow.

**Documented strength:** Ghost is a demonstration capability, not a top-level page or source of learner competence evidence. It should explain rationale, consequences, and workflow connections; it must not rescue a protected independent assessment.

**Known gaps:** the exact on-screen teaching pattern—what is highlighted, narrated, explained before/after a command, how the learner controls pace, replay, pause, and detail—is not adequately specified in the baseline. The actual demonstration experience must be inspected.

**Fable should test:** Does Ghost explain the terminal screen and operational reasoning, or merely replay commands? Does it show the relationship between command, response, state change, and professional purpose? Can learners control the explanation without being overwhelmed? Is the transition from demonstration to learner execution clear? Does it avoid creating false independence evidence?

### 3.5 Scenario Bank

**Intended job:** organize and present professional cases. It is a case library; execution belongs in Terminal Scenario Mode.

**Documented strength:** case-linked Learning, gradual access based on relevant preparation, customer facts/hidden information, professional and operational criteria, failure/recovery, and variants for transfer are recognized.

**Known gaps:** the canonical case dossier, category/level hierarchy, case discovery UX, prerequisites, case lifecycle, variant design/fairness, professional closure criteria, and full case coverage are not finalized. CP-001 remains HOLD and requires modification plus professional/operational validation.

**Fable should test:** Can the learner understand what a case is for without seeing its protected answers? Are cases built around validated job tasks rather than arbitrary command drills? Does a case preserve continuity from customer dialogue into Terminal and then evidence/Growth? Are there enough case types to test transfer without bloating Core?

### 3.6 Growth

**Intended job:** turn valid performance records into understandable development insight. Growth should show demonstrated capabilities, conditions, assistance, errors/recovery, gaps, and next useful development—not points or an unsupported readiness percentage.

**Documented strength:** evidence integrity and the difference between guided success and independent performance are central.

**Known gaps:** exact learner-facing evidence model, information hierarchy, skill aggregation, correction/history views, continued-development structure, and the minimum honest Evidence Summary / export are not fully specified. Provider/employer access is not approved and must not be assumed.

**Fable should test:** Does Growth answer what the learner can do, under what conditions, how independently, and what still needs evidence? Does it distinguish simulated evidence from practitioner-reviewed evidence and external certification? Is the main view simple while the detailed record remains transparent and accessible?

### 3.7 Coach

**Intended job:** a context-aware professional learning supervisor, helping learners orient, reason, practice, review, and improve—not merely a generic tooltip or answer dispenser.

**Documented strength:** its intended supervisory role, separation from the customer, mode awareness, gradual reduction of assistance, and prohibition on rescuing Independent Assessment are clear.

**Known gaps:** detailed intervention rules, trigger conditions, allowed/prohibited content by mode, recurring error diagnosis, debrief structure, next-step recommendations, and observable Coach success criteria need design and testing. The current Coach was previously described as rule-based; current implementation must be verified.

**Fable should test:** Does Coach help the learner think instead of doing the work? Does it know the exact task/mode/state? Is it predictable and trustworthy? Does it avoid duplicating Ghost? Does it provide the right amount of help at the right moment and then fade?

## 5. Cross-product integration — the central test

The five areas and cross-product capabilities must behave as one connected product, not separate destinations. Fable should map at minimum:

- First-time entry and returning learner routes through Home.
- Learning topic → relevant demonstration → guided practice → scenario/case.
- Scenario Bank case selection → Terminal Scenario Mode with the correct case context.
- Terminal actions/state → task-level validation → performance evidence.
- Assistance/Coach/Ghost exposure → accurate independence and assessment interpretation.
- Attempt result and valid evidence → Growth → recommended next activity → Home.
- Error, interruption, pause/resume, changed customer request, failed attempt, rule correction, and reassessment routes.

The current documents contain the intent and many individual rules, but they do not establish that a complete, tested, end-to-end UX flow already exists. Produce state-aware journey maps and validate them with actual implementation and learners.

## 6. Learning progression and understanding gate

The founder's direction is that a learner should not advance to genuinely new material while lacking the understanding needed for it. This must be translated into a fair, skill-specific progression design—not a simplistic global lock.

Fable should distinguish:

- Exposure to content.
- Comprehension / retrieval evidence.
- Supported execution.
- Independent execution.
- Transfer to a changed situation.
- Valid independent assessment.

A correct answer once, a lesson completion, or a demonstration watched is not enough to establish understanding. Equally, avoid arbitrary percentages, excessive repetition, or blocking a learner from all progress because of one non-critical gap. Define what must be understood before the next dependent task, what may be revisited later, and how the learner is told what remains unclear.

Progression criteria should be tied to the importance and risk of the underlying skill, use multiple appropriate forms of evidence where necessary, and remain understandable to the learner.

## 7. UX quality standard

**Complexity belongs in the system, not in the learner's experience.**

The UX should help a beginner understand:

- Where they are and what mode/state they are in.
- What they need to do now.
- Why it matters and what a good result looks like.
- What the system actually did.
- What help was provided and how that affects evidence.
- What happened when they made an error or could not complete the task.
- What they can do next.

Use progressive disclosure, plain language, consistent interaction patterns, contextual explanations, recovery paths, accessibility, and device-appropriate layouts. Do not solve complexity by hiding important operational or assessment information. Do not add controls, dashboards, animations, badges, avatars, AI, or steps without a demonstrated purpose.

The desktop/laptop is first priority, tablet second, phone third; phone remains useful. English is primary, Arabic support is available in-product. Text must remain a viable alternative to voice. Writing and speaking workplace English are longer-term goals, but the current Core is text-first unless separately authorized and validated. The exact boundary between Arabic assistance and assessment of English skill remains open.

## 8. Cross-company transferability

Use the 2019 Amadeus book to map breadth, not to assume current command truth. Teach the verified common foundation. Clearly separate it from items that can vary by airline, market, date, fare, agency/company policy, office/PCC configuration, permissions, or employer workflow. Variable details may be simulated but must be labelled as illustrative and must not be confused with live data or universal policy. See the English addendum for the verification record and method.

## 9. Evidence model and truth boundaries

Preserve these distinctions:

- Command syntax correctness.
- Operational/system correctness.
- Customer/request/task correctness.
- Professional/business correctness.
- Attempt validity.
- Learner independence and assistance.
- Simulated performance versus practitioner-reviewed evidence versus external certification.

A valid final state is not proof of independence. Coach/Ghost use, hints, errors, recovery, transfer, task conditions, and relevant state changes must be handled in a traceable way. Corrections to rules/results must preserve original history and apply downstream changes according to the approved safeguards.

## 10. Future capabilities — not default Core requirements

The following are candidates to evaluate, not automatic build commitments:

- Evidence Summary / possible Professional Evidence Profile.
- Internal Case & Provenance Validator.
- Practitioner Review Export.
- DEIXEN World / Virtual Company and work-shift assessment.
- LLM-supported natural customer expression and possible voice.
- Coach/avatar and cinematic presentation development.
- Speed/time-to-correct-work analysis.

Each requires a clear use case, evidence of value, UX impact, cost, dependencies, and a scope decision. These must not delay the usable local Core without an explicitly approved reason.

## 11. Current documentary gap summary

These are planning gaps visible from the current documents, not findings about actual running software:

1. Complete P1/P2 job-task and competency map.
2. Detailed Home information hierarchy and next-action logic.
3. Complete Customer Service and Amadeus Track curricula, outcomes, and lesson-to-task traceability.
4. Evidence-based, understandable progression/understanding gates.
5. Comprehensive current Amadeus command/output/state verification.
6. Terminal's task-level correctness and recovery coverage beyond the narrow initial workflow.
7. Ghost's exact screen-explanation pedagogy and interaction design.
8. Canonical case dossier, Scenario Bank information architecture, variants, and professional closure criteria.
9. Growth evidence display, correction history, learner export, and continued-development design.
10. Coach's detailed mode-aware intervention and fading-assistance rules.
11. Complete end-to-end UX maps across all five areas and error/recovery states.
12. Beginner usability/comprehension validation and practitioner validation.
13. Cross-company variable-data and policy simulation framework, including explicit labels and test boundaries.
14. Definition of local Core completion and acceptance criteria tied to real tasks and end-to-end evidence.
15. Verified scope of professional roles and tasks in P1/P2, with P3 kept as a later specialization.
16. A justified split of device-specific experiences and a measurable definition of beginner-friendly UX.
17. Confirmation of practitioner qualifications and review scope, and a fair protocol for the founder plus two beginner trainees.

Fable must verify each gap against the actual application and current source of truth. Some may already be implemented; others may require a better alternative. Do not assume either way.

## 12. Reference source roles

- `05_REFERENCE_ON_DEMAND/DEIXEN_Objectives_and_Founder_Goals_Reference_v0.2.md`: detailed objectives and non-goals.
- `05_REFERENCE_ON_DEMAND/DEIXEN_Product_Feature_Ideas_Inventory_v0.2.md`: detailed page/capability ideas, including future World and Coach concepts; ideas are not automatically approved implementation.
- `05_REFERENCE_ON_DEMAND/DEIXEN_UX_Workflow_Proposal_Register_v2.4.md`: detailed workflow rules and historical proposal-stage detail. Consult targeted sections when a specific lifecycle or safeguard is relevant; do not treat every historical line as current without checking the governing register and approved Workstream C disposition.

These are useful deep references, not three separate documents that Fable must read line-by-line before starting.
