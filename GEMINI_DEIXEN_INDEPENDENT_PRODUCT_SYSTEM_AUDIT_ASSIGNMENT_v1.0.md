# GEMINI ASSIGNMENT — DEIXEN Independent Product-System, End-to-End UX & Software Blind-Spot Audit

**Assignment ID:** DEIXEN-GEMINI-AUDIT-001  
**Version:** 1.0  
**Commissioned:** 20 November 2026  
**Reviewer:** Gemini (independent reviewer; advisory role only)  
**Source repository:** https://github.com/deixenlabs/Gemini-audit-  
**Required branch:** main  
**Primary output:** One downloadable Markdown report attached to Gemini's response.  
**Source-repository write access:** Not authorized. Read only.

---

## 1. Start here: access the repository directly

You are expected to read the source material directly from GitHub. **The founder will not upload the documents into this Gemini conversation. Do not ask the founder to attach, paste, or resend files that are already in the repository.**

1. Open https://github.com/deixenlabs/Gemini-audit- and work from the main branch.
2. Read this assignment from the repository root, then retrieve the referenced source files by their exact filenames. The repository currently presents the curated files at its root; some older README/manifest references may retain the original handoff-folder paths. Locate files by filename rather than assuming those folders exist in this mirror.
3. Confirm the branch and list the files you can actually access. Record the review date and, where available, the commit SHA or file blob SHAs so the review is tied to a known snapshot.
4. If a file cannot be fetched, record the exact filename and access/error condition. Do not silently substitute an older copy, claim it was read, or ask the founder to upload it before completing the work that is possible.
5. Do not edit, delete, rename, commit, branch, open a PR, create an issue, or otherwise change this repository or any project source. This is an independent read-only review.

**Important distinction:** This repository is a curated documentary review package, not the DEIXEN application's source-code repository. It currently contains planning, governance, curriculum, audit, and reference documents—not the live application code. Therefore, you must perform a serious **software/product-engineering requirements and architecture blind-spot audit from the available evidence**, but you must not claim to have discovered or reproduced a code defect unless you genuinely inspected and tested the relevant source code. Do not search or modify other private repositories as a workaround. State clearly what code-level inspection was and was not possible.

### Required report delivery

Create the complete report as a real Markdown file with this filename:

**DEIXEN_Gemini_Independent_Product_System_UX_and_Software_Blind_Spot_Audit_2026-11-20.md**

Attach that file as a **downloadable artifact in your final Gemini response**. Do not provide only an in-chat summary, a code block, or a link that requires the founder to navigate the source repository. The report itself must be complete and self-contained, with source references. Do not commit the report to this source repository. In the final response, include a short verdict and the downloadable file attachment.

---

## 2. Your mission

Produce a rigorous, independent assessment of whether DEIXEN's documented product direction can become a coherent, genuinely useful, beginner-understandable professional training product—and what important product, UX, curriculum, workflow, evidence, or software-design blind spots could prevent that outcome.

Do not merely answer the founder's stated questions or repeat previous reviewers. Challenge the assumptions, test the completeness of the whole system, look for overlooked failure paths, and identify stronger alternatives where the evidence supports them.

The required outcome is **the strongest useful DEIXEN with the simplest coherent learner experience**. The goal is not to maximize feature count, novelty, AI use, cinematic content, technical sophistication, or the length of the roadmap.

Your review must answer all of these overarching questions:

1. Is the product's purpose translated into a complete, coherent, realistic learning-to-work system?
2. Do the five product areas and shared capabilities work together as one product rather than as separate feature collections?
3. Can a true beginner understand where to start, what to do, why it matters, what happened, and what to do next without being exposed to unnecessary system complexity?
4. Does the product cover meaningful professional work—not just command entry or successful final states?
5. Are learning, demonstration, assistance, progression, assessment, independence, evidence, and growth logically connected and fair?
6. Are there missing workflows, product capabilities, rules, data concepts, system states, validations, tests, or safeguards that could cause serious problems when implemented or used?
7. Which existing elements deserve to stay, improve, be rethought, replaced, combined, simplified, deferred, or removed?
8. Are there any genuinely valuable new capabilities that are not in the current plans? Recommend them only when they solve a demonstrable problem better than improving an existing capability.
9. What is the smallest complete and trustworthy local Core, and what must remain later or out of scope?
10. What needs founder approval, what belongs to Fable's delegated technical authority, and what still requires external evidence?

Be critical rather than agreeable. A finding is valuable only when it is grounded, specific, consequential, and actionable.

---

## 3. DEIXEN baseline you must preserve while testing it

Use the source documents to validate and refine the following baseline. It is a starting understanding, not a reason to protect weak design.

### 3.1 Product purpose

DEIXEN is intended to develop a beginner toward demonstrable professional capability in travel and reservations operations, beginning with Amadeus. It is not intended to be only a generic LMS, a command-memorization course, an isolated GDS terminal, a free-form chatbot, or an entertainment game.

A professional task can involve understanding the customer, asking and clarifying, identifying constraints, advising within verified information and bounded alternatives, confirming the customer's choice and authorization, executing the operational work, checking the actual result/state, handling errors or changes, communicating clearly, and closing or following up appropriately.

The founder's central problem thesis is:
- good Amadeus learning can be expensive or difficult to access;
- knowing commands is not the same as performing travel-operations work;
- weak practical preparation may reduce a candidate's competitiveness;
- superficial progress systems can reward completion without establishing understanding, independence, or genuine progression.

Other proposed problems—such as difficulty knowing where to start, confusing explanations, weak error recovery, hidden skill gaps, poor transfer to unfamiliar tasks, or insufficient workplace English—are hypotheses to test, not automatic reasons to add features.

### 3.2 Current product structure

The documented product model has five top-level areas:

- **Home** — orientation, status, and the next useful action. Its detailed hierarchy and exact naming remain open to evaluation.
- **Learning** — structured Customer Service Track and Amadeus Track, linked to practical tasks and cases.
- **Terminal** — the operational workspace, with exactly three distinct modes: **Practice, Scenario, and Independent Assessment**.
- **Scenario Bank** — professional case discovery and selection. A case is executed through Terminal Scenario Mode, not as a disconnected activity.
- **Growth** — understandable development and credible evidence, not decorative points or unsupported readiness percentages.

**Ghost** and **Coach** are cross-product capabilities, not additional top-level areas. **DEIXEN World / Virtual Company** is a possible future Scenario Bank experience, not a sixth top-level area and not a prerequisite for the local Core.

Do not collapse the three Terminal modes into one mode with assistance levels. Their assistance policies may be refined, but the mode distinction and independent-assessment protections must remain unless the founder explicitly approves a product-level change.

### 3.3 Learning and integrity principles

The intended learning architecture is:

Learning → Demonstration/Ghost → Guided Practice → Independent Practice → Scenarios → Independent Assessment → Evidence → Growth/continued development.

This is a pedagogical architecture, not proof of a complete or mandatory one-way user journey. Safe return loops, targeted refreshers, reassessment, and non-linear routes may be necessary.

Preserve these distinctions:
- an action is not automatically a qualifying action;
- lesson completion is not proof of understanding;
- assisted performance is not independent competence;
- Independent Practice is not automatically Independent Assessment evidence;
- a correct final state alone does not prove who did the work or how independently;
- requesting help is not the same as help being delivered;
- system acceptance is not the same as operational correctness;
- operational correctness is not the same as fulfilling the customer's request;
- customer satisfaction is not a substitute for professional correctness.

Avoid arbitrary readiness percentages and single scores that hide critical failures. Evidence should describe what was demonstrated, under what conditions, with what assistance, and what remains unproven.

### 3.4 Truth, simulation, and AI boundaries

The current documented Core direction is deterministic-first; do not assume an LLM runtime already exists. If a future LLM is proposed, it may support natural expression or bounded customer-persona variation, but it must not invent case facts, booking data/state, Amadeus truth, command outcomes, correctness, assessment decisions, or evidence.

Keep authentic Amadeus output separate from DEIXEN guidance. Unknown behavior must remain unknown or clearly labeled as simulated; do not fabricate plausible-looking operational output.

Teach the transferable, verified common foundation while clearly representing differences due to airline, market, date, fare, product, agency/company policy, office/PCC configuration, permissions, and employer workflow. A simulated variable must be disclosed as fictional or illustrative, not presented as a universal or live rule.

Simulation is not actual workplace experience. Do not claim guaranteed employment, universal workplace readiness, external certification, employer acceptance, official Amadeus affiliation, or partnership without genuine evidence and authorization.

### 3.5 Priority and decision boundaries

P1 and P2 are both current core priorities. P3 is advanced specialization for later consideration after P1/P2 are adequately mapped, implemented, and validated. Do not expand or delay the Core by prematurely pulling P3 into it.

The founder retains product-level authority over purpose, objectives, professional promise, target users/markets, curriculum promise, material Core scope, learner journey, assistance/assessment meaning, and strategic direction. Material changes in these areas require an explicit founder decision.

Fable 5.2 is the sole DEIXEN project lead. Technical and implementation decisions are delegated to Fable. Gemini is an independent reviewer, not a parallel project lead, architect, product owner, or implementation agent. Your report is advisory evidence for the founder and Fable; do not present your recommendations as approved decisions.

---

## 4. Source-of-truth and evidence discipline

Read the current founder-authority document first. Use this precedence when interpreting the source package:

1. **DEIXEN_Current_Founder_Authority_and_Product_Direction_v1.1.md** — current consolidated owner authority and direction.
2. **DEIXEN_Workstream_C_Consolidation_Proposal_v0.1_2026-11-20.md** — the founder-approved consolidation approach and reconciled review dispositions, interpreted under the current authority register. Preserve distinctions between what was approved, what remains a proposal, and what requires external evidence.
3. **DEIXEN_Amadeus_Curriculum_and_Cross_Company_Transferability_EN.md** — current owner direction for curriculum scope, transferability, and the boundary between book coverage and current Amadeus truth.
4. **DEIXEN_Product_Baseline_and_Documentary_Completeness_Review_v1.0.md** — curated product baseline and known documentary gaps; it is not proof of current implementation.
5. **DEIXEN_Objectives_and_Founder_Goals_Reference_v0.2.md**, **DEIXEN_Product_Feature_Ideas_Inventory_v0.2.md**, and **DEIXEN_UX_Workflow_Proposal_Register_v2.4.md** — detailed planning references. Check them against the newer authority and reconciliation; do not treat every item as approved or current.
6. The Sonnet and Argon reports — independent reviewer evidence and recommendations, not owner authority. Challenge them where appropriate; do not simply reproduce their findings.
7. **README.md**, **START_HERE_FABLE_HANDOFF_v1.1.md**, **PACKAGE_MANIFEST_AND_CURATION_RECORD_v1.1.md**, and **FABLE_First_Assignment_Read_Only_Product_Audit_and_Development_Plan_v1.1.md** — package context and Fable's remit. The Fable-specific assignment is **not an assignment to Gemini**. Read it only to understand the division of responsibility and the intended next project phase.

Where documents conflict, record the exact conflict, compare dates and explicit approval status, and explain the controlling interpretation. Do not silently resolve a material product ambiguity by personal preference. Separate:
- owner-approved direction;
- founder-endorsed strategic candidate;
- reviewer recommendation;
- historical or superseded proposal;
- open hypothesis;
- external evidence requirement;
- your own new recommendation.

### 4.1 Required evidence labels

Label each material statement as one of:
- **Documented fact** — directly supported by a specific source.
- **Documentary gap** — required detail is not sufficiently specified in the reviewed material; this does not prove that the live application lacks it.
- **Document conflict/ambiguity** — sources disagree or leave a material decision unclear.
- **Inference/risk hypothesis** — a reasoned concern derived from the sources, not yet verified in implementation.
- **Implementation verified** — only when you genuinely inspected the relevant live code or ran a reproducible test; state exactly what was inspected.
- **External validation required** — needs current Amadeus evidence, a practitioner, learner testing, market evidence, legal/security review, or another external source.

For each finding, provide precise evidence: filename, section/heading, and page/line reference or a direct GitHub link where possible. Do not cite a whole large document when a specific section supports the point. Do not invent line numbers or source references.

### 4.2 Known review limitations to preserve

- The package was prepared as a documentary handoff; it did not inspect the current application source code or test the live Amadeus environment.
- Argon's Phase 2 summary and PV ledger disclose their own inspection scope and limitations. Preserve them; they are not a live-code or live-Amadeus audit.
- Sonnet's product/UX audit did not inspect the application code. Its competitive report disclosed limitations in hands-on competitor testing and regional market evidence. Do not upgrade those claims into established facts.
- EV-01 (Amadeus operational truth) and EV-02 (practitioner review) are separate evidence gates. Do not treat one as satisfying the other.
- EV-01–EV-06 remain open unless the required evidence is actually present and the closure is justified.

---

## 5. Mandatory repository reading plan

Do not bulk-read without a method, but do not skip relevant material to save tokens. Start with the short governing documents, then inspect the detailed source files by section. Your report must list every repository file and classify it as **read in full**, **read in relevant sections only**, **metadata/structure only**, or **not read**, with a brief reason. Include the SHA/commit snapshot where available.

### 5.1 First-pass documents — read in full

1. **DEIXEN_Current_Founder_Authority_and_Product_Direction_v1.1.md**
2. **DEIXEN_Product_Baseline_and_Documentary_Completeness_Review_v1.0.md**
3. **DEIXEN_Workstream_C_Consolidation_Proposal_v0.1_2026-11-20.md**
4. **DEIXEN_Amadeus_Curriculum_and_Cross_Company_Transferability_EN.md**
5. **DEIXEN_Objectives_and_Founder_Goals_Reference_v0.2.md**
6. **README.md**
7. **PACKAGE_MANIFEST_AND_CURATION_RECORD_v1.1.md**
8. **START_HERE_FABLE_HANDOFF_v1.1.md**
9. **FABLE_First_Assignment_Read_Only_Product_Audit_and_Development_Plan_v1.1.md** (context only; not your instructions)
10. **SHA256SUMS.txt** (understand the supplied package integrity manifest; do not let it displace product review)

### 5.2 Detailed references — inspect systematically

11. **DEIXEN_Product_Feature_Ideas_Inventory_v0.2.md** — inspect all sections relevant to product areas, Coach/Ghost, World, customer simulation, task runtime, work-shift assessment, current reality, end-to-end UX, priorities, and open decisions. Treat ideas as candidates, not approved features.
12. **DEIXEN_UX_Workflow_Proposal_Register_v2.4.md** — inspect the complete structure and the detailed sections relevant to task lifecycle, case lifecycle, mode/assistance rules, assessment start and fairness, exposure, evidence, corrections, recovery, privacy, navigation, and integration. In particular, reconcile Stages 147/148 and 150–155 with Workstream C and the current authority register.
13. **Sonnet_Independent_Strategic_Product_UX_Workflow_Audit.md** — review the full findings and the source coverage/limitations; test the findings independently.
14. **Sonnet_Independent_Competitive_Positioning_Review_Revised_v2.md** — review the strategy, feature candidates, claims discipline, and research limitations; do not turn limited market research into proof.
15. **Argon_Phase2_Integrated_Findings.md** — review all integrated findings and limitations.
16. **Argon_Phase2_Evidence_Traceability_Ledger_PV001-PV034.md** — inspect the relevant PV entries and source references, especially Amadeus boundaries, task/runtime lifecycles, semantic validation, CP-001, product areas, curriculum, competence, validation backlog, and assessment/Coach boundaries.

If the actual repository listing differs from this list, report the difference accurately and continue with accessible files. Do not state that a document is absent if it exists under another root-level filename.

---

## 6. Required audit workstreams

### A. Product completeness and system coherence

Audit all five areas—Home, Learning, Terminal, Scenario Bank, and Growth—as one integrated product. Also audit Ghost and Coach as cross-product capabilities and evaluate future DEIXEN World as a possible Scenario Bank mode.

For each area/capability, answer:
- What specific learner or professional problem does it solve?
- What is its single primary responsibility, and what must it not own?
- What does the learner need to understand or accomplish there?
- What information/state must enter it, and what must it hand to other areas?
- What are the start, success, failure, pause, exit, and recovery states?
- What does the current documentation establish, leave open, or contradict?
- Is it sufficiently useful and complete for the Core, or is the purpose better achieved by improving another capability?
- What is the simplest coherent design that meets the need without hiding meaningful complexity?

Do not assume the interface, page names, navigation, or feature inventory are optimal merely because they are documented.

### B. End-to-end learner and professional-work journeys

Map at least these connected journeys with explicit transitions, decisions, information, prerequisites, system feedback, and recovery routes:

1. **First-time learner:** orientation → starting point → first useful learning action → comprehension check → demonstration → practice → next meaningful action.
2. **Learning to operational ability:** Customer Service Track and Amadeus Track → Ghost → guided practice → independent practice → case application → evidence of what was actually learned.
3. **Scenario execution:** Scenario Bank discovery → case understanding/neutral briefing → customer interaction → clarification and choice → customer confirmation/authorization → Terminal Scenario Mode → result/state verification → professional closure → task/evidence result → Growth and next learning action.
4. **Independent assessment:** eligibility → preview/briefing → explicit start/commit → protected execution → interruption/recovery → result validity → debrief → correction/reporting where appropriate → reassessment or next opportunity.
5. **Continued development:** completed evidence → visible skill strengths and gaps → appropriate next opportunity → refreshed learning → new/changed case → durable progress history.
6. **Future Virtual Company/work shift (evaluate as FUTURE, not assumed Core):** entry into a work environment → multiple customer interactions → task switching/interruption → operational execution → exception/escalation → end-of-shift review and Shift Evidence Record. Define what would make this meaningfully better than the text scenario flow and what must be proven before building it.

For each journey, identify:
- missing links or duplicated responsibilities;
- points where learners may not know what to do next;
- where information is lost, repeated, contradicted, or prematurely disclosed;
- cases that end correctly without a booking or ticket;
- abandoned, paused, interrupted, failed, partially completed, or uncertain operations;
- stale state, navigation return, session restoration, and retry behavior;
- opportunities to simplify the learner's experience without weakening evidence or controls.

Do not force every learner into a single rigid waterfall. Identify useful return loops and alternative routes while retaining transparent prerequisites.

### C. Professional task, curriculum, and Amadeus coverage

Treat a professional task—not an isolated command—as the organizing unit. Map the intended task lifecycle from understanding the request through closure/follow-up. Distinguish customer-service competencies from Amadeus operational competencies while showing how they combine in work.

Review the supplied Amadeus index transcription in Appendix A as a **topic-coverage map only**. For each topic or meaningful cluster:
- preserve its printed page references and original wording;
- map it to a candidate professional task and skill;
- propose P1, P2, P3, or out-of-scope/needs research classification with rationale;
- identify prerequisites and how it connects to other topics;
- identify whether it is likely common foundation, product/airline/market/date dependent, agency/company policy, office/PCC/permission dependent, synthetic training content, or still ambiguous;
- state what current evidence would be needed before teaching exact syntax or outcomes.

Do not assume every topic belongs in Core or should be taught to equal depth. Do not delete advanced topics from the coverage map just because they may be deferred. Identify professional tasks and competencies not represented by the book index. The book itself has intentionally **not** been uploaded to this repository; this is a deliberate time/token-saving choice, not a documentary defect and not a reason to block the audit. Do not ask the founder to upload the book. The founder-provided index transcription below is the available scope reference for this review. It does not mean that the complete book has been read or that any command has been verified.

Keep two distinct workstreams separate:
- curriculum breadth/topic mapping based on the index;
- current operational verification of syntax, preconditions, outputs, state transitions, errors, and exceptions.

The book is attributed to 2019 and cannot establish current Amadeus behavior. Use current authoritative sources and authorized practical testing for operational claims. Where external research is used, cite exact sources and dates and label what remains uncertain. Do not invent a response or claim a command is valid based on memory alone.

Examine the full range suggested by the index—not only a narrow booking slice—including access, encode/decode, information, availability/schedule/timetable, names, itinerary, PNR retrieval and elements, optional elements, frequent flyer, groups, queues, copy/print, APIS/passport, booking, pricing, ticket issuance and ticket elements, taxes, payment, endorsement, commissions, tour code, validating carrier, invoice, ticket copies, action identifiers, booking classes, meals, codeshare/alliance, ticket structure, FXD, EMD, sales reporting, passenger-count mismatch, excess baggage, penalties, infant addition, mileage, agent/agency information, refund, reissue, automated reissue, history, remarks, modifications, BSP, and other indexed topics. This list is a reading aid; preserve the actual index entries in Appendix A.

### D. Terminal, simulator, and operational truth

Audit the Terminal as the operational center, not merely a command box. Review:
- three distinct modes and their permissions/assistance boundaries;
- command input, guidance, response, state transition, and task validation;
- the difference between authentic output, simulated output, and DEIXEN training guidance;
- syntax errors versus invalid operational state versus professional/task mismatch;
- recovery, warnings, unknown results, partial success, duplicate submissions, retries, timeouts, and uncertain transaction outcomes;
- how the learner understands current PNR/session/task state;
- what data is authoritative and how it changes;
- how customer authorization and task decisions are represented separately from system elements;
- how pricing/ticketing, refund/reissue, EMD, queues, history, and other advanced flows are scoped and sequenced.

Keep these four correctness dimensions separate:
1. Command/syntax correctness.
2. Operational/system-state correctness.
3. Customer-request/task correctness.
4. Professional/business correctness.

Review known sensitive boundaries as questions to verify, not as facts to assume: RF as a PNR Received From element versus customer authorization; ER/ET end-transaction behavior; FXP versus FXX pricing/TST behavior; pricing persistence; ignored/off-path recovery; PNR state and history; and ticketing/refund/reissue boundaries. Use the Argon PV records to locate the concerns, then assess exactly what is supported and what still requires EV-01.

CP-001 remains HOLD. The bounded advice-and-choice step between prepared alternatives is not live availability search or full fare shopping. Do not treat it as validated or expand its scope without approval.

### E. Learning design, Coach, Ghost, and progression

Evaluate whether learning creates usable mental models, not just command recall. Check:
- clear explanations of terms, purpose, preconditions, consequences, and expected results;
- sequencing and prerequisite logic across both tracks;
- meaningful retrieval and comprehension checks;
- progression based on appropriate understanding/performance evidence rather than clicks, lesson completion, or arbitrary percentages;
- controlled practice and gradual reduction of assistance;
- transfer to altered cases rather than memorization of rehearsed paths;
- fair treatment of mistakes, retries, prior knowledge, and reassessment;
- language support and accessibility without accidentally measuring English when the task is measuring operations.

For Ghost, assess whether it explains the screen, reasoning, command, response, and resulting state—or merely replays commands. For Coach, assess whether it behaves like a coherent, context-aware supervisor: knows the learner's mode and state, supports thinking rather than doing the task, gives the right amount of help at the right time, diagnoses recurring issues, fades assistance, and does not duplicate Ghost or rescue Independent Assessment. Every Coach intervention must have a defined trigger, allowed content, prohibited content, and effect (or non-effect) on evidence.

### F. Assessment, evidence, fairness, and provenance

Audit the entire evidence chain and its causal meaning. In particular, examine:
- the distinction among Task Run, Attempt, and Operational Session/PNR lifecycle; do not assume these can be merged merely to simplify the data model;
- eligibility and prerequisite snapshots at attempt start;
- whether previews create attempts or allow protected commands before start commit;
- idempotent start identity and duplicate start prevention;
- authoritative eligibility recomputation at the start boundary;
- stale previews, lost eligibility, and restored eligibility behavior;
- the six guarantees reconciled in Workstream C Stages 150–155;
- prospective effect of prerequisite corrections under Stages 147/148, without retroactively invalidating a valid already-completed attempt solely because a prior prerequisite was corrected;
- original results and rule versions retained through additive, traceable corrections;
- separation of content delivery, actual display/exposure, audit records, policy effects, and derived results where needed for causal fairness;
- assistance requested versus assistance delivered;
- Coach/Ghost exposure and protected-content disclosure;
- variant fairness, transfer opportunities, skill-level versus overall validity, and reassessment;
- customer outcome versus learner performance;
- evidence summaries that clearly state conditions and limitations.

A case that correctly ends without a reservation, ticket, or transaction must be representable as a valid professional outcome where appropriate. Customer satisfaction cannot repair an operational error, and a correct booking cannot erase poor customer handling.

### G. Software/product-engineering blind-spot audit

Because this repository contains documentation rather than application source code, inspect the specifications for missing engineering contracts, unsafe assumptions, untestable behavior, and high-risk design gaps. Do not report these as confirmed code defects. Consider at least the following domains and include only issues that are relevant to DEIXEN and supported by evidence or a clear, explicitly labeled risk hypothesis:

1. **Domain model and lifecycle integrity:** boundaries among learner, task, case, attempt, task run, operational session/PNR, command execution, customer dialogue, evidence, and derived progress.
2. **State machines and invariants:** valid/invalid transitions, preconditions, terminal states, cancellation, partial completion, uncertain outcomes, stale state, retries, idempotency, race conditions, and recovery.
3. **Deterministic operational engine:** command catalog/versioning, syntax parsing, preconditions, state mutation, output generation, error taxonomy, unsupported commands, and golden test fixtures. How is authentic Amadeus behavior kept separate from synthetic training behavior?
4. **Source-of-truth separation:** case facts, customer intent, authorization, operational state, company/airline policy, training guidance, assessment rules, and learner evidence must not accidentally overwrite or impersonate one another.
5. **LLM isolation (future):** if introduced, how are model outputs prevented from changing scenario facts, commands, bookings, state, correctness, assessment, or evidence? How are prompt injection and untrusted customer/learner text contained? Do not assume LLM use is currently implemented.
6. **Event history and provenance:** immutable or versioned records where required, derived projections, corrections, auditability, rule-version snapshots, replay/recomputation, and causal links from action to outcome.
7. **Eligibility and assessment integrity:** protected-mode boundaries, authorization checks, assistance channels, disclosure, variant assignment, eligibility races, assessment start atomicity, and reproducible fairness tests.
8. **Data quality and content operations:** competency/case/command/version links, source provenance, validity dates, scope of applicability, reviewer status, stale guidance, and how content updates are approved and tested.
9. **Privacy and security:** personal/passenger data, synthetic versus real data, minimization, tenant/learner separation, access controls, consent, evidence export/sharing, retention/deletion, secrets, logs, and misuse of downloadable evidence. Identify needs for specialist review without inventing legal conclusions.
10. **Reliability and resilience:** local storage limitations, persistence boundaries, browser refresh, offline behavior, crashes, timeouts, duplicate actions, backup/recovery, migration, future backend concurrency, and failure messaging.
11. **Testability and quality assurance:** unit/integration/contract/state-machine/property/regression tests, end-to-end learner journeys, command golden transcripts, seeded cases, fairness tests, accessibility tests, and release acceptance criteria.
12. **Observability and supportability:** diagnostic information sufficient to investigate failure without exposing sensitive data or leaking protected assessment content.
13. **UX implementation risks:** empty/loading/error/warning/disabled states, keyboard and screen-reader access, focus management, responsive behavior, localization, terminology, reduced motion, interruption and restoration, and error recovery.
14. **Scalability and maintainability:** content authoring/versioning, airline/company variation, future GDS extensibility without premature abstraction, feature flags, schema evolution, migration, and test fixture maintenance.
15. **Performance and operational cost:** what can run locally, what must be server-authoritative later, any expensive or fragile dependency, and the risk of introducing a complex architecture before Core value is established.

For each relevant blind spot, state the missing contract or invariant, why it matters to the learner/business/trust, the failure scenario, the affected areas, the best minimal safeguard, and how to test it. Avoid generic software checklists detached from the DEIXEN domain.

### H. UX simplicity, accessibility, and interaction quality

Apply the product-wide principle: **complexity belongs in the system, not in the learner's experience.** The learner should be able to understand where they are, which mode they are in, what the task means, what is expected, what happened, and what is next—without being forced to understand internal architecture.

Inspect:
- first-use orientation and mental model;
- navigation and location awareness;
- information hierarchy and progressive disclosure;
- clear mode and assistance indicators;
- terminology, bilingual support, and translation boundaries;
- content density, decision burden, repeated steps, unnecessary clicks, and competing calls to action;
- error/warning presentation and recoverability;
- evidence transparency without overwhelming the main flow;
- keyboard, focus, contrast, screen-reader, text resizing, and reduced-motion requirements;
- desktop/laptop-first design with appropriate tablet and phone behavior rather than blindly shrinking a desktop interface;
- any cinematic/voice/avatar proposal's learning value, interruption cost, accessibility, performance, and text fallback.

Do not equate fewer clicks, visual polish, gamification, or enjoyment with good UX. Do not recommend hiding important consequences or evidence in the name of simplicity.

### I. Existing features and new feature opportunities

Review all current and proposed capabilities, including but not limited to:
- Home/orientation and next-action logic;
- Customer Service Track and Amadeus Track;
- Terminal and the three modes;
- Scenario Bank and case dossier/lifecycle;
- Ghost demonstration;
- Coach/supervisor and its possible non-human avatar;
- Growth and learner-controlled evidence;
- Evidence Summary / possible Professional Evidence Profile;
- Case & Provenance Validator;
- Practitioner Review Export;
- DEIXEN World / Virtual Company and shift assessment;
- voice, customer personality/interruptions, cinematic scenes, and text fallback;
- speed/time-to-correct-work concepts;
- any other opportunity you discover.

For every major candidate, decide whether it is:
- an essential Core requirement;
- a better way to improve an existing feature;
- a useful later capability;
- a future experiment that requires evidence;
- unnecessary, duplicative, or actively harmful;
- not yet assessable.

A proposed feature must identify the concrete problem, target user, expected observable benefit, why an existing feature cannot solve it, best simpler alternative, dependencies, build/maintenance/validation cost, UX and cognitive-load impact, risks to assessment/evidence, and what evidence would justify investment. Do not add a feature merely because a competitor has it or because AI/3D/voice is available.

### J. Competitive and commercial claims — bounded review

Assess whether the proposed differentiation is coherent and potentially valuable, but keep the strength of the conclusion proportional to the available market evidence. Distinguish:
- product logic that appears differentiating;
- features that are table stakes;
- market hypotheses;
- verified competitor capabilities;
- untested competitor claims;
- willingness-to-pay, employer/provider acceptance, and regional demand that remain unproven.

Do not redo a broad market report unless you find a material gap that changes the product recommendation. Use current primary sources when making fresh market, legal, regulatory, or competitor claims; cite publication dates and exact evidence. Do not make pricing, launch-market, partnership, or employment claims as facts.

---

## 7. Required software blind-spot and failure-path register

Create a consolidated register of the most consequential risks. Do not split one root cause into many repetitive findings. Each finding must use this structure:

| Field | Required content |
|---|---|
| ID | Stable unique ID, e.g. GEM-SW-001 or GEM-UX-001 |
| Title/category | Plain-language issue and product/engineering domain |
| Evidence status | Documented fact, documentary gap, conflict, risk hypothesis, implementation verified, or external validation required |
| Source evidence | Exact file, section, and page/line or GitHub link |
| Finding | What is missing, weak, contradictory, or potentially unsafe; be precise |
| Failure scenario | A realistic example of what could go wrong and who is affected |
| Impact/severity | P0 Critical / P1 High / P2 Medium / P3 Low, with a reason |
| Confidence | High / Medium / Low and why |
| Affected areas/dependencies | Screens, tracks, Terminal modes, data lifecycles, evidence, integrations, etc. |
| Best response | KEEP / IMPROVE / RETHINK / REPLACE / COMBINE / REMOVE / VALIDATE / DEFER, with a specific recommendation |
| Simpler/stronger alternative | State the best alternative; do not list options without choosing a recommendation |
| Validation | The test, source, practitioner review, or learner experiment that would confirm or reject it |
| Acceptance criterion | Observable result that would show the issue is resolved |
| Decision authority | Fable technical decision / founder product approval / external evidence or specialist sign-off |

Severity guidance:
- **P0 Critical:** could invalidate assessment/evidence, create materially false operational output, corrupt important state/history, expose sensitive data, or make the core task untrustworthy.
- **P1 High:** blocks coherent Core use, creates a major beginner/operational failure, or leaves a key competence untestable.
- **P2 Medium:** material quality, recovery, accessibility, maintainability, or later-pilot issue that can be sequenced after higher-risk foundations.
- **P3 Low:** refinement or optional future improvement.

Do not inflate severity to make the report look important. Do not assign severity without explaining impact. Record a risk as unverified where it is not demonstrated.

Also provide a compact **cross-dependency map** for the highest-risk items so that fixing one area does not silently damage another (for example: Coach help → exposure → assessment eligibility → evidence → Growth; or customer authorization → Terminal action → operational state → professional validation → task result).

---

## 8. Required product disposition and roadmap

Create one integrated disposition matrix covering all five areas, Ghost, Coach, the major shared systems, and the most important feature candidates. Use the founder's categories:

- **KEEP** — sound and useful as-is.
- **IMPROVE** — preserve the purpose but strengthen the mechanism/UX.
- **RETHINK** — the current framing or design may be wrong.
- **REPLACE** — recommend a stronger alternative.
- **COMBINE** — overlapping responsibilities should be integrated.
- **REMOVE** — no sufficient value or creates more harm/complexity than benefit.
- **VALIDATE** — cannot responsibly decide without specific evidence.
- **DEFER** — potentially valuable but not necessary for the current Core.

Every row needs: current purpose, evidence-backed assessment, proposed disposition, learner/business value, risk/dependency, and decision authority. Do not force a change where the current approach is already strong.

Then propose a phased order with explicit dependencies:

1. **Core foundations / NOW:** what must be defined or validated for a usable, coherent local Core and why.
2. **Core completion / NEXT:** what must be completed before meaningful beginner and practitioner validation.
3. **Later / AFTER evidence:** what should wait until the Core has proven value or has a specific dependency.
4. **Future / experimental:** World/Virtual Company, LLM, voice, advanced cinematic systems, or other expansion only where justified.
5. **Do not build:** elements that are duplicative, premature, distracting, or unsupported.

Do not invent fixed delivery dates or effort estimates unless you can support them. Show sequencing, dependencies, and exit criteria instead. Preserve both P1 and P2 as current core priorities; P3 remains later specialization unless a founder-approved reason changes that.

Define a testable local-Core completion standard that distinguishes:
- functional implementation;
- verified operational behavior;
- instructional/pedagogical adequacy;
- beginner usability;
- professional/practitioner validity;
- assessment/evidence integrity;
- production readiness (including Backend/security/reliability).

A local Core can be functionally complete while still awaiting other evidence gates. Do not conflate those states.

---

## 9. Required validation plan

For every P0/P1 and key P2 finding, propose the smallest high-value validation that can confirm or reject it. Include:

- **Amadeus truth (EV-01):** source and environment evidence needed for command syntax, preconditions, outputs, state, errors, and recovery.
- **Practitioner review (EV-02):** competencies, job tasks, professional correctness, policy boundaries, and the reviewer's qualifications/scope.
- **Curriculum/job-task coverage (EV-03):** P1/P2 competencies, task map, depth, sequencing, and traceability.
- **Beginner usability (EV-04):** observed first-use and task performance with genuine beginners; do not overgeneralize from the founder.
- **Transfer and fairness (EV-05):** changed variants, disclosure, assistance, interruptions, prior knowledge, and assessment validity.
- **Market/provider/employer evidence (EV-06):** separate demand, willingness to pay, adoption, and acceptance questions; do not claim proof from a few postings or interviews.

For product UX, propose realistic scenarios and observation questions rather than satisfaction-only surveys. Capture where users hesitate, misunderstand, need help, make a wrong decision, lose state, cannot recover, or believe they succeeded when they did not.

For software-design risks, define explicit invariants and tests where useful (for example: a preview must never create an attempt; duplicate start must not create two attempts; a command must not execute before the assessment-start boundary commits; help requested but not delivered must not be recorded as delivered; later prerequisite correction must not retroactively invalidate a completed valid attempt under the approved rule). These are illustrative safeguards from the documented direction—verify exact semantics against the governing documents before recommending changes.

---

## 10. Report structure and quality standard

The downloadable report must be complete but not padded. Use this structure:

1. **Executive verdict** — clear overall assessment; strongest parts; top risks; whether the current product plan is coherent enough to proceed and what must be resolved first.
2. **Scope, repository snapshot, and evidence limits** — branch/commit, files accessible, what was read fully/partially/not read, and whether any code was inspected.
3. **Controlling product baseline** — concise separation of approved directions, candidate features, hypotheses, and unresolved matters.
4. **Whole-product completeness matrix** — Home, Learning, Terminal, Scenario Bank, Growth, Ghost, Coach, and cross-product connections.
5. **End-to-end journey analysis** — the required journeys, key states, breaks, loops, and recovery.
6. **Curriculum and professional task coverage** — index mapping, P1/P2/P3 recommendations, unrepresented competencies, and operational verification needs.
7. **Assessment/evidence/fairness review** — lifecycle, eligibility, assistance, exposure, variant integrity, corrections, and evidence meaning.
8. **Software/product-engineering blind-spot register** — prioritized, DEIXEN-specific, explicitly separated from confirmed code defects.
9. **Feature opportunity and disposition matrix** — existing features and only genuinely justified additions.
10. **UX, accessibility, and cognitive-load review** — learner-visible impact and concrete alternatives.
11. **Founder decision items and Fable-delegated technical items** — separate product approval from technical execution; show the evidence and trade-offs.
12. **Prioritized roadmap and local-Core acceptance standard** — dependencies and exit criteria, not unsupported dates.
13. **Validation plan** — experiments/tests mapped to EV-01–EV-06 and the key risks.
14. **What should remain unchanged** — protect sound decisions and safeguards; do not create churn for its own sake.
15. **Limitations and unresolved questions** — what you could not establish and why.

The report must include:
- one consolidated findings register without repetitive duplicates;
- a compact area disposition table;
- a compact feature opportunity table;
- a dependency/risk map for the top issues;
- source citations/references next to claims;
- a short list of the **top 5 founder-level decisions**, only if actual decisions are required. Do not manufacture decisions where Fable can decide technically or where evidence should be gathered first.

### Quality checks before delivery

Before attaching the file, verify that:
- every finding is grounded or explicitly labelled as a hypothesis;
- no documentary gap is falsely described as a confirmed app defect;
- no existing feature is called absent without checking all relevant source documents;
- no unapproved proposal is described as a decision;
- no market, employment, certification, Amadeus, or practitioner claim exceeds its evidence;
- the three Terminal modes and the owner/Fable authority boundary are preserved;
- the book index is treated as a scope map, not as proof of current command behavior;
- the report does not ask for the book PDF or claim its absence is a gap;
- repeated findings are merged into root causes with cross-references;
- each recommendation explains trade-offs, dependencies, and how to validate it;
- the report clearly distinguishes NOW, LATER, FUTURE, and OUT OF SCOPE;
- the report is a real downloadable file, not merely text in the Gemini conversation.

---

## Appendix A — Founder-provided transcription of the 2019 Amadeus book index

**Use:** Curriculum topic-coverage map only. The original book PDF is intentionally not present in this repository to save review time and context. This transcription is supplied by the founder for the audit. It does not establish that the reviewer or founder has read the full book, and it does not verify any command or procedure. Preserve the headings and page references as supplied; spelling, ambiguity, duplicates, and overlapping page entries are part of the source record. Do not silently correct or infer ambiguous headings. You may flag a possible typo or interpretation separately and explain what would verify it.

| Printed page | Index entry as supplied |
|---:|---|
| 1 | الفهرس |
| 2 | Alphabet |
| 3 | الدخول الى سستم اماديوس |
| 4 | الدخول الى سستم اماديوس |
| 5 | الدخول الى سستم اماديوس |
| 6 | Encode & Decode |
| 7 | التاريخ و الوقت والالة الحاسبة |
| 8 | الوقت الكافى بين رحلتين |
| 8 | Amadeus Information |
| 9 | Avilability |
| 9 | Schedule |
| 10 | Timetable |
| 11 | Name |
| 12 | Divid |
| 12 | المساعدة المباشرة HE |
| 13 | مصطلحات الحجز |
| 14 | حالات الحجز |
| 15 | Itinerry |
| 16 | Retreive PNR |
| 17 | The Optinal Elments |
| 18 | The Optinal Elments |
| 18 | Frequent Flyer |
| 19 | Group Booking |
| 20 | Queues |
| 21 | Copy PNR |
| 21 | Print Out |
| 22 | ادخال بيانات جواز السفر للراكب |
| 23 | ادخال بيانات جواز السفر للراكب |
| 23 | حالة التذكرة بعد الاصدار |
| 24 | عناصر سجل الحجز |
| 25 | كيف تحجز وتسعر وتصدر تذكرة |
| 26 | كيف تحجز وتسعر وتصدر تذكرة |
| 27 | كيف تحجز وتسعر وتصدر تذكرة |
| 28 | الاسعار |
| 29 | الاسعار |
| 30 | الاسعار |
| 31 | الاسعار |
| 32 | الاسعار |
| 33 | اضافة ضريبة |
| 34 | طريقة الدفع |
| 34 | اضافة بيان Endoresment |
| 34 | العمولة |
| 35 | Tour code |
| 35 | Validity Carrier |
| 35 | Issue Ticket |
| 35 | Invoice |
| 36 | Copy Of Ticket |
| 36 | Ticketing Action identifiers |
| 37 | Ticketing Action identifiers |
| 38 | فئات درجات الحجز |
| 39 | الوجبات |
| 40 | الوجبات |
| 41 | الكود شير |
| 42 | الكود شير |
| 43 | Star Alliance |
| 44 | عدد السجمنت التى تمت |
| 45 | شرح مكونات التذكرة |
| 46 | شرح مكونات التذكرة |
| 47 | التسعير بــ FXD |
| 48 | التسعير بــ FXD |
| 49 | التسعير بــ FXD |
| 50 | طباعة EMD |
| 51 | التقرير البيعى TJQ |
| 52 | التقرير البيعى TJQ |
| 53 | عدم مطابقة الحجز مع عدد الركاب |
| 53 | لاضافة وزن زيادة |
| 54 | بحث عن غرامة التذكرة |
| 54 | اضافة رضيع على حجز موجود |
| 55 | استخراج غرامة التذكرة |
| 56 | الاميال وحساباتها |
| 56 | كشف عن درجات الحرارة |
| 57 | معرفة شركات الطيران الوكيلة |
| 57 | Refund |
| 58 | Refund |
| 59 | Reissue |
| 60 | Reissue |
| 61 | Reissue |
| 62 | Reissue |
| 63 | Reissue |
| 64 | Reissue |
| 65 | Reissue |
| 66 | Reissue |
| 67 | Reissue |
| 68 | Reissue |
| 70 | Penalty Codes |
| 71 | Reissue Automated |
| 72 | Reissue Automated |
| 73 | Retieve History |
| 74 | Remarks Field |
| 74 | تعديل من داخل الحجز |
| 74 | بعض اسباب اشعار الخصم |
| 75 | متنوعات |
| 76 | اكواد BSP |
| 77 | حالة التذكرة مترجم |
| 78 | اختصارات |
| 79 | اختصارات |
| 80 | اختصارات |
| 81 | اختصارات |
| 82 | اختصارات |
| 83 | اختصارات |
| 84 | اختصارات |
| 85 | اختصارات |

---

## Final instruction

Deliver an independent, evidence-led assessment that helps the founder and Fable make better decisions. Protect what is strong, expose what is weak or missing, identify software-design failure paths that ordinary feature reviews overlook, and recommend only changes that improve DEIXEN's ability to teach and evidence real professional task performance with a clear beginner experience. **Do not trade rigor for agreement, and do not trade product integrity for feature count.**
