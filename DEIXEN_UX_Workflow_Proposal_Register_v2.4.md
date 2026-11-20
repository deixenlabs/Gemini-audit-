# DEIXEN — Product UX & Workflow Proposal Register
## Provisional Product Proposals, Current Development Priorities & Deferred Implementation — v2.4

**Updated:** 18 November 2026  
**Latest provisional stage:** 155  
**Source baseline:** DEIXEN_UX_Workflow_Decision_Register_v2.3.md  
**Companion source references:** `DEIXEN_Objectives_and_Founder_Goals_Reference_v0.2.md`; `DEIXEN_Product_Feature_Ideas_Inventory_v0.2.md`  
**Revision purpose:** Incorporate Stages 153–155 as proposals provisionally accepted for inclusion in this working draft; reconcile the correction/start race, stale eligibility display, and eligibility restoration with Stages 144–152; and make the provisional review status explicit throughout the register. Retain the owner’s current sequence: Frontend and deterministic Program Engine first; Backend later, not cancelled; World/LLM as future expansion; human/trainer/institutional workflows outside the current software scope.

> **DOCUMENT STATUS — WORKING PROPOSAL DRAFT, NOT FINAL PRODUCT APPROVAL.** This file consolidates product UX/workflow proposals for review. Every stage from the early consolidated stages through Stage 155 is a proposal, not a final product decision, approved technical specification, implementation authorization, or claim that a feature exists in the repository. When the owner says “موافق” on a stage, that means the proposal's current wording may be carried forward in this draft for further analysis; it does **not** mean the concept has passed independent review or received final product/build approval. All stages remain open to challenge, revision, rejection, or deferral during the review sequence.
>
> **REVIEW ROUTE AND MODEL ROLES — as assigned by the owner:** The current working collaboration is the owner with ChatGPT and Claude Sonnet 5.5. After this proposal round closes, Sonnet 5.5 performs a second, independent review of this register together with the two companion reference files. Claude Fable 5.2 is the final reviewer and project lead: it receives the reviewed package, sets the final direction, and leads the project by directing the planned implementation models Claude Opus 5.5, Sonnet 5.5, and Haiku 5.5. These are the owner's planned roles and sequence, not claims that those reviews or implementation work have already occurred.
>
> **CURRENT DEVELOPMENT SEQUENCE — owner instruction:** The immediate work priority is the **Frontend and deterministic Program Engine**, built and tested as a local/single-user prototype. **Backend is not cancelled**: production persistence, accounts, security, access control, multi-user use, cross-device concurrency, and other server guarantees remain necessary for a real production launch, but implementation is postponed until the Frontend and Engine are sufficiently validated and the owner moves the project into that phase. Capabilities that need Backend remain proposed product requirements; only their Backend implementation is deferred. DEIXEN World and LLM are separate future expansions and are not prerequisites for the core product or its initial Backend. Human review, trainer administration, institutional governance, HR, investigations, and similar workflows are outside the current software-design scope and must not be silently reintroduced as Backend features.
>
> **SOURCE BASIS:** This proposal register was developed from the two companion working references listed above. Those files are themselves discussion-derived references, not final approved specifications. This register elaborates selected workflow proposals; it does not prove they are correct, complete, implemented, or fully consistent with every source idea. The three files must be reviewed together before final direction is set.
>
> No Amadeus command, response, or operational capability is accepted as supported without evidence from the actual training engine and appropriate authoritative references. This document does not claim repository verification or feature implementation.

---

# 0. Development priority and implementation boundaries

This section governs how every later proposal in this register must be interpreted. It prevents an accepted future requirement from being mistaken for work that should be built now.

## 0.1 Priority now — Frontend and deterministic Program Engine

The immediate objective is to build and test the product's actual user experience and its deterministic operating logic. Current work should focus on:

- The Frontend journeys and interactions for Home, Learning, Terminal, Scenario Bank, and Growth.
- The Program Engine: task states, conversation/task/operational separation, deterministic case rules, command execution through the verified training engine, validation, assistance rules, eligibility, attempts, results, evidence, corrections, and derived-state recalculation.
- The three Terminal modes and their different permissions/support rules.
- The first bounded professional workflow, including customer discovery, confirmation/authorization, operational work, validation, recovery, task closure, and learner-facing evidence.
- Structured, versioned data and explicit rule boundaries so the behavior is testable and can later be connected to Backend services.
- Local/single-user testing, including simulated failures and state transitions. Transitional local persistence may be used where necessary to test continuity, but it is not production-grade record storage.

The current implementation must be useful and testable as a product prototype, not merely a set of static screens. No LLM is used to fill gaps in rules or generate operational truth. Coach/customer behavior for this phase is deterministic and case-controlled.

## 0.2 Deferred implementation — Backend for production operation

Backend work is intentionally postponed until the Frontend and Program Engine have matured enough that their real data and service requirements are understood and the owner judges the product ready to approach the launch-preparation phase. Deferral does **not** cancel the requirements that Backend will need to support.

Before a real production launch to external learners, Backend will be needed for the capabilities that cannot be guaranteed by a local Frontend alone, including as applicable:

- Durable server-side storage of accounts, attempts, command/event histories, operational/task states, assessment results, evidence, rule versions, exposure records, and corrections.
- Authentication, authorization, role and ownership enforcement, and secure access to learner records.
- Reliable synchronization, recovery, backup/restore, and continuity across devices/sessions.
- Atomic attempt creation, server-enforced uniqueness, transaction safety, and idempotency across concurrent requests/devices.
- Server-side enforcement of access rules and protection against client-side tampering of protected assessment/evidence records.
- Appropriate audit/security logs, deployment, monitoring, and operational safeguards for a production service.

The precise Backend architecture, database, APIs, hosting, authentication provider, and migration plan are intentionally not being designed or implemented in this current phase. They should be based on the validated Frontend/Engine contracts rather than guessed in advance.

## 0.3 Design for later Backend without building it now

The current Frontend/Engine should avoid unnecessary coupling to local storage or screen components:

- Keep business rules and task/assessment state transitions in explicit engine functions, not scattered through UI components.
- Keep persistence behind a replaceable boundary/adapter; local storage is transitional and must not define the permanent architecture.
- Use stable identifiers and explicit versions for cases, variants, attempts, rules, and results.
- Preserve append-only event history and correction links in the data model.
- Define clear inputs, outputs, and failure states for operations that will later become Backend services.
- Do not claim cross-device, multi-user, tamper-resistant, or production-durable guarantees before Backend exists.

This is a lightweight readiness discipline, not a request to build a speculative abstraction framework or a premature distributed architecture.

## 0.4 Future expansions — DEIXEN World and LLM

The following remain separate future directions, not current dependencies:

- DEIXEN World / Virtual Company as an immersive presentation and interaction mode within Scenario Bank.
- LLM-assisted customer personality, natural dialogue, or voice interaction, while keeping case facts, operational truth, rules, and assessment integrity under deterministic control.
- Voice and speech recognition beyond an optional later enhancement with an equivalent text path.

Neither World nor LLM should delay the core Frontend/Engine. Their eventual use may require additional Backend services, but that is a later design question, not a reason to build those services now.

## 0.5 Outside the current product scope

Human review/approval, trainer administration, committees, institutional investigations, disciplinary actions, HR workflows, external-review arrangements, and institution-level governance are not current Frontend/Engine priorities and are not automatically included in future Backend scope. The software should preserve basic learner-facing transparency, evidence integrity, and privacy-by-design principles without building those human or institutional workflows.

## 0.6 Proposal status and implementation-priority labels

**Proposal status applies to every stage in this register, including stages whose wording the owner has provisionally accepted.** A stage-level “موافق” means only that the current proposal may remain in the draft and proceed to review. It is not final product approval, technical approval, implementation authorization, or a commitment that the feature will ship.

Use the separate implementation labels below only to describe sequencing. They do not change the provisional status of the product proposal itself.

| Label | Meaning |
|---|---|
| **PROVISIONAL — accepted for review** | The owner has agreed to keep the current proposal in the working draft. It remains open to independent challenge and final review. |
| **NOW — Frontend/Engine priority** | The owner's current development sequence places this capability or test in the immediate Frontend/Engine phase. This is not, by itself, final approval of the underlying feature. |
| **LATER — Backend** | The product requirement remains a working proposal for review; reliable production implementation depends on Backend and is postponed. |
| **FUTURE — World/LLM/Expansion** | A separate later product capability; not a dependency for the core product. |
| **OUT OF CURRENT SCOPE** | Not part of the current product workflow. It is not to be smuggled into the plan merely because Backend is eventually built. |
| **OPEN** | The product proposal or exact behavior is not yet settled; do not invent it during implementation. |

A proposal provisionally carried into this draft does not automatically approve every production implementation detail. Where a behavior can be developed and validated in the local Engine now but needs Backend enforcement later, both phases must be stated.

---

# 1. Executive direction

The immediate development goal is to prove, through the Frontend and deterministic Program Engine, that DEIXEN can take a beginner through a real, bounded travel-operations task and represent what the learner can perform, how independently they performed it, and where they need further development. This is first a build-and-test objective; it is not a claim that a local prototype is ready for public production use.

The current product is deterministic software: all current assessment, feedback, eligibility, and evidence logic must use explicit versioned rules and structured data. No LLM is part of the current release direction; LLM use remains deferred to future DEIXEN World.

The initial product must connect five things:

1. **Learning:** teach the operational and customer-service knowledge required for the selected work.
2. **Demonstration and assistance:** show how verified work is performed and help the learner understand it without doing the learner's work in protected assessment.
3. **Operational practice:** let the learner perform work through one central Terminal using the verified DEIXEN training engine.
4. **Scenario and assessment:** let the learner apply the knowledge to a case grounded in controlled customer and operational facts.
5. **Evidence and Growth:** preserve what happened, distinguish assisted from independent performance, and show the learner meaningful development information. After an assessment result is secured, provide a useful review while protecting reusable assessment content.

The current build strategy is **one complete, trustworthy professional workflow in the Frontend and Engine before a broad catalogue of partially finished features**. Backend integration follows when that workflow and its data/service contracts are sufficiently validated, and is required before a real production launch.

Do not turn DEIXEN's first release into a generic LMS, a full HR/institution-management platform, a case-investigation system, a large 3D game, or a multi-GDS product. Those expansions do not prove the core value proposition.

## 1.1 Proposed criteria before the core product can be considered production-launch ready

- A real, bounded operational workflow is supported and verified end to end.
- Customer understanding and professional judgment are part of the task, not an optional decoration around command practice.
- One Terminal supports the necessary modes without creating separate terminal products.
- The training engine's output and booking state are genuine to the supported training environment; DEIXEN never invents Amadeus behavior.
- The system can tell whether the learner completed the task correctly, whether the result met the customer's request, and whether the learner worked independently or with assistance.
- A learner can understand their result and see the evidence relevant to their development.
- Original evidence cannot be silently overwritten, and access to learner records is limited to an authorized purpose.
- The experience handles the common error, interruption, and recovery paths rather than only the ideal demonstration.
- Backend-backed persistence, authentication/authorization, secure data access, and multi-user reliability are implemented and tested before public production use.

The Frontend and Engine can be developed and tested before Backend integration. Passing local prototype tests is not equivalent to meeting production-launch requirements. These are product requirements to design, validate, and implement, not claims about current implementation status.

---

# 2. Product purpose and boundaries

## 2.1 Purpose

DEIXEN is a specialist professional training and work-competence system for travel operations. Its purpose is to reduce the gap between completing training and performing relevant work responsibly and independently.

Working category description:

**Professional Work Competence & Training System for Travel Operations.**

DEIXEN's value is the connection between customer understanding, professional judgment, operational execution, task correctness, recovery, and credible evidence of performance.

## 2.2 What DEIXEN is not

DEIXEN must not be reduced to:

- a generic Learning Management System;
- a command-memorization course;
- a GDS terminal simulator without customer and professional context;
- an unrestricted AI roleplay chatbot;
- an airline booking website;
- an open-world game;
- a full HR, employee administration, or institutional case-management system.

## 2.3 Competence priorities

- **Entry-level job-entry competence** and **additional skills that improve confidence and professional reliability** are both core priorities for the current product direction.
- Advanced specializations are future scope and must not delay the core.
- Amadeus is the initial operational center. Do not add other GDS platforms until the first operational foundation is validated.
- Saudi Arabia, the UAE, Oman, Egypt, and wider international markets remain relevant to DEIXEN's potential market. A current personal career focus must not narrow the product's long-term scope.
- Any Amadeus partnership, endorsement, or affiliation remains an aspiration unless formally evidenced and authorized.

## 2.4 The professional task is the organizing unit

The core design unit is a complete professional task, not an isolated lesson or command. A task may involve:

1. receiving the customer request;
2. clarifying missing or ambiguous information;
3. advising, deciding, and confirming the intended action;
4. performing supported operational work;
5. checking that the result matches the request and case constraints;
6. correcting, pausing, declining, or escalating where appropriate;
7. communicating the result and next steps;
8. closing or following up as the task requires.

Not every case uses every step. A responsible refusal or escalation may be the correct outcome; the system must not force a booking merely to produce a superficially successful result.

## 2.5 Correctness and customer experience are distinct

DEIXEN must not collapse these dimensions into one score:

- **Input / syntax correctness:** Was the information or command entered correctly?
- **Operational correctness:** Did the training engine reach the intended operational state?
- **Customer / task correctness:** Does that state satisfy the customer's confirmed request and constraints?
- **Professional correctness:** Were the decisions, advice, communication, and handling responsible and appropriate?
- **Customer experience:** How was the interaction experienced, based on observable behavior and case-grounded reactions?

Customer satisfaction cannot compensate for a wrong booking. An operationally accepted booking can still be professionally wrong or fail the customer's request. Accent, personality stereotypes, or vague impressions must not substitute for observable professional behavior.

## 2.6 Current software approach: deterministic rules, no LLM dependency

For the current Frontend/Engine phase, all product behavior must be implemented through explicit, testable software rules and structured data. This includes Coach behavior, assessment eligibility, case logic, deterministic customer-response rules, evidence handling, content visibility, variant exposure tracking, and assessment-validity states.

- Do not assume that an LLM or generative model is available in the current product.
- Do not use an LLM as a temporary substitute for missing business rules, operational truth, or assessment logic.
- When the program cannot determine a state from explicit rules and recorded events, preserve the uncertainty and use a defined safe state (such as a learner-specific hold) rather than guessing.
- LLM use is a possible future DEIXEN World capability only; it is not part of the current Frontend/Engine phase or a prerequisite for the core product.
- Human review, trainer administration, appointment, committee, investigation, HR, and institutional procedures are outside the current product workflow scope. They are not assumed to become Backend features.

---

# 3. Product structure

## 3.1 Five top-level areas

The current proposed product structure is:

1. **Home** — orientation and the next useful action.
2. **Learning** — Amadeus and Customer Service learning, understanding checks, and relevant practice.
3. **Terminal** — the operational workspace where the learner performs supported work.
4. **Scenario Bank** — the library of professional cases and their eligibility/access rules.
5. **Growth** — evidence of demonstrated skills, performance conditions, development history, and next priorities.

**Ghost** and **Coach** are capabilities used across the product, not additional top-level areas. **DEIXEN World / Virtual Company** is a possible future Scenario Bank mode, not a sixth area.

## 3.2 Responsibility boundaries

| Area / capability | Primary responsibility | Must not become |
|---|---|---|
| Home | Orient the learner and show a useful next step | A generic dashboard or duplicate Growth page |
| Learning | Teach concepts, inputs, outputs, and professional context | Proof of independent competence just because content was completed |
| Terminal | Execute work through the verified training engine | Separate terminals for each mode or an invented Amadeus output generator |
| Scenario Bank | Organize professional cases and initialize task runs | A detached execution runtime or second terminal |
| Growth | Explain evidence and development | Points, arbitrary badges, or one readiness percentage |
| Ghost | Demonstrate verified workflows and explain real output | Independent learner evidence or hidden assessment assistance |
| Coach | Teach, guide, question, and give permitted feedback | The customer, a silent executor, or an answer-giving assistant in protected assessment |
| Customer simulation | Deliver case-grounded information and reactions | An unrestricted chatbot that invents authoritative facts |
| Assessment and evidence | Evaluate observable work and preserve its provenance | Intuition-based scoring or retroactive rewriting of history |
| DEIXEN World | Future optional presentation layer around a professional task | A current build dependency, open world, or parallel task engine |

---

# 4. Core learner and task journeys

## 4.1 Learner journey

First entry and orientation → relevant baseline/diagnostic where useful → Amadeus and Customer Service Learning → understanding verification → Ghost demonstration where relevant → guided practice → independent practice → eligible scenario → independent assessment → evidence review in Growth → continued development.

This is an adaptive route, not a rigid funnel. A learner may return to a targeted lesson or practice activity, and previously demonstrated knowledge may reduce unnecessary repetition. A diagnostic or lesson completion does not prove independent competence.

## 4.2 Professional task journey

Customer request → clarify/discover → advise/decide/confirm → execute operational work → validate the real result against the request → recover/correct/pause/decline/escalate when needed → communicate → close/follow up.

### Initial task candidate proposal (Stage 90)

The first end-to-end professional task targeted for launch is a **simple new flight reservation** with the following bounded scope:

- one adult traveller / one passenger;
- one flight segment;
- one fare context;
- no assumed payment, ticket issuance, live availability search, or fare comparison unless the current engine and authoritative references are separately verified and those functions are deliberately added;
- changes to an already-created reservation are outside this first task and should be covered by a later case only after the engine behavior is verified.

This is the current working proposal for the first bounded task, provisionally carried into this draft for review. It is not a final launch-scope decision and does not prove that the current repository or training engine supports every part of the workflow. Exact scope and supported operations must be checked against the current implementation and authoritative operational references before the case is finalized.

### What counts as success for the first task (Stage 91)

The task can be considered successfully completed only when the learner has created the reservation through Terminal, the training engine has saved it and it can be retrieved/verified, the passenger and flight details match the latest customer-confirmed request, no unresolved error or unknown result prevents validation, and the learner communicates the outcome professionally. A valid reservation must not be described as a ticketed journey: **reservation creation and ticket issuance are separate outcomes**. Success demonstrates only the defined task scope, not mastery of all Amadeus functions.

## 4.3 Learning and assistance journey

Identify the learner's need → direct them to the relevant concept or demonstration → guided attempt → observe the difficulty → provide only the support permitted by the active mode → reduce assistance as the learner develops → verify understanding and independent performance.

A syntax misconception, a weak customer-discovery decision, and an accepted booking that does not meet the customer's request are different problems and must not receive the same generic hint.

## 4.4 Scenario and assessment journey

Browse case category → select case → understand task objective and prerequisites → initialize one task run → receive permitted case/customer context → work in Terminal Scenario Mode → validate the result → submit for review → receive a mode-appropriate debrief → retain valid evidence and identify the next useful step.

A case, customer facts, operational session, assistance policy, task run, and evidence record must remain connected and consistent.

---

# 5. Proposed core-product behavior for review and validation

This section collects proposed capabilities for a possible first core release. It is a working design hypothesis to be challenged against the two source references, repository reality, and independent review; it is not a final release specification or implementation authorization. It does not prescribe the final screen design or backend architecture.

## 5.0 Implementation priority across the product

The proposals below are not all intended for implementation in the same phase. Use this map while reading Sections 5.1–5.23. The priority map follows the owner's current development-sequencing instruction; it does not make the underlying product proposals final.

| Product function | NOW — Frontend/Engine | LATER — Backend or future phase |
|---|---|---|
| Home and navigation | Build the current learner orientation and next-step experience | Server-backed profiles and synchronized progress |
| Learning | Build learning paths, content, understanding checks, and deterministic routing | Durable learner progress synchronization |
| Ghost and Coach | Verified demonstrations and rule-based assistance in permitted modes | LLM-driven interaction/personality is future World scope |
| Terminal | One workspace, three modes, command lifecycle, validation, recovery, and evidence events | Server persistence and multi-user protection |
| Scenario Bank | Small versioned case set, deterministic eligibility, variants, preview and start flow | Server-side case/attempt storage and concurrent attempt guarantees |
| Customer interaction | Authored text and deterministic case-grounded responses | Voice/LLM interaction is future scope |
| Assessment | Criteria, eligibility, assistance restrictions, exposure logic, result validity, issue checks, and corrected results | Server-side protection, durable records, and authoritative multi-user enforcement |
| Growth and recommendations | Learner-facing evidence view, deterministic skill calculations, recommendations, and correction propagation | Durable server-backed portfolio and controlled sharing |
| Privacy and recovery | Private-by-design UI, local test behavior, clear states | Authentication, authorization, secure storage, backup, cross-device recovery |
| Trainer/institutional workflows | Not in current scope | Not automatically included in Backend; requires a separate owner decision |
| DEIXEN World / LLM / multiple GDS | Not in current scope | Separate future expansion, not a prerequisite for core Backend |

For many functions, the **product rule is current while production infrastructure is deferred**. For example, the Engine should already know that a duplicate start request must not create a second Attempt; Backend later enforces the same guarantee across concurrent clients and devices.

---

## 5.1 Learning: teach understanding, not memorization

**NOW — Frontend/Engine:** build the learner-facing tracks, content flow, understanding checks, and deterministic next-step routing for the selected task. **LATER — Backend:** synchronize and durably retain learner progress. The learning design should not wait for Backend.

The two primary tracks are:

- **Amadeus Track:** operational concepts, inputs, commands, outputs, warnings, resulting states, and recovery.
- **Customer Service Track:** discovery, clarification, communication, advice, expectation management, handling changes, and professional closure.

Working learning hierarchy:

**Track → Module → Lesson → Learning Objectives → Understanding Verification → Related Practice.**

Content completion and understanding verification are separate. Watching a demonstration or clicking “I understand” is not sufficient evidence of comprehension. Teach what to enter and how to interpret what the system returns, with depth appropriate to the skill.

A baseline diagnostic may help route the learner to relevant material, but it must not certify independent competence.

## 5.2 Ghost and Coach: distinct roles, mode-aware support

**Ghost** demonstrates using the same verified training engine and explains why an action is taken, what output means, and what changed. It is demonstration, not proof that the learner can perform independently.

**Coach** orients, asks questions, checks understanding, provides proportionate guidance in permitted modes, and recommends useful learning/practice. It must not execute the learner's work or reveal answers during protected independent assessment.

Assistance must be traceable. Distinguish help that reached the learner from a request denied before helpful content was disclosed. A later correct result does not convert an assisted step into independent performance.

**NOW — Frontend/Engine:** implement only the deterministic assistance types needed for the validated Learning/Practice/Assessment flow. **FUTURE:** a highly elaborate Coach persona, autonomous AI coaching, or LLM-driven interaction is not a current requirement.

## 5.3 Terminal: one operational workspace

**NOW — Frontend/Engine:** build the shared workspace, mode-specific behavior, command lifecycle, and clear operational/task/customer/assistance states. **LATER — Backend:** persist authoritative attempts, operations, and evidence and enforce multi-user protection.

Terminal remains one workspace with three operating modes:

1. **Practice Mode** — supported learning, trying commands, inspecting outputs, making and correcting errors.
2. **Scenario Mode** — executing a professional case selected from Scenario Bank.
3. **Independent Assessment Mode** — a protected attempt with prohibited answer-revealing assistance blocked and evidence conditions enforced.

The modes share the operational workspace but have different support rules, context, permissions, and evidence conditions. Do not build a separate terminal application for each mode.

Terminal's functional responsibilities are:

- clear mode and attempt state;
- command entry and genuine system output;
- relevant task context;
- customer interaction where the case requires it;
- permitted assistance;
- useful task status and recovery.

These are connected responsibilities, not six mandatory screen panels. The interface must also keep four message types distinguishable: genuine operational output; task/customer information; DEIXEN validation or assessment feedback; and Learning/Coach/Ghost explanations. They must not be presented as though they came from the same source. In protected assessment, learning explanations and answer-revealing validation feedback remain restricted.

## 5.4 Preserve the sources of truth

**NOW — Frontend/Engine:** implement these as explicit, separately testable state/data boundaries. **LATER — Backend:** persist and protect their authoritative records across users and sessions.

The following must remain distinct:

- **Case definition:** task facts, constraints, known/discoverable information, allowed outcomes, and criteria.
- **Customer/conversation state:** what was said, disclosed, clarified, or changed.
- **Task state:** what is now required and where the task has reached.
- **Operational state:** the actual booking/PNR state held by the verified training engine.
- **Coach/Ghost:** instructional content and demonstrations.
- **Assessment rules:** eligibility, assistance restrictions, criteria, and outcome logic.
- **Evidence record:** observable events, source, attempt conditions, assistance exposure, and results.

A customer changing a request does not itself change the booking. Only the learner's supported action through the operational engine can change operational state. DEIXEN checks whether the resulting operational state meets the latest confirmed request.

System output must not be invented. DEIXEN teaching explanations must be visibly separate from genuine operational output. Do not describe a training environment as a live Amadeus connection unless that is actually verified.

## 5.5 Command and task lifecycle

**NOW — Frontend/Engine:** implement the input/execution/response/impact lifecycle and deterministic recovery behavior. **LATER — Backend:** provide durable event and operational-state persistence and cross-device recovery. The local prototype must not claim those production guarantees.

The operational cycle is:

**Learner command input → execution → genuine system response → task/operational impact.**

- No operational work is performed on the learner's behalf in independent assessment.
- Submitted commands and their responses must be linked.
- Typed-but-not-submitted input must be distinguishable from an executed command.
- Corrections are added as new events; prior actions are not silently rewritten.
- An unknown result remains unknown until the engine verifies it.

Keep three records conceptually separate even if they appear in one interface: **Command & Response History** (what the learner submitted and what the engine returned), **Current Operational State** (the latest verified booking/PNR state), and **Task Progress** (what is known, complete, remaining, or awaiting action). A history of successful commands is not itself proof that the current booking is correct.

The learner initiates task submission/closure. DEIXEN validates the applicable:

1. operational result;
2. match to the latest customer request and case requirements;
3. professional communication/closure or justified escalation.

Command success, command count, or the existence of a PNR alone does not establish task completion.

Review and correction behavior must differ by mode: Practice should allow the learner to inspect and correct the same active attempt while preserving its history; Scenario correction must follow the case rules and retain the sequence of actions; a submitted Independent Assessment is protected and must not receive answer-revealing repair help. If a technical problem makes an assessment result unverifiable, do not award independent evidence, but do not automatically blame the learner.

## 5.6 Case packages and Scenario Bank

**NOW — Frontend/Engine:** define and test a small structured, versioned case set, its preview, eligibility, and handoff to the shared Terminal. **LATER — Backend:** persist and distribute case/attempt records for production use.

Scenario Bank is the case library; Terminal is where the work runs. Cases should be organized primarily by professional work situation/domain, with skills as a secondary discovery filter. Before a run, the learner receives a useful brief about the general situation, responsibility, objective, and prerequisites; it must not reveal protected facts, exact commands, or the solution sequence. Access should depend on relevant skill prerequisites and evidence, not course completion alone.

Keep the following task objects distinct because they serve different product purposes:

- **Case Package:** the authored, versioned professional situation and its rules.
- **Scenario Variant:** a controlled change to the situation that tests meaningful transfer.
- **Task Run:** one initialized case/variant under a particular mode and support policy.
- **Attempt:** the learner's performance history and evidence for that opportunity.
- **Operational Session:** the actual booking/PNR state held by the training engine.

A professional case should define only what is needed to control the task reliably:

- customer request and task objective;
- information known at the start and information the learner must discover;
- relevant constraints and permitted outcomes;
- expected operational state and supported actions;
- customer response rules where interaction is included;
- assistance rules by mode;
- observable task/professional criteria and recovery routes;
- version and any controlled variant used.

The case must be versioned. A later change must not rewrite the facts or criteria of a past attempt.

For the candidate first core release, start with a small number of structured cases that pass explicit software-completeness checks and source-backed operational verification. Do not create a large scenario catalogue before the first cases are operationally and professionally validated.

## 5.7 Customer simulation: controlled, text-first

Customer behavior must follow the case definition. The customer may disclose facts, answer questions, clarify needs, or change the request only according to the case's allowed rules.

**NOW — Frontend/Engine:** customer dialogue uses authored text and predefined deterministic response rules. No LLM generates dialogue or alters case facts. **FUTURE — World/LLM:** more natural personality, voice, and generative expression may be considered later, while case facts, operational truth, and assessment rules remain controlled by the deterministic Engine.

A text-based customer interaction is sufficient for the first launch. Voice may be added later, but it must remain optional and have an equivalent text path. Accent or speech-recognition errors must not be treated automatically as learner mistakes.

Customer satisfaction/reaction is one evidence input, not the sole evaluator. If the scenario offers no fair opportunity to demonstrate a behavior, mark it Not Applicable rather than Not Demonstrated.

## 5.8 Assessment: distinguish result, independence, and validity

**NOW — Frontend/Engine:** build deterministic eligibility, assistance, evaluation, exposure, validity, and feedback rules. **LATER — Backend:** secure and durably store finalized results and evidence and enforce their integrity across users/devices.

Performance and independence are separate dimensions. The evidence model must be able to distinguish:

- how the learner performed (independent, hint-assisted, Coach-assisted, system-assisted, or contaminated); and
- what happened (correct, self-corrected, assisted correction, incorrect, incomplete, or invalidated).

These are working labels; final status definitions and criteria must be specified and validated before implementation.

Evidence should be traceable at three levels:

- **Step evidence:** an action, decision, interpretation, or skill under known conditions.
- **Task evidence:** the professional task result against the case criteria.
- **Transfer evidence:** performance in a meaningfully changed situation, not merely a superficial value substitution.

The working assessment outcomes are:

- Valid — Independent Evidence;
- Valid — Criteria Not Met;
- Incomplete;
- Invalidated.

A valid assessment where the learner did not meet criteria is not the same as an invalid assessment. An assisted or unverified attempt must not be reported as independent success. Do not invent arbitrary readiness percentages, universal attempt counts, or pressure/timing thresholds.

## 5.9 Post-task outputs and Growth

**NOW — Frontend/Engine:** build the learner-facing Task Outcome, Performance Review, Learning Debrief, and Growth evidence views, plus deterministic skill/recommendation calculations. **LATER — Backend:** store and protect the long-term evidence portfolio and support account-based access. Do not build broad sharing or trainer-facing views now.

Keep four outputs conceptually distinct:

1. **Task Outcome:** what happened to this task.
2. **Performance Review:** how the learner performed and under what support conditions.
3. **Learning Debrief:** what the learner should understand or practice next.
4. **Growth Evidence:** what is retained as evidence of demonstrated capability.

Growth is an evidence portfolio, not a points dashboard. It should help the learner understand:

- what skill/task was demonstrated;
- under what conditions and with what assistance;
- what errors and recoveries occurred;
- what was and was not assessed;
- whether meaningful transfer was demonstrated;
- what useful development step comes next.

Competency interpretation must consider the evidence set, independence, task scope, and conditions. Do not use the average or last attempt alone, do not erase conflicting evidence, and do not generalize beyond what was assessed. No single numeric readiness percentage and no employment guarantee.

Keep a distinction between the learner-facing evidence view and the more detailed structured evidence record. The learner should not have to interpret raw telemetry. The internal record must preserve enough commands, outputs, events, assistance, versions, and assessment conditions to reproduce the product's decision. **NOW — Frontend/Engine:** build and test the learner-facing evidence and the underlying structured record in the local prototype. **LATER — Backend:** provide durable, protected, multi-user storage before production use. Historical evidence should persist; its current relevance may be reconsidered when a skill or authoritative procedure changes, but do not impose arbitrary expiry dates.

## 5.10 Human/trainer review is outside the current product workflow

Human review, trainer administration, trainer notes, trainer recommendations, learner/trainer disputes, reviewer assignment, and institutional appeal workflows are **OUT OF CURRENT SCOPE** for the Frontend/Engine work defined here. They must not be treated as current launch requirements or quietly introduced as Backend features.

The following software principles remain relevant now because they protect the integrity of the learner's own record:

- system-generated development recommendations must be based on evidence and explicit rules;
- a recommendation is not itself proof of competence;
- original performance evidence and result history must not be silently overwritten;
- any deterministic correction to a result or recommendation must remain traceable;
- the learner must be able to understand material changes to their own Growth information.

The system's deterministic recommendations in Stages 105–106 and 145–146 are distinct from recommendations written by a human trainer. The former remain part of the current product direction; the latter are not part of this scope.

## 5.11 Privacy, access, and sharing

Privacy is a product constraint from the beginning, but actual production-grade identity and access enforcement depends on Backend.

**NOW — Frontend/Engine:**
- Design learner evidence as private by default; do not add broad sharing or public exposure.
- Keep learner-facing information scoped to the learner's own record in the single-user prototype.
- Avoid displaying unrelated learner information or exposing internal records through ordinary product screens.
- Keep data structures and UI boundaries compatible with future role/ownership checks without building trainer or institutional workflows.

**LATER — Backend before production launch:**
- Provide authentication and server-side authorization.
- Enforce ownership and least-privilege access to learner records.
- Protect sensitive evidence from client-side alteration or unauthorized access.
- Add appropriate security/access logging, secure storage, retention/backup, and recovery controls.
- Only later consider voluntary evidence sharing or aggregate analytics after their purposes, permissions, and privacy controls are explicitly defined.

Do not build trainer portals, employer portals, staff dashboards, broad sharing, or marketing analytics in the current phase. If production access and privacy guarantees are not implemented in Backend, DEIXEN must not present the product as a secure multi-user production service.

## 5.12 Recovery, continuity, and usability

**NOW — Frontend/Engine:** implement and test explicit pause, resume, reload, and interruption states for the current single-user workflow. Preserve task context, customer/conversation state, operational state, assistance events, command history, and attempt identity within the available local test environment. Before retrying an uncertain operation, check the known engine state; never blindly resend.

Practice and Scenario may resume the same attempt when the local Engine can establish its identity and state. Independent Assessment may resume only when the attempt identity, event history, operational state, and assistance conditions remain verifiable. Otherwise, do not award unverified independent evidence, and do not automatically classify a technical interruption as learner failure.

Provide clear loading, empty, denied-assistance, incomplete-task, error, and recovery states. Test readable controls, keyboard use, Arabic/RTL behavior, captions/text alternatives where relevant, and reduced motion within the actual Frontend.

**LATER — Backend:** reliable cross-device recovery, durable server-side event storage, synchronization, backup/restore, and recovery after server/network failure require Backend. Local persistence is transitional and must not be represented as production durability.

## 5.13 First-case validation and customer interaction (Stages 92–94)

**Priority for Sections 5.13–5.23:** the task, customer, eligibility, assessment, exposure, correction, Growth, and attempt-start rules below are **NOW — Frontend/Engine** product behavior. Implement and test them deterministically in the current local prototype. **LATER — Backend** supplies durable production storage, account/security enforcement, and cross-device guarantees; deferring those services does not cancel the product rules. **FUTURE — World/LLM** capabilities are not required for these workflows, and human/trainer/institutional procedures remain outside the current scope.

The proposed first reservation case must teach and assess more than command entry. The learner must obtain the required customer information, distinguish confirmed facts from missing or uncertain details, clarify what is needed, and confirm the essential details before operational execution. Information collection is part of professional competence, not decorative dialogue before the Terminal.

The case must not hide information arbitrarily. Some cases may provide details directly; others may require the learner to discover them through appropriate questions. What is supplied and what must be discovered must be explicitly defined in the Case Package according to the learning objective.

For the candidate first release, customer interaction may be **text-first**. The simulated customer must be natural in expression but controlled in facts:

- answers must be grounded in the information defined by the case;
- details should not be volunteered automatically when discovery is the skill being tested;
- unclear questions may receive a request for clarification;
- unsupported assumptions by the learner must not be confirmed merely to keep the dialogue moving;
- the customer simulation must not invent missing facts or authoritative operational information.

Customer personality and wording may vary, but the case facts, constraints, and expected operational outcome must remain stable for fair practice and assessment. A text-first implementation is sufficient for launch; voice is optional future scope and must not become a fairness barrier.

### Error, warning, and unknown-result handling (Stage 92)

The first task must distinguish:

1. **Blocking errors:** issues that prevent a valid task outcome, such as incorrect passenger/flight details, failure to save or retrieve the reservation, or a critical mismatch with the confirmed request.
2. **Warnings requiring attention:** messages that may allow processing to continue but require the learner to interpret their meaning and take the appropriate supported action. A visible reservation does not justify ignoring a warning.
3. **Unknown or unsupported behavior:** outputs or effects that have not been verified. The system must preserve uncertainty, avoid invented explanations, and must not declare success by guessing.

A PNR appearing is not sufficient evidence of task success. Validation must consider the actual saved state, consistency with the latest confirmed request, and unresolved errors/warnings/unknown outcomes. The exact classification of real Amadeus messages must be sourced from verified engine behavior and authoritative references, not hard-coded from assumptions.

---


## 5.14 Customer confirmation, authorization, and request changes (Stages 95–99)

The first reservation workflow must distinguish the customer's confirmation of the request from authorization to proceed with creating the reservation.

- **Confirm the request:** Before operational execution, the learner summarizes the essential passenger and flight details and resolves any material mismatch. Do not repeat questions that have already been answered or add ceremonial dialogue.
- **Obtain authorization to create:** The customer must clearly authorize the learner to create the reservation. Providing details or confirming that they are accurate is not, by itself, authorization to execute the booking action.
- **Keep authorization bounded:** Authorization to create a reservation is not authorization to make a payment or issue a ticket. Those are separate actions and are outside the assumed first-task scope.

### If the customer changes the request

The workflow depends on when the change occurs:

1. **After confirmation/authorization but before execution:** stop work based on the old request, record the change in conversation/task context, clarify affected details, reconfirm the revised request, and obtain renewed authorization when the change is material. Customer dialogue must not update operational booking state.
2. **During execution:** pause steps that rely on the old request; preserve all submitted actions and responses; verify the actual engine state before deciding what can safely happen next. Do not assume an action failed or blindly repeat commands. Use only a verified recovery path, then reconfirm the revised request and authorization before continuing as appropriate.
3. **After reservation creation:** preserve the original reservation creation as a valid historical event and record the customer's new request as a separate change request. Do not describe the reservation as matching the new request until a supported modification has actually been performed and verified. Modification of an existing reservation is outside the first launch task and must wait for a later, separately validated workflow.

This prevents an earlier confirmation from being treated as permission to execute a request that is no longer current. Conversation changes, task requirements, and operational booking state remain separate sources of truth. The learner remains responsible for the operational action; customer simulation, any future AI/LLM layer, and Coach must not modify the booking behind the learner's back.


## 5.15 Professional outcomes, skill evidence, and next learning opportunity (Stages 100–106)

### A task may end correctly without a reservation (Stages 100–101)

The first case and every future Case Package must define its valid professional outcomes. Do not assume that every customer interaction must end with a created PNR.

For example, the learner may correctly:

- create a reservation that matches the confirmed and authorized request;
- stop when the customer withdraws before execution, record the decision, and close the interaction professionally without pressure;
- decline, pause, or escalate when the request cannot responsibly be completed within the supported scope, where the case definition allows that outcome.

Creating a reservation that is unauthorized or materially mismatched is not made professionally correct merely because the operational engine accepted it. If any commands were already executed before authorization was withdrawn, the learner must verify the actual operational state and follow only a supported recovery path.

### Keep task outcome separate from learner performance (Stage 102)

DEIXEN must distinguish two connected records:

- **Task Outcome:** what happened operationally (for example, reservation created, no reservation because the customer withdrew, escalated, incomplete, or an incorrect/unauthorized operation occurred).
- **Performance Outcome:** how appropriately the learner understood the request, obtained confirmation and authorization, made decisions, used the operational system, handled the customer, and closed or escalated the task.

A task can end without a reservation while the learner's performance is professionally correct. Conversely, the engine may create a PNR while the learner's performance is incorrect. The Case Package defines which task outcomes are valid and which performance criteria apply to each path.

### Record skills only when the case provides a fair opportunity (Stages 103–104)

For each skill relevant to the task, distinguish:

- **Demonstrated:** the learner had an opportunity and showed the required behavior.
- **Not Demonstrated:** a fair opportunity to show the skill was present, but the required performance was not shown.
- **Not Assessed:** the task path did not provide a suitable opportunity to assess that skill.

Not Assessed is not a failure and must not be converted into a negative competence conclusion. For example, if the customer withdraws before operational work begins, the learner may have demonstrated customer discovery and authorization handling while reservation execution and PNR validation remain Not Assessed.

Do not force every case to exercise every skill, and do not require the learner to repeat a whole scenario just because one skill was Not Assessed. Preserve the evidence already earned and offer a suitable later activity that gives a fair opportunity to demonstrate the missing skill. Any later evidence is additive and linked to the relevant skill; it does not rewrite the earlier attempt.

### Select the next opportunity based on evidence, not assumptions (Stages 105–106)

DEIXEN should identify which relevant skills still need an appropriate opportunity and select the smallest suitable next step:

- **Understanding is missing or uncertain:** return to a targeted Learning explanation or Ghost demonstration, as appropriate.
- **Understanding exists but application has not been shown:** offer Guided Practice or Independent Practice.
- **Transfer to a changed situation has not been shown:** offer a relevant Scenario.
- **Prerequisites and evidence requirements are satisfied:** make the learner eligible for Independent Assessment.

The system must not assume that Not Assessed means the learner needs to relearn the skill, must not repeat already demonstrated content without reason, and must not treat a suggested next activity as evidence that the learner is weak. Explain the reason for the next-step suggestion in learner-understandable language without revealing protected assessment answers or criteria.

These rules define the product direction. The precise recommendation logic, thresholds, and activity-matching rules remain to be validated against the first launch case; do not build a complex adaptive engine prematurely.

## 5.16 Independent-assessment eligibility, reassessment, and controlled variants (Stages 107–111)

### Eligibility is based on necessary preparation, not lesson or attempt counts (Stage 107)

A learner becomes eligible for an independent assessment when the necessary preparation for the target skill has been demonstrated. For the first task, this normally means:

- relevant understanding checks have been passed;
- an appropriate Ghost or other verified demonstration has been provided and understood;
- the learner has had a suitable practical opportunity to apply the skill.

These are preparation requirements, not a requirement to master the task before assessment. Reliable prior evidence may satisfy a requirement and prevent unnecessary repetition. Eligibility must be tied to the assessed skill and task scope, not to a fixed number of lessons or attempts.

### Practice errors do not automatically block assessment (Stage 108)

Previous practice errors and the number of practice attempts do not, by themselves, determine eligibility. The learner need not achieve flawless performance during practice before entering an independent assessment. However, an essential misunderstanding that could lead to an invalid or materially incorrect operation must be addressed before the assessment begins. This balances a fair opportunity to demonstrate independence with the need for minimum operational understanding.

### An unsuccessful assessment leads to development and a new attempt (Stage 109)

When the learner does not meet the assessment criteria:

- preserve the submitted attempt and its result as an immutable record;
- secure the result before showing protected feedback;
- provide a review of what was and was not demonstrated, at a level appropriate to the assessment rules;
- identify the relevant skill-development need and offer a suitable Learning, Practice, or Scenario activity;
- allow a new independent assessment when the learner again meets the applicable prerequisites.

Do not repair the sealed attempt, reveal protected answers before the result is fixed, impose a fixed attempt limit merely because the learner did not pass, or reuse an unchanged case in a way that rewards answer memorization.

### Use controlled variants to test transfer, not recall (Stage 110)

Where a later independent assessment is needed, use a controlled variant of the professional task when appropriate. The variant may change selected case details while preserving:

- the target competency and observable criteria;
- the same professional task purpose and permitted outcome logic;
- a comparable level of difficulty and operational demand;
- verified operational behavior and supported actions.

The changes must be authored or bounded by explicit case rules. For the current release, customer dialogue and its variations must use authored text and predefined deterministic response rules. No LLM is used to generate customer dialogue or assessment facts in the current product. Controlled variants are intended to test transfer to a meaningfully changed situation, not to create arbitrary novelty. Future LLM use in DEIXEN World remains separate and deferred.

### Require complete variant data before activation (Stage 111)

No new or changed variant should enter Independent Assessment merely because its data has been changed. Before the software allows activation, the variant must contain:

1. defined operational facts, supported actions, and expected outcome;
2. the target skills and their observable assessment criteria;
3. controlled changes from the reference case and comparable difficulty attributes;
4. complete customer-information and disclosure rules;
5. the sensitivity classifications and skill mappings needed for assessment-exposure protection;
6. a configured validation/activation state indicating that the required content checks are complete.

The program checks that these required fields and relationships exist and blocks activation when they are missing or contradictory. It does not generate assessment variants or judge their professional correctness through an LLM. For the initial release, use a small, bounded set of versioned variants rather than a general-purpose variant-generation or automated difficulty-equivalence platform.

**Still open:** the exact software validation fields for each assessed skill; the required comparable-difficulty attributes; how much case variation is enough to test transfer without changing the skill; and the minimum number of ready variants needed for fair reassessment. External content-approval and human sign-off arrangements are outside this current product-workflow scope.


## 5.17 Independent-assessment entry, integrity, and permitted resources (Stages 112–119)

### Assessment can begin at the first eligible opportunity (Stage 112)

A learner may enter Independent Assessment as soon as the task-related eligibility requirements are met, including at the first opportunity. Do not require a fixed number of practice attempts or repeated training merely to satisfy an arbitrary count. Eligibility depends on demonstrated preparation and the absence of unresolved essential misunderstandings, not on a practice counter.

### The learner chooses when to begin (Stage 113)

DEIXEN determines and explains whether the learner is eligible, without revealing protected assessment criteria or answers. The learner decides whether and when to start. The system must not launch an assessment automatically just because eligibility has been reached. If the learner is not eligible, explain the preparation still needed in learner-understandable terms.

### Eligibility can be retained when the learner delays (Stage 114)

If an eligible learner postpones the assessment, preserve their progress, supporting evidence, and eligibility basis. Do not force an immediate attempt or require lessons/practice to be repeated without a reason. If a material change occurs in an authoritative procedure, supported engine behavior, or task prerequisite, recheck only the affected requirement and explain what has changed. A delay is not negative evidence of competence.

### Provide a concise pre-assessment briefing (Stage 115)

Before the attempt, show a short briefing that explains:

- the general nature of the task and the learner's responsibility;
- that the attempt is independent and which forms of assistance or reference use are permitted or prohibited;
- that relevant actions, commands, responses, errors, corrections, and assistance exposure are recorded as part of the evidence;
- what happens after submission and when feedback becomes available;
- that the learner may leave the briefing without starting or consuming an assessment attempt.

Do not disclose hidden customer facts, expected answers, protected criteria, or the solution sequence. The briefing should inform the learner of the rules, not coach them through the task.

### The explicit start action creates the assessment attempt (Stage 116)

The learner deliberately selects **Start Assessment** and confirms. This begins the attempt-creation process, but the attempt is not considered successfully started until DEIXEN has created and stored its distinct Attempt record and bound the applicable case/variant, eligibility snapshot, assessment rules, and assistance policy. No operational command may execute before that record is successfully established. Stages 150–152 define the preview/start boundary, safe Attempt creation, and duplicate-request protection. Stages 153–155 extend these rules to eligibility corrections and scenario availability before start.

At successful creation, DEIXEN must:

- create one distinct Attempt record;
- bind the exact Case Package, Variant, and version used;
- bind the eligibility decision/snapshot and the assessment rules and assistance policy applicable to that attempt;
- begin recording the relevant performance events and operational interactions.

Leaving or disconnecting after the start does not erase the attempt. Resume the same attempt only when its identity, event history, operational state, and assessment integrity can be verified. Otherwise classify the attempt according to the evidenced technical/integrity condition; a technical interruption is not automatically professional failure.

### Distinguish requesting assistance from receiving it (Stage 117)

A request for Coach/Ghost help during Independent Assessment is recorded, even when the request is denied. A denied request alone does not remove the attempt's independent status. The interface should clearly state that the requested help is unavailable without revealing the answer. If prohibited help is accidentally delivered, preserve exactly what reached the learner and review its actual impact on independence and attempt validity; do not silently ignore the exposure or automatically assume a particular outcome without examining it.

### Distinguish workplace information, ordinary interface tools, and instructional help (Stage 118)

The assessment must permit the genuine information and basic interface functions required by the defined task, while blocking instructional help that performs the learner's thinking or work.

- **Operational/workplace information:** genuine training-engine outputs, operational errors and warnings, customer facts supplied by the case, verified booking state, and the learner's own command/response history. These are part of the work environment, not Coach assistance.
- **Ordinary interface functions:** navigation, viewing available task information, and reviewing the learner's own command history, provided these functions do not reveal a solution or execute work on the learner's behalf.
- **Prohibited instructional assistance:** hints that reveal which command or step to use, answer-revealing interpretations/corrections, Ghost demonstrations of the solution, Coach prompts that disclose the next action, or system execution on behalf of the learner.

Keep the boundary explicit in the attempt's assistance policy and record any assistance actually delivered. Do not treat a normal operational response as teaching assistance merely because it helps the learner understand what the system did.

### External references are assessment-specific, not universally allowed or banned (Stage 119)

Each assessment must define its permitted resources before the learner starts. An assessment may allow selected operational references where using those references is part of the real work being assessed. Another assessment may restrict references when the intended skill is unaided recall. In all cases:

- do not allow another person to perform or solve the task for the learner;
- do not allow sources that expose hidden case answers or protected assessment criteria;
- make the resource rules visible in the pre-assessment briefing;
- record which resources are made available and any resource use DEIXEN can actually verify.

Do not claim that DEIXEN monitors every external browser, document, or device unless that capability is genuinely implemented and verified. Independent performance means the learner understands, decides, and performs the work under the declared conditions; it does not automatically mean working without professional references.

**Still open:** the exact allowed-resource list for the first reservation assessment; which in-product references can be provided directly; how the product records available/used resources without overstating monitoring; the precise attempt status when prohibited assistance is accidentally delivered; and the minimum fields shown in the pre-assessment briefing. Resolve these against the first validated assessment and actual product capabilities. Do not build browser surveillance, device monitoring, a general proctoring suite, or a complex assessment-control platform as a launch prerequisite.


## 5.18 Post-assessment review, protected learning feedback, and variant reuse (Stages 120–124)

### Provide a useful review after the result is secured (Stage 120)

After an Independent Assessment result is finalized, the learner should receive a review that connects the operational task result with the quality and independence of their performance. At minimum, it should explain:

- the **Task Outcome** — what happened operationally, including a valid no-reservation or escalation outcome where applicable;
- the **Performance Outcome** — what the learner did well and what did not meet the applicable requirements;
- the **independence conditions** — whether the work was independent or whether instructional assistance was actually delivered;
- skill-level evidence — what was Demonstrated, Not Demonstrated, or Not Assessed;
- the next useful learning, practice, or assessment opportunity.

Do not reveal complete model answers, hidden case facts, or the protected solution sequence when the case or its variants remain in use for independent assessment. Give enough information for the learner to understand performance and progress without undermining future assessment integrity.

### Separate immediate performance review from detailed teaching explanation (Stage 121)

Use two levels of feedback:

1. **Post-assessment performance review:** available after the result is secured. It explains relevant strengths, unmet requirements, material errors and their professional impact, self-correction versus assistance, and development needs without exposing the protected answer or full solution sequence.
2. **Detailed teaching explanation:** may explain the correct workflow, operational responses, and reasoning in Learning or Practice when doing so does not expose a still-protected assessment version. Keep this educational explanation separate from the immutable assessment attempt and its result.

The learner must not be denied useful teaching merely to protect an assessment, but assessment feedback must not leak answers that remain in active use.

### Protect active assessment variants while providing alternative teaching (Stage 122)

While a case variant remains in protected independent-assessment use, do not reveal its complete solution to a learner who has attempted it. Provide general teaching about the relevant skill using a different, non-protected practice example. If a variant is formally retired from protected assessment use, it may be converted into a Practice case with a detailed explanation. Retiring or explaining the variant does not alter the learner's original attempt or result. Keep practice content and protected assessment content clearly separated.

### Do not reuse a fully exposed variant with the same learner (Stage 123)

If a learner has seen the complete solution to a particular assessment variant, do not use that same variant again with that learner for Independent Assessment. Select another activated variant that tests the same target skills with appropriately comparable difficulty and complete required metadata; do not replace it with an unconstrained AI-generated case. If no suitable variant is available, defer the assessment rather than offer an unfair repeat.

Exposure is learner-specific: a variant may remain suitable for other learners under its assessment controls, but must be marked as exposed for the learner who received its full solution.

### Handle assessment-variant exhaustion fairly (Stage 124)

If no unexposed, validated variant is available for a learner:

- do not recycle a variant whose complete solution the learner has seen;
- retain the learner's previous evidence and results;
- offer continued development using non-protected practice examples;
- prepare a new versioned variant with complete operational facts, skill/criteria mappings, sensitivity metadata, and required validation state before activation;
- postpone Independent Assessment until a fair, appropriate variant is available.

A shortage of assessment content is a product/content limitation, not a failure or penalty attributable to the learner. Do not make the learner repeat unrelated learning or discard valid evidence because DEIXEN has not yet prepared another assessment variant.

**Still open:** the simplest way to record learner-specific variant exposure; the software state and transition that retire a variant from protected use; the minimum safe feedback granularity for a reusable variant; the required metadata/validation fields for a newly authored variant; and how to make a fair variant available without building a large content-generation platform. Resolve these in the first assessment workflow with a small, versioned set. External approval and human sign-off processes are outside this current software-workflow scope.


## 5.19 Learner-specific assessment exposure and fair variant holds (Stages 125–138)

### Track what each learner has actually seen (Stage 125)

Keep a small exposure record linked to the learner and the specific assessment Case Variant/version. It should distinguish at least:

- **Not attempted / no solution exposure recorded:** no relevant assessment content or answer has been delivered to the learner.
- **Attempted, but no complete solution disclosed:** the learner completed or began an assessment, but the attempt itself does not imply that the solution became known.
- **Complete solution disclosed:** the learner received enough information to reproduce the solution without independently discovering it; that variant must not be reused for that learner's Independent Assessment.

The record should identify the variant/version, the relevant content delivered, whether a complete solution was disclosed, and when the disclosure occurred. A normal performance review does not automatically count as full solution exposure; classify based on what the learner actually received.

For the initial release, use the simplest reliable, attributable record. Do not build a broad content-surveillance or learner-tracking platform.

### Distinguish feedback from complete or partial solution disclosure (Stage 126)

A performance review is not a complete solution merely because it identifies a skill gap or points out an error. Complete solution disclosure occurs when the learner receives information sufficient to reproduce the solution without discovering it independently, such as the full correct execution sequence, the required commands and values for that case, hidden facts the learner was meant to discover, or a model correction sequence that reveals the answer.

When only part of the solution is disclosed, record the actual portion delivered. Do not automatically exclude the entire variant; assess whether the disclosed portion is material to the skills and decisions being measured.

### Assess disclosure against pre-identified sensitive elements using explicit rules (Stage 127)

When authoring a protected assessment variant, identify the facts, steps, or decisions whose disclosure could compromise the fairness of that variant. When content is delivered to a learner, DEIXEN records what was delivered and compares it with those pre-identified sensitive elements. Apply a proportionate response:

- **No material impact:** the variant remains eligible for that learner, subject to the other assessment rules.
- **Limited impact:** review whether the affected skill or criterion can still be assessed fairly; do not automatically disqualify the full variant.
- **Material impact:** do not use the variant for that learner's Independent Assessment.
- **Uncertain impact:** keep the variant temporarily unavailable for Independent Assessment for this learner until the software has enough explicit metadata and rules to classify the effect. Do not guess, silently exclude the whole variant, or invoke a human-review workflow in the current product.

Sensitive elements and their relationships to skills/criteria must be stored as structured variant metadata before the variant is activated. DEIXEN applies only explicit, testable mappings; it does not infer sensitivity from free text.

### Apply a temporary, learner-specific hold while the software resolves disclosure uncertainty (Stage 128)

If there is credible uncertainty about whether solution content was disclosed and the effect is not yet known, temporarily hold that variant from use with the affected learner while the configured deterministic software checks evaluate the available exposure record and mappings. This is an automated data/rule process, not a human-review workflow. The hold is a precaution, not a failed assessment or a negative judgment about competence.

- Do not cancel a previously completed assessment solely because a disclosure concern is under review.
- Allow the learner to continue with non-protected practice examples.
- Offer another validated variant if one is available and suitable.
- Keep the hold specific to the learner and variant; do not disable the variant for everyone without a separate reason.
- If the effect cannot be determined reliably from the configured metadata and deterministic rules, keep the learner-specific hold in place; do not guess or claim the variant is valid.

### Explain the hold to the learner without revealing protected details (Stage 129)

Tell the learner, in neutral language, that this variant is temporarily unavailable to them while its assessment suitability is checked. Make clear that the hold is not a fail or a negative competence judgment and that their earlier evidence and results remain preserved. Where possible, offer an alternative validated assessment variant or non-protected practice. Do not disclose the hidden solution or sensitive content that could further compromise the assessment.

**Still open:** the minimal data fields and event triggers for an exposure record; the exact UI event that counts as displayed content; the controlled content-fragment identifiers; the deterministic mapping from sensitive fragments to skills and criteria; and the simplest learner-facing hold notice. Resolve these as explicit software rules for a small initial set of variants. Do not build browser/device surveillance, automated proctoring, an LLM-based exposure classifier, a complex adjudication engine, or broad investigation case management for launch.


### Determine variant eligibility through deterministic software rules (Stage 130)

DEIXEN must classify whether a specific assessment variant can be used with a specific learner based only on recorded exposure events, structured content classifications, skill mappings, and explicit rules. Use a small set of program states:

- **Eligible:** no recorded exposure affects the skills/criteria being assessed.
- **Eligible for unaffected skills only:** exposure affects a separable skill/criterion, while other skills remain independently assessable under the case rules.
- **Unavailable for this learner:** material exposure compromises a core skill or the validity of the assessment as a whole.
- **Temporarily held:** the available records or mappings are insufficient to determine impact safely.

The system must not call an LLM, infer fairness from free text, or create a human-review workflow to resolve these states. Where rules or mappings are missing, retain the temporary hold and offer another suitable learning/assessment path.

### Record delivery separately from actual in-product display (Stage 131)

Track at least two distinct events:

- **Content Delivered:** the program sent the content to the DEIXEN interface.
- **Content Displayed:** the content became visible in the active DEIXEN interface according to a defined UI event.

Store the content identifier and version, content type, related assessment variant/version, and event time. Do not infer that the learner read or understood content from either event. Understanding must be checked separately through an appropriate learning/knowledge check.

### Classify exposure according to what the interface displayed (Stage 132)

Apply deterministic rules:

1. Content not sent: no exposure event.
2. Content sent but not displayed: record delivery, but do not classify it as disclosed.
3. Part of the content displayed: record the exact content fragment(s) displayed.
4. Complete protected solution displayed: mark the complete solution as exposed for this learner/variant, regardless of whether reading or understanding can be proven. This is a precaution for assessment integrity, not a claim about the learner's knowledge.

### Define display using DEIXEN interface state, not external monitoring (Stage 133)

A content fragment counts as displayed only when the corresponding DEIXEN content area is actually visible/expanded in the active interface. Loading content, storing it in the background, or placing it in a closed/collapsed area does not count. Partial display records only the fragments that became visible; complete display requires all fragments designated as the complete solution to have been displayed. Record these events inside DEIXEN only. Do not monitor the learner's external browser, device, or activity outside the product.

### Pre-classify solution-related content as structured metadata (Stage 134)

Each review/explanation fragment that may affect assessment reuse must have a predefined content classification:

- **General Feedback:** feedback that does not disclose the solution.
- **Sensitive Detail:** information that may reveal part of the solution or a protected decision.
- **Protected Solution:** the model solution or content sufficient to reproduce the answer.

Each fragment must be linked to its case/variant/version, relevant skill or task step, sensitivity classification, and mode-specific display rules. The software applies these stored labels; it does not classify arbitrary text dynamically.

### Apply mode-specific content visibility rules (Stage 135)

Use configured rules for each operating mode:

| Content type | Practice | Scenario | Independent Assessment |
|---|---|---|---|
| General Feedback | Allowed | According to case rules | After the result is secured |
| Sensitive Detail | Allowed under practice rules | According to case rules | Not during the active attempt; after submission, only under the configured protection rules |
| Protected Solution | Allowed | Only when the case/version permits it | Not during the active attempt |

A retired assessment variant may be made available as Practice with its detailed solution. Once a learner has been shown that solution, mark the variant as exposed for that learner and do not reuse it with them for Independent Assessment. Record what was actually displayed.

### Map sensitive content fragments to affected skills and criteria (Stage 136)

Every Sensitive Detail or Protected Solution fragment must be mapped in advance to the skill(s), task step(s), and assessment criterion/criteria it may affect. When the fragment is displayed, use that mapping to determine which evidence may be compromised. If the mapping is missing or ambiguous, keep the variant on hold for that learner rather than guessing.

### Limit exposure impact to the affected skills where possible (Stage 137)

A disclosed fragment must not automatically invalidate every skill in the case. Apply these rules:

- Do not use the affected skill/criterion to claim independent performance if the disclosure compromises the learner's ability to demonstrate it independently.
- Other skills may still be assessed when their evidence is genuinely separate and the case criteria permit that separation.
- If the exposure compromises a core skill or the overall task outcome, mark the assessment variant unavailable for this learner as a whole.
- Never change the case criteria or assessment rubric mid-attempt to work around a disclosure event.

### Separate overall assessment validity from skill-level evidence (Stage 138)

Store the assessment-level validity state separately from each skill's evidence result. For the initial product, the assessment-level state may be:

- **Valid:** the attempt can support the intended assessment conclusions.
- **Limited:** only specified unaffected skills/criteria can support independent evidence.
- **Invalid for Independent Assessment:** the disclosure compromises the overall task or a core skill such that the attempt cannot support the intended independent result.

At skill level, retain the normal evidence outcomes (Demonstrated, Not Demonstrated, Not Assessed) while also recording when a skill is **excluded from independent evidence due to solution exposure**. Do not mislabel an exposure-excluded skill as Not Demonstrated or Not Assessed. Preserve all valid unaffected evidence, but do not infer overall task competence from a partial subset of skills. Preserve the attempt and its event history even when its independent-assessment validity is limited or invalid.

**Current implementation boundary for Stages 130–138:** all exposure recording, content visibility, classification, skill mapping, eligibility decisions, holds, and assessment/skill validity states are deterministic software behavior based on structured metadata and explicit rules. No LLM or human-review workflow is part of the current product flow. If the software lacks enough data to decide, it keeps the learner-specific variant on hold and offers a safe alternative; it does not guess.


## 5.20 Assessment result validity, issue reporting, and versioned rule correction (Stages 139–143)

**NOW — Frontend/Engine:** implement the learner-facing report flow, deterministic checks, rule-version references, and additive corrected-result logic. **LATER — Backend:** persist and protect reports, event history, rule versions, and corrected results durably for production.

### Present limited or invalid assessment outcomes clearly (Stage 139)

The learner-facing result must distinguish overall assessment validity from skill evidence:

- **Valid:** show the assessment result and the skills for which evidence is valid.
- **Limited:** explain that only specified unaffected skills/criteria can support conclusions; show those valid skill records and identify which skills could not be used to prove independence because of prior solution exposure. Offer an appropriate later opportunity for affected skills.
- **Invalid for Independent Assessment:** explain that the attempt cannot support a reliable independent-assessment result; preserve the attempt and any usable records, do not label the learner as having failed solely because validity was compromised, and offer suitable practice or another assessment opportunity.

Do not reveal the protected solution or sensitive details that caused the validity limitation. Keep the explanation factual and learner-understandable.

### Allow the learner to report a possible result issue (Stage 140)

Provide a simple **Report Result Issue** action from the assessment result. The learner may identify the part of the result they believe is wrong and add a short explanation. Where relevant, the report should be linked to the original Attempt and the result/rule version that produced it.

Submitting a report does not automatically change the result, delete evidence, or rewrite the original assessment record. This is a narrow product function for recording a possible result error, not a ticketing, complaints, or institutional case-management system.

### Show a clear software status for the report (Stage 141)

The learner can see a simple status for the submitted report:

- **Received:** the report has been saved and linked to the Attempt.
- **System Check in Progress:** the deterministic checks are being run or completed.
- **Result Corrected:** a corrected result record has been created and linked to the original.
- **No Change:** the checks found no rule/data error that changes the result; show a concise explanation.
- **Unable to Verify Automatically:** the stored data/rules are insufficient to reach a reliable software conclusion; preserve the original result and explain that no automatic correction was made.

The current product does not introduce a human-review workflow behind these statuses. Do not imply a manual review is happening. The report must not prevent the learner from continuing Learning or Practice.

### Recheck using the original attempt data and original rule version (Stage 142)

The program checks a reported result issue using the data that produced the original result, including where available:

- the original command/response/event history and operational state;
- the exact Case Package, Variant, and version used;
- the exact assessment rule version used;
- the content-delivery/display and solution-exposure records;
- the links between exposed content, affected skills, and assessment criteria.

The check must be deterministic and reproducible. It must not silently substitute a newer rule version when reproducing the original outcome. If the available records do not permit a reliable automated conclusion, record **Unable to Verify Automatically**, retain the original result, and do not guess.

### Preserve and version assessment rules; correct outcomes additively (Stage 143)

Every finalized assessment result must retain the exact version of the assessment rules that produced it, together with the relevant case/variant version and attempt data. DEIXEN must be able to reproduce the original result using that original rule version.

If a software defect is established in an assessment rule:

1. Preserve the original rule version unchanged.
2. Create a corrected rule version with a new version identifier; do not edit the historical version in place.
3. Define the correction's applicability and the conditions under which prior attempts are eligible for rechecking.
4. Re-evaluate only the affected attempts using the corrected version and the original attempt data.
5. If the result changes, create a new corrected-result record linked to the original result, the original Attempt, and the corrected rule version.
6. Preserve the original outcome and all earlier records; never silently overwrite, delete, or rewrite assessment history.

A corrected rule version does not automatically mean every historical attempt must be re-evaluated. Its applicability must be explicit and testable. The distinction between reproducing an old decision and issuing a corrected decision must remain clear to the learner and in the evidence record.

**Current implementation boundary for Stages 139–143:** result validity display, issue reporting, report status, deterministic rechecks, rule version retention, and additive corrected-result records are software behavior based on structured data and explicit rules. No LLM or human-review workflow is part of this current product flow.

**Still open:** the precise fields in the minimum Report Result Issue form; the deterministic checks run for each issue type; how the software identifies attempts affected by a rule defect; the applicability/eligibility conditions for a corrected rule version; and the concise learner-facing explanation for each report outcome. Resolve these as a small set of explicit, testable rules for the first assessment workflow rather than building a general issue-management platform.


## 5.21 Corrected-result propagation, recommendation lifecycle, and evidence recalculation (Stages 144–149)

**NOW — Frontend/Engine:** implement the deterministic dependency recalculation, recommendation superseding, temporal eligibility, and evidence-set calculations. **LATER — Backend:** preserve these versioned relationships and corrections durably and securely across user sessions/devices.

A corrected assessment result must change the current accepted conclusion for the original Attempt without rewriting the historical record or creating a second performance attempt. The correction must also propagate to product information that depends on that result, while respecting the difference between activities not yet started, attempts already in progress, and attempts already completed.

### Treat the corrected result as the current result for the same Attempt (Stage 144)

- The corrected result becomes the current accepted result for that same Attempt.
- The original result remains preserved as a historical, superseded record and is explicitly linked to the corrected result; both retain their applicable assessment-rule version references.
- Growth and current competency calculations use the corrected result as the current outcome for that Attempt. They must not count both the original and corrected records as two performances.
- A correction changes the evaluated conclusion about the past performance; it does not change what the learner actually did at the time or create a new performance event.

### Recalculate only the derived information that depends on the correction (Stage 145)

When a corrected result changes information used by other product functions, DEIXEN must deterministically recalculate only the affected dependent outputs. These may include the learner's Growth/skill position, development recommendations, and eligibility or access to activities and scenarios.

- Do not rewrite unrelated attempts, evidence, or historical events.
- Update dependent views and future access decisions from the corrected result and the remaining valid evidence.
- Make the learner aware when displayed progress or next-step information changes because an earlier result was corrected; the explanation should be factual and should not expose protected assessment content.

### Supersede recommendations that were based on the old result (Stage 146)

- A recommendation that is no longer appropriate after correction is marked **Superseded**; it is not deleted or silently rewritten.
- Preserve its link to the result and evidence that originally caused it to be issued.
- Where a different development need remains, create a new recommendation based on the corrected result and current evidence, with a clear link to the basis for the new recommendation.
- A superseded recommendation must not remain active as though its invalidated basis were still current.

### Apply corrected eligibility prospectively to activities not yet started (Stage 147)

- Recalculate eligibility for scenarios and activities the learner has not started, using the corrected current competency/evidence position.
- Once an Attempt has been successfully created and stored under the start boundary in Stages 150–155, preserve the eligibility decision and rule version under which it began. A click, preview, or unconfirmed start request alone does not freeze eligibility. A later correction to an earlier prerequisite must not silently change the in-progress attempt's conditions or stop it solely because the prerequisite status changed.
- If the correction reveals a defect in the validity of the in-progress attempt's own assessment basis or result, handle that through the established result-correction path; do not alter the running attempt through an unrelated eligibility update.

### Do not automatically invalidate completed attempts because an earlier prerequisite changed (Stage 148)

A completed attempt that was eligible when started is not automatically invalidated merely because a prior result used to establish its entry eligibility is later corrected.

- Evaluate the completed attempt using its own recorded facts, case/variant version, attempt conditions, and applicable assessment-rule version.
- If the completed attempt's own performance evidence and assessment basis are unaffected, retain its evidence as valid for the relevant skill calculations.
- If the completed attempt itself was affected by an assessment-rule defect, use the versioned result-correction process; do not invalidate it solely due to a changed historical prerequisite.
- A prior eligibility correction still governs future access decisions; preserving a completed attempt does not restore the corrected prerequisite status.

### Recalculate competency from the complete set of valid evidence (Stage 149)

- Calculate current skill position from the full set of relevant valid evidence, not from the corrected result in isolation.
- For the corrected Attempt, use the corrected result in place of its superseded original result; never double-count both.
- Retain other valid completed attempts and evidence, including attempts whose entry eligibility remains historically valid under Stage 148.
- Do not assume that correcting one result necessarily removes or establishes a skill. The resulting skill position depends on all remaining valid evidence and the defined competency rules.
- Recalculate future activity/scenario eligibility from that resulting skill position.

**Boundary:** corrected conclusions and their dependent future-facing outputs may change; historical actions, unrelated evidence, and the recorded conditions of already-started attempts are not rewritten.




## 5.22 Attempt start boundary, safe creation, and duplicate-request protection (Stages 150–152)

These stages complete the attempt-start rules introduced for Independent Assessment in Stage 116 and clarify the corresponding boundary for scenario activities that create an Attempt. They define when a case/activity becomes an actual attempt, what must be recorded before attempt-governed work can execute, and how repeated start actions are handled. The product rules are to be implemented and tested now in the local deterministic Engine; stronger durable and cross-device guarantees are completed later through Backend.

### Previewing a case is not starting an attempt (Stage 150)

- Opening Scenario Bank, viewing a case brief, reviewing task context, or entering a pre-start briefing does not create or consume an Attempt.
- Until the learner confirms the applicable start action for that activity/mode (for example, **Start Scenario** or **Start Assessment**), eligibility can be recalculated when relevant prerequisites or corrected results change.
- When the learner requests the start, DEIXEN rechecks eligibility against the latest computed skill/evidence position and the applicable current rules. A stale eligibility display must not authorize a start.
- If the learner is no longer eligible, the Engine rejects the start request with a clear explanation. No Attempt is created and no failure is recorded against the learner.
- If eligible, the Engine creates the Attempt using a snapshot of the case/variant version, eligibility basis, applicable task/assessment rule version, and assistance policy for that activity/mode.
- The actual attempt begins only after that Attempt record has been successfully created and stored. The button click alone is not the start boundary.

### An Attempt must exist before attempt-governed work executes (Stage 151)

- The Engine must successfully create and record the Attempt in the current phase's local attempt store before allowing any command or operational action governed by that Scenario/Assessment attempt to execute. This local record is sufficient for prototype behavior testing only; it is not a production durability guarantee.
- The record must have a stable Attempt identity and be linked to the exact case, variant, relevant versions, eligibility snapshot, and assistance policy.
- If creation clearly fails, the attempt remains unstarted; no attempt-governed command may run and no attempt is consumed.
- If creation returns an uncertain result (for example, the interface loses the response), the program must check whether the Attempt record already exists before retrying. It must not blindly create another Attempt.
- If the record exists, DEIXEN recovers that same Attempt and its current state. It must not ask the learner to start over or generate a second record.
- If the Engine cannot determine whether creation succeeded, it must keep execution blocked until the state is resolved from available data. It must not guess or allow operational work without a verified Attempt identity.

### One start action must not create duplicate Attempts (Stage 152)

- The first deliberate start action creates one logical start-request identity. Repeated clicks, double taps, retries, or resubmissions while that same start flow is pending reuse that identity and are treated as one request.
- While that request is pending, show its current state and prevent a second Attempt from being created for the same request. Do not generate a fresh request identity merely because the interface timed out or the learner tapped again.
- If an Attempt was already created for the request, return/reopen that same Attempt instead of creating another.
- If multiple identical start requests reach the current local Engine, its duplicate-request protection should resolve them to one Attempt. The exact start control depends on the mode; the protection applies to the same logical start intent, not to every later, deliberate attempt.
- A genuinely new attempt may be created later only after the previous start flow has reached a known state, through a new, deliberate start action with a new request identity, and only when the activity/assessment rules allow it. Duplicate protection must not become a permanent ban on valid future reassessment.

### Implementation boundary for Stages 150–152

**NOW — Frontend/Engine:** implement a clear pre-start/start-pending/created/rejected/failed-or-uncertain state flow for every relevant attempt-creating mode; use a stable request identity within the local prototype; prevent duplicate clicks and repeated submissions; test recovery of an already-created Attempt; and block attempt-governed commands until the created Attempt is confirmed.

**LATER — Backend:** enforce durable Attempt creation, idempotency, uniqueness, and transaction safety on the server. The Frontend cannot guarantee that two devices or concurrent clients will never create duplicate Attempts by itself. Cross-device concurrency guarantees are a Backend requirement and must not be claimed during the current local phase.

## 5.23 Eligibility corrections, active start requests, and refreshed scenario access (Stages 153–155)

These proposals close the remaining interaction between corrected-result propagation (Stages 144–149) and the attempt-start boundary (Stages 150–155). They define intended behavior when a correction and a learner's start request occur close together, when eligibility changes after the learner has opened a case, and when eligibility is later restored before the attempt begins.

### Resolve a correction/start race at one recorded start boundary (Stage 153)

- A start request and a correction that changes eligibility must be ordered by the Program Engine; neither operation may silently overwrite the other.
- At the point the Attempt is successfully created and recorded, the Engine uses the latest eligibility state applied before that creation point.
- If the relevant correction is applied before the Attempt record is successfully created, the start check uses the corrected eligibility. If the Attempt record is successfully created first, that Attempt retains the eligibility snapshot and rule versions recorded at creation; a later correction does not rewrite its starting conditions.
- No attempt-governed operational action may execute until this start boundary is resolved and the Attempt record exists, consistent with Stages 150–155.
- If the Engine cannot establish the order or determine whether Attempt creation succeeded, it blocks execution and avoids creating another Attempt until the state can be recovered. It must not guess which operation happened first.

**NOW — Frontend/Engine:** define one explicit local commit point for Attempt creation, apply eligibility updates in a controlled order, and test correction-before-create, create-before-correction, and uncertain-response sequences in the local/single-user prototype. The exact internal implementation technique remains open; do not build distributed infrastructure prematurely.

**LATER — Backend:** enforce cross-client ordering, durable transactions, and authoritative concurrency handling when multiple devices/sessions can submit corrections or start requests at the same time. Local tests do not prove multi-user atomicity.

### Refresh an opened case when eligibility is lost before start (Stage 154)

- Opening a case or reading its brief does not freeze eligibility and does not create an Attempt.
- If a relevant correction changes the learner's eligibility before the start boundary, the Engine recalculates the case state and the open Scenario Bank view must stop presenting the old eligibility as current.
- If the learner is no longer eligible, the start action is blocked and no Attempt is created or consumed. This is not a learner failure.
- Explain that eligibility changed since the case was opened. Show the specific unmet prerequisite only when the underlying rule and information are safe to disclose; do not expose protected assessment criteria, answers, or variant facts.
- If the Engine cannot determine a reliable reason from recorded data and explicit rules, show a neutral unavailable/temporarily-checking state and block start rather than inventing a reason.
- Where the missing prerequisite is safe to identify, the interface may point the learner to the relevant Learning or Practice activity. It must not assume a weakness or generate a recommendation unsupported by evidence.

**NOW — Frontend/Engine:** test the open-case → eligibility-changed → refreshed-view flow, including protected-reason masking and uncertain-state handling.

**LATER — Backend:** synchronize eligibility changes reliably across sessions/devices and ensure stale client screens cannot authorize a production start.

### Restore availability without automatically starting an attempt (Stage 155)

- If a later correction restores the prerequisite evidence and the learner becomes eligible again before starting, the Engine recalculates the affected eligibility and the Scenario Bank may show the case as available again.
- Restoring eligibility does not create an Attempt, consume an attempt, or launch the scenario automatically.
- The learner remains in control and must deliberately request the start. At that point the Engine repeats the eligibility check under Stage 153 and creates an Attempt only if the current state permits it.
- A period of temporary ineligibility and later restoration is not recorded as a failed assessment or negative competence evidence.
- If the recalculated state remains uncertain, the case stays unavailable/temporarily held until the Engine can determine eligibility from explicit data; do not infer eligibility from an older screen state.

**NOW — Frontend/Engine:** test available → unavailable → available transitions before start, verify that no Attempt is created during status changes, and verify that an explicit new start request rechecks current eligibility.

**LATER — Backend:** provide reliable cross-session and cross-device refresh and authoritative server-side eligibility enforcement for production.

**Boundary across Stages 153–155:** the Attempt's successful creation is the recorded boundary. Before it, corrected eligibility controls whether the learner may start; after it, the Attempt retains its starting snapshot. If ordering or creation cannot be verified, hold execution safely. These are proposals for local Engine and later Backend behavior, not proof that either guarantee is implemented.


# 6. Development sequence — what to build now and what to defer

The sequence below records the owner's current work order. It separates what may be prototyped now from production infrastructure to add later. It is not final product-scope approval, authorization to implement every proposal, or evidence that any gate has passed.

## Phase A — Current priority: Frontend and deterministic Program Engine

This is the current owner-directed development priority for the next implementation phase, subject to final review of the product proposals.

### A1. Verify and bound the operational foundation

- Inspect the current repository and actual training engine to confirm the supported command/workflow scope.
- Select one bounded representative professional task.
- Define verified operational facts, supported actions, expected states, and explicit out-of-scope boundaries before activating the first case.
- Verify every command, response, warning, and resulting state that DEIXEN will teach or assess.
- Do not include ticketing, payment, live availability, fare comparison, or adjacent functions unless verified and deliberately included.

The earlier narrow booking slice was discussed around one adult, one passenger, one segment, and one fare context, with a candidate command sequence such as AN → SS → NM → AP → SRCTCM/CTC → TK → RF → ER → FXP (FQD was optional in one earlier discussion). Treat this as a historical candidate only. It must be checked against the current repository, current training engine, and authoritative operational references before it becomes the launch-case specification.

### A2. Build the Frontend and Engine vertical slice

- Build the minimum useful Home, Learning, Terminal, Scenario Bank, and Growth journeys around the selected task.
- Implement business rules and state transitions in a deterministic Program Engine, separated from UI components.
- Complete the learning-to-practice path, including understanding checks and only the useful Ghost/Coach behaviors.
- Build one central Terminal supporting Practice, Scenario, and Independent Assessment modes.
- Build the first versioned Case Package and controlled customer facts, with deterministic text interaction.
- Preserve conversation, task, and operational states separately.
- Validate actual operational state against the latest customer-confirmed and authorized request.
- Support correction, interruption, recovery, escalation, incomplete outcomes, and professionally correct no-reservation outcomes where the case permits them.
- Implement the current result/evidence model, exposure controls, result issue checking, versioned corrections, Growth recalculation, and future-eligibility rules in a form that can be tested locally.
- Implement Stages 150–155 in the local Engine: explicit preview/start boundary, safe Attempt creation, duplicate-request protection, correction/start ordering, stale eligibility refresh, and eligibility restoration before start within the current single-user/client environment.
- Use transitional local persistence only as needed to test product behavior. Keep its boundary replaceable and do not describe it as secure production storage.

### A3. Validate the local prototype

- Test happy paths and failure paths with deterministic fixtures and controlled scenarios.
- Verify every state transition, command/response link, result, correction, recommendation, eligibility change, and evidence calculation.
- Test repeated clicks, delayed responses, reloads, ambiguous start outcomes, correction/start ordering, eligibility loss while a case is open, and eligibility restoration before start in the local/single-client environment.
- Test with genuine beginners and relevant practitioners, not only the founder.
- Resolve usability, language, accessibility, and product-logic defects before starting Backend integration.

**Exit condition for Phase A:** the owner has enough evidence that the core Frontend and Program Engine behave as intended, that their data/service needs are understood, and that the product is ready to be prepared for Backend integration. The transition into Backend preparation/implementation is made only when the owner decides the product has reached that point. This is not yet a public production-launch approval.

## Phase B — Prepare the Backend boundary (design only after the core is validated)

- Identify which validated Engine operations require server-side persistence or enforcement.
- Specify the data that must be durable and the service contracts required by the Frontend/Engine.
- Confirm migration needs from local test data and decide what prototype data should or should not be carried forward.
- Keep this phase grounded in tested behavior; do not prebuild speculative APIs or infrastructure during Phase A.

## Phase C — Later implementation: Backend for production launch

Backend implementation is deferred until Phases A and B provide a stable basis. Before a real production launch to external learners, implement and test as applicable:

- durable server-side storage for users, attempts, command/event history, task/operational states, assessment results, evidence, rule versions, exposure records, recommendations, and corrections;
- authentication, authorization, ownership, and server-side least-privilege access;
- transaction-safe attempt creation and server-enforced uniqueness/idempotency for concurrent or repeated requests across clients/devices;
- reliable synchronization, pause/resume, backup/restore, and recovery across sessions/devices;
- server-side protection against client tampering with protected results and evidence;
- appropriate security/access logs, deployment, monitoring, and operational safeguards.

The actual database, APIs, hosting, identity provider, and service architecture remain open until the validated Frontend/Engine requirements are known. Backend is required before a genuine production launch to external learners; it is not required to begin the current Frontend/Engine work.

## Phase D — Future product expansions

Only after the core is validated and production foundations are appropriately established should DEIXEN consider, on their own merits:

- DEIXEN World / Virtual Company;
- LLM-assisted customer expression/personality and optional voice;
- multi-customer/shift simulation and Shift Evidence Record;
- expansion to additional GDS platforms;
- large scenario catalogues and advanced analytics.

World/LLM are not included in the current priority and are not a prerequisite for the core product or initial Backend. Human/trainer/institutional workflows remain outside this current scope unless separately reconsidered by the owner.

---

# 7. Deferred implementation and out-of-scope directions

These earlier discussion outcomes are preserved as provisional proposal directions where relevant, but their implementation timing or scope differs. Backend is a required later implementation phase; human/institutional workflows are outside the current product scope; World/LLM and other expansions are future options.

## 7.1 Backend implementation — deferred, not cancelled

Backend is a required later implementation phase for production operation, but its development is intentionally postponed. Do not interpret the deferred Backend implementation as cancellation of server-side persistence, accounts, security, access control, synchronization, evidence protection, or cross-device concurrency requirements. Their scope is described in Sections 0 and 6 and must be based on the validated Frontend/Engine.

## 7.2 Human and institutional workflows — outside current product scope (Steps 61–89)

The human/trainer/institutional mechanisms discussed in these stages are **outside the current software workflow scope**, not hidden launch requirements or automatic future Backend features. They include:

- formal independent review of disputes about trainer recommendations;
- a bounded second-review route with detailed eligibility and appointment rules;
- periodic institutional sampling and indicator-driven quality audits;
- formal defect-severity classification for trainer reviews;
- temporary trainer-permission safeguards during investigations;
- external reviewer procurement, independence, remuneration, confidentiality, and conflict-of-interest process;
- full institutional intervention records and lifecycle state management;
- independent corrective-action verification, multiple verification outcomes, and reopening closed interventions.

**What remains essential in the current product:** preserve the learner's own evidence and correction history, keep learner-facing explanations truthful, and design data boundaries that do not expose unrelated records. These are software integrity principles, not a requirement to build human review, trainer access, disputes, or institutional administration.

Do not build a governance console, trainer portal, investigation case-management system, external reviewer marketplace, staff disciplinary workflow, or enterprise quality-management suite as part of the current scope.

## 7.3 Human trainer recommendation lifecycle — outside current scope

This subsection records the narrower trainer-recommendation decisions from the earlier stages; it does not add another workflow beyond the exclusion in Section 7.2. The principle that a human trainer's recommendation does not prove competence remains valid as a boundary, but human trainer recommendations and their lifecycle are not part of the current software workflow. The following capabilities are excluded from the current scope:

- multiple recommendation status transitions;
- a full learner/trainer disagreement state machine;
- formal independent adjudication of recommendation completion;
- second reviews and repeated dispute handling;
- extensive institutional escalation rules.

Do not implement these human recommendation/response workflows now. This does not affect deterministic system-generated development recommendations in Stages 105–106 and the superseding/recalculation behavior in Stages 145–146, which remain current product logic.

## 7.4 Future product expansions — not current dependencies

Do not make these prerequisites for the current Frontend/Engine vertical slice or the core product's initial production release:

- DEIXEN World / Virtual Company with cinematic 3D characters and workplace scenes;
- simulated multi-customer work shifts and Shift Evidence Record;
- mandatory voice or speech recognition; text-first is acceptable;
- expansion to multiple GDS platforms;
- a large case catalogue before the first cases are validated;
- advanced institution dashboards, aggregate analytics, broad employer portals, or HR functions;
- detailed employment, disciplinary, contracting, and legal investigation workflows.

These items may be reconsidered only when validated user need, operational capability, commercial value, and implementation cost justify them.

---

# 8. Proposal-stage history — preserved, provisional, and prioritized

This table preserves the history of proposals and their provisional treatment in the current draft. The owner's stage-by-stage “موافق” means **provisionally accepted for inclusion and continued review only**; it does not make the proposal a final product decision. The review may confirm, revise, combine, reject, or defer any item. Read the treatment together with Section 0: **NOW** means proposed Frontend/Engine priority; **LATER** means a retained proposal whose Backend implementation is postponed; **FUTURE** means a separate expansion proposal; and **OUT OF CURRENT SCOPE** means excluded from the current software workflow unless the owner reopens it. The table is not a verbatim reconstruction of every early discussion step. Stages 1–33 remain thematically consolidated; stages 36–42 were recovered individually from owner-provided chat text. Phrases such as ‘Core product behavior’ or ‘Launch target’ in the table describe the current proposal's intended role, not a final approval or a verified capability.

| Stage / source range | Proposed direction / theme | Provisional treatment in this draft |
|---|---|---|
| Steps 1–33 | Foundational principles: professional task first, real independence, assistance integrity, evidence levels, customer correctness, case definition, source-of-truth separation, progressive learning, Home/Scenario/Terminal/Growth roles, World boundaries, and recovery | Preserved in Sections 2–6; early stage numbering remains thematically consolidated, not reconstructed one by one |
| 34 | Learning tracks and hierarchy; completion distinct from understanding | Core product behavior |
| 35 | One central Terminal with distinct modes | Core product architecture |
| 36–42 | Terminal responsibilities; separate conversation/task/operational states; learner-initiated closure and DEIXEN validation; mode-specific review; information-source separation; command lifecycle; history/state/progress separation | Core product behavior |
| 43 | Session interruption, continuity, recovery, and integrity conditions | **NOW:** local/single-user state and recovery behavior. **LATER:** durable cross-device recovery and server guarantees through Backend |
| 44–48 | Scenario Bank organization, case brief, skill-based access, versioned case/run/attempt/session concepts, Scenario-to-Terminal handoff | Core case/assessment foundation; keep first implementation small |
| 49–51 | Case-grounded customer behavior, text/optional voice, continuity across channels, fairness | Controlled text-based customer interaction is launch-relevant; voice can wait |
| 52–58 | Separate task outcome/review/debrief/evidence; competency-led Growth; evidence set not average; learner-facing/internal evidence; corrections; evidence currency; development history | Core evidence and Growth principles; final presentation can be staged |
| 59–60 | Private-by-default evidence, separate sharing routes, trainer review additive rather than destructive | **NOW:** private-by-default product design and no broad sharing. **LATER:** enforceable accounts/access and durable evidence via Backend. Human trainer-review workflow is outside current scope |
| 61–63 | Trainer least-privilege access; substantive notes visible; learner response/flag; original records preserved | Human/trainer review flows are outside current scope. Preserve evidence integrity and private-by-default design now; Backend later enforces learner account ownership and security, but this does not approve trainer access features |
| 64–68 | Recommendations advisory; learner response distinct from proof; performance evidence required; recommendation status distinct from competency; learner/trainer actions attributable | Human trainer recommendations/responses are outside current scope. System-generated recommendations remain current deterministic product logic; recommendations never substitute for performance evidence |
| 69–73 | Separate learner/trainer positions, independent dispute review where possible, reasoned outcomes, recommendation follow-up separated from competence, bounded second review | Human dispute/adjudication workflows are outside current software scope. Retain only relevant no-overwrite and evidence-integrity principles; do not treat these as Backend features |
| 74–78 | Institutional oversight, sampling, trainer-quality defect classification, temporary safeguards | Outside current product scope; any reconsideration requires a separate owner decision |
| 79–83 | Role-appropriate notification, scoped oversight authority, small-institution safeguards, limited external review, reviewer independence | Human/institutional procedures are outside current product scope; preserve privacy/transparency principles only where relevant to the learner's own software record |
| 84–88 | Intervention records, lifecycle states, independent verification, verification outcomes, reopening closed interventions | Outside current product scope; reconsider only if the owner explicitly reopens this scope |
| 89 | Role-appropriate access to institutional information; separate personal summaries from full intervention files; log access | Preserve the principle of least-privilege and relevant disclosure. Full intervention-file UX is deferred with institutional governance. |
| 90 | First launch task direction: create a simple new reservation for one adult/passenger, one segment, and one fare context | Launch target, subject to verification against current engine, repository, and authoritative operational references; payment, ticketing, live availability, and fare comparison are not assumed |
| 91 | Success requires a saved and retrievable reservation matching the latest confirmed request, with professional closure | Core task-validation rule; reservation is not ticket issuance and proves only the defined scope |
| 92 | Separate blocking errors, warnings requiring attention, and unknown/unsupported behavior | Core operational-truth and task-validation rule; do not treat PNR presence alone as success |
| 93 | Customer discovery and clarification are part of the professional task; distinguish confirmed, missing, and uncertain information | Core learning and scenario behavior; information disclosure must be designed per case objective |
| 94 | Simulated customer is natural in dialogue but constrained by authored case facts; must not validate assumptions or invent unknown facts | Core scenario-integrity rule; text-first customer interaction is sufficient for initial launch |
| 95 | Confirm essential details with the customer before reservation execution, without redundant questioning | Core first-task behavior; customer confirmation does not itself change booking state |
| 96 | Separate confirmation that request details are correct from explicit authorization to create the reservation | Core professional-consent boundary; reservation authorization does not authorize payment or ticket issuance |
| 97 | If the request changes before execution, stop using the old request, clarify/reconfirm, and renew authorization when material | Core task-state rule; conversation change never silently updates operational state |
| 98 | If the request changes during execution, pause dependent steps, preserve events, verify engine state, and use only supported recovery | Core recovery/integrity rule; no assumptions or blind command retries |
| 99 | If the request changes after reservation creation, preserve the original booking event and record a separate change request; only verified modification can align it to the new request | Historical and state-integrity rule; post-creation changes remain outside the first launch task |
| 100 | Respect customer withdrawal before reservation execution; do not create without current authorization, and verify any action already taken | Core professional boundary; a correct stop may be a valid outcome, not learner failure |
| 101 | A case may have a valid professional outcome without a reservation; define allowed outcomes in each Case Package | Core case and assessment principle; assess the learner's decision, not only whether a PNR exists |
| 102 | Separate Task Outcome from Performance Outcome | Core evidence model; operational result and quality of learner performance are related but not interchangeable |
| 103 | Distinguish Demonstrated, Not Demonstrated, and Not Assessed for each relevant skill | Core evidence-fairness rule; lack of opportunity is not negative evidence |
| 104 | Do not repeat a whole scenario solely because a skill was Not Assessed; offer a later suitable opportunity and add new evidence | Core learner-journey and evidence-continuity rule |
| 105 | Select the next activity according to skills needing a fair opportunity, not by assuming weakness | Core adaptive learning direction; avoid unnecessary repetition |
| 106 | Match the next step to the need: understanding, practice, transfer scenario, or eligible independent assessment | Core progression principle; explain suggestions without exposing protected assessment criteria; validate simple rules before any complex adaptive engine |
| 107 | Independent-assessment eligibility depends on task-related understanding, a suitable demonstration, and a fair practical opportunity; reliable prior evidence may count | Core assessment-preparation rule; no fixed lesson/attempt count and no requirement to master the task before assessment |
| 108 | Practice errors do not automatically block assessment; address essential misunderstandings before the independent attempt | Core fairness and operational-safety rule; error count alone is not an eligibility test |
| 109 | An unsuccessful independent assessment is preserved; after the result is secured, the learner receives a review and targeted development route before a new eligible attempt | Core assessment and learner-development rule; no repair of sealed attempts or arbitrary attempt limits |
| 110 | Use controlled variants for later assessment to test transfer rather than answer recall | Core assessment-integrity direction; preserve target skills, criteria, and comparable difficulty; no unconstrained AI-generated assessment facts |
| 111 | Ensure each assessment variant has verified operational content, consistent skills/criteria, and comparable difficulty before activation | Launch quality gate: require complete versioned content and validation metadata; no automated LLM-based variant generation or difficulty judgment |
| 112 | Permit Independent Assessment at the first eligible opportunity; no fixed practice-attempt count | Core assessment access rule; eligibility is based on preparation evidence, not repetition count |
| 113 | DEIXEN determines and explains eligibility; the learner chooses when to start | Core learner-control rule; no automatic assessment launch |
| 114 | Preserve eligibility and prior evidence when the learner delays; recheck only affected prerequisites after material changes | Core progression/reliability rule; delay is not negative competence evidence |
| 115 | Provide a concise pre-assessment briefing on task, independence rules, evidence capture, and post-submission behavior | Core assessment UX; no hidden answers or protected criteria disclosed; allow exit without starting |
| 116 | Create the formal Attempt only after explicit Start Assessment confirmation; bind case/version/rules and record events | Core assessment integrity and traceability; interruption does not erase the attempt |
| 117 | Record help requests separately from help actually delivered; denied requests alone do not invalidate independence | Core assistance integrity; accidental delivery is reviewed based on actual exposure |
| 118 | Separate operational information and ordinary UI functions from prohibited instructional help or work performed for the learner | Core independent-assessment boundary; operational output is not automatically teaching assistance |
| 119 | Define permitted external references separately for each assessment; prohibit another person solving the task and sources exposing protected answers | Core assessment-condition rule; track only resources made available or usage DEIXEN can actually verify; no unsupported monitoring claims |
| 120 | After result finalization, review Task Outcome, Performance Outcome, independence, skill evidence, and the next useful step | Core post-assessment feedback; protect reusable case facts and solution sequences |
| 121 | Separate immediate performance review from detailed teaching explanation | Core feedback design; detailed teaching belongs in separate Learning/Practice content when safe |
| 122 | Do not reveal full solutions for active protected variants; teach the skill through a different example; retired variants may become Practice content | Core assessment integrity and learner development; keep attempt results immutable |
| 123 | Do not reuse a fully exposed variant with the same learner for another independent assessment | Core reassessment fairness; use a validated alternate variant or defer |
| 124 | If suitable variants are exhausted, retain evidence, continue non-protected practice, prepare a new versioned variant with required metadata, and defer assessment until it is valid for activation | Core software fairness rule; content shortage is not learner failure and does not justify answer-exposed repeats |
| 125 | Keep a minimal learner-specific record of assessment-variant exposure, distinguishing an attempt from actual complete-solution disclosure | Core reassessment fairness; record what content reached the learner and when, without treating every attempt or review as solution exposure |
| 126 | Define complete solution disclosure by whether the content lets the learner reproduce the solution; record partial disclosure proportionately | Core feedback/assessment boundary; ordinary performance feedback is not automatically a full solution |
| 127 | Pre-identify sensitive variant elements and apply proportional impact rules to disclosed content | Core software fairness control; sensitive elements are structured metadata and uncertain cases enter a learner-specific hold rather than a human-review workflow |
| 128 | Temporarily hold a variant only for the affected learner while deterministic software checks resolve uncertain disclosure; preserve previous results and offer other learning/opportunities | Core automated proportionate safeguard; no human-review flow, and suspicion alone does not invalidate a prior result or disable the variant globally |
| 129 | Explain a learner-specific variant hold neutrally, preserving evidence and offering an alternative where possible without revealing protected details | Core learner communication and trust; the hold is not a fail or competence judgment |
| 130 | Determine variant eligibility for each learner using explicit exposure records and deterministic rules | Core software behavior; use Eligible, Eligible for Unaffected Skills Only, Unavailable for This Learner, and Temporarily Held states; no LLM or human-review workflow |
| 131 | Distinguish Content Delivered from Content Displayed and do not infer reading or understanding | Core event-recording rule; understanding requires a separate check |
| 132 | Record no display, partial display, or complete solution display distinctly | Core exposure rule; complete solution is treated as exposed regardless of whether reading/understanding can be proven |
| 133 | Count exposure only when content becomes visible in the active DEIXEN interface | Core software event rule; loading/background storage/closed panels do not count; no external browser/device monitoring |
| 134 | Classify review/explanation fragments as General Feedback, Sensitive Detail, or Protected Solution | Core content metadata; link each fragment to case/version, skill/step, and mode rules |
| 135 | Apply mode-specific display rules to the three content classes | Core deterministic visibility rules across Practice, Scenario, and Independent Assessment |
| 136 | Map every sensitive fragment to affected skills, steps, and assessment criteria | Core structured-data rule; missing or ambiguous mappings trigger a learner-specific hold rather than guessing |
| 137 | Limit exposure impact to affected skills when evidence is separable; invalidate the whole assessment only when core validity is compromised | Core fairness rule; never change criteria mid-attempt |
| 138 | Separate overall assessment validity from skill-level evidence eligibility/results | Core evidence model; preserve unaffected evidence and separately mark skills excluded from independent evidence due to exposure |
| 139 | Show Valid, Limited, and Invalid for Independent Assessment outcomes clearly, preserving valid unaffected skill evidence | Core learner-facing result behavior; no competence penalty for a validity problem and no protected-solution disclosure |
| 140 | Allow the learner to submit a simple Report Result Issue linked to the original attempt/result | Core product function; submission does not automatically alter the result or create a general complaints system |
| 141 | Show deterministic report states: Received, System Check in Progress, Result Corrected, No Change, Unable to Verify Automatically | Core status feedback; no implied human review and no interruption to Learning/Practice |
| 142 | Recheck reported issues using original attempt data, original case/variant version, and original assessment rule version | Core reproducibility rule; never substitute newer rules when reproducing the original result and never guess when data is insufficient |
| 143 | Preserve immutable assessment rule versions and create corrected-result records under a new rule version when a software defect is confirmed | Core evidence integrity and reproducibility; recheck only explicitly affected attempts and preserve the original outcome and history |
| 144 | Make the corrected result the current accepted result for the same Attempt while preserving the original as linked, superseded history | Core evidence-integrity rule; Growth uses the corrected result once and a correction does not create a new performance attempt |
| 145 | Recalculate only dependent Growth, recommendation, and future eligibility/access outputs after a correction | Core propagation rule; preserve unrelated attempts/evidence and explain material progress changes to the learner |
| 146 | Supersede recommendations that no longer fit the corrected evidence and retain their historical basis | Core recommendation lifecycle; create a new recommendation only when supported by the corrected result and current evidence |
| 147 | Recalculate eligibility for activities not yet started, while preserving the conditions and rule version of attempts already in progress | Core temporal-integrity rule; do not interrupt or retroactively alter a running attempt solely because a prerequisite was corrected |
| 148 | Do not automatically invalidate a completed attempt when an earlier eligibility prerequisite is corrected | Core evidence-validity rule; keep the completed attempt when its own performance and assessment basis are unaffected, and correct it only if its own assessment was defective |
| 149 | Recalculate competency from all relevant valid evidence, replacing the old result with its correction for the same Attempt | Core Growth/evidence rule; do not double-count the corrected Attempt or discard other valid evidence |
| 150 | Opening or previewing a scenario does not start an Attempt; eligibility is rechecked at the actual start boundary and the Attempt is bound to the applicable eligibility/rule/version snapshot | **NOW:** implement preview → mode-specific start request → eligibility recheck → Attempt-created states in the local Engine. The successfully stored Attempt, not the click alone, freezes the starting conditions |
| 151 | Do not execute attempt-governed operations until the Attempt record is successfully created; failed or uncertain creation must not consume an attempt, and an existing record must be recovered | **NOW:** test safe create/fail/unknown/recover behavior locally. **LATER:** guarantee durable storage and cross-session recovery through Backend before production |
| 152 | Treat repeated submissions of the same start action as one start request; prevent duplicate Attempt creation and recover the same Attempt where it already exists | **NOW:** implement client/local idempotency and duplicate-click protection in the prototype. **LATER:** enforce server-side idempotency, uniqueness, and transaction safety for simultaneous requests across clients/devices |
| 153 | Resolve a corrected-eligibility update and an Attempt start request at one recorded start boundary | **NOW:** test both event orderings and uncertain creation in the local Engine. **LATER:** enforce cross-client ordering and transaction safety through Backend |
| 154 | If eligibility is lost after a case is opened but before it is started, refresh the case state and block start without consuming an Attempt | **NOW:** test refreshed UI state, safe explanations, and neutral uncertainty handling. **LATER:** synchronize eligibility and prevent stale-client starts across devices |
| 155 | If eligibility is restored before start, make the case available again without auto-starting; require a fresh explicit start and eligibility check | **NOW:** test available → unavailable → available transitions without creating an Attempt. **LATER:** synchronize refreshed eligibility across sessions/devices |


---

# 9. Open design questions — Frontend/Engine first, Backend design later

Only the unresolved design questions below should drive near-term Frontend/Engine design and validation. Backend questions are explicitly grouped for later design after the core behavior is validated. Other older open issues should be revisited only when they become relevant to the selected product slice.

## 9.1 Operational scope and truth

- What exact first task and command scope are currently supported by the training engine and repository?
- Which authoritative operational references support each taught command, response, and state transition?
- What is explicitly out of scope for the first case?
- Which structured operational facts, expected states, and boundaries must be present before the first case can be activated?

## 9.2 Learning and assistance

- What are the specific learning objectives for the selected first task?
- Which understanding checks demonstrate interpretation rather than memorization?
- Which assistance types are allowed in each of the three Terminal modes?
- What exact intervention changes the independence status of an action or attempt?

## 9.3 Terminal and case workflow

- What is the minimum Terminal hierarchy and task-context presentation that keeps operational work central?
- How will the first Case Package and controlled customer facts be represented and versioned?
- How will the system validate the actual operational state against the latest customer-confirmed and authorized request?
- How will the learner confirm the request and obtain authorization, and how will a change before, during, or after reservation creation be represented without merging conversation, task, and operational state?
- How will task submission, correction, escalation, incomplete outcomes, and a valid no-reservation outcome behave in each mode?
- Which professional task outcomes are acceptable in the first Case Package, including customer withdrawal or justified escalation?

## 9.4 Assessment and evidence

- What are the observable criteria and critical failure conditions for the first task?
- What evidence is sufficient for step, task, and transfer conclusions?
- How are assisted, independent, incomplete, and invalid attempts represented?
- How is a debrief kept separate from operational output and protected assessment feedback?
- What are the observable Performance Outcome criteria for the reservation path and for valid no-reservation paths?
- How are Demonstrated, Not Demonstrated, and Not Assessed assigned fairly for each skill and case path?
- What simple rules should select a targeted next activity without duplicating learning or exposing protected assessment criteria?
- What resources are permitted in the first independent reservation assessment, and which can be made available inside DEIXEN?
- What exact assistance exposure changes an attempt from independent to assisted/contaminated, especially when help is accidentally delivered?
- What minimum briefing information and start confirmation are required before an Attempt is created?
- What post-assessment review fields help the learner understand performance without revealing protected answers?
- How should learner-specific exposure to complete variant solutions be recorded and checked before reassessment?
- What explicit software state retires a variant from protected use, and what required metadata/validation state must be present before a replacement becomes available?
- What is the smallest reliable exposure record for each learner/variant, and what delivered content counts as partial or complete solution disclosure?
- What exact deterministic rule keeps a variant on hold when disclosure impact cannot be classified, and what concise learner-facing notice explains the temporary unavailability?
- What minimum fields should Report Result Issue capture, and which result/attempt/rule-version records must it reference?
- Which deterministic checks are run for each report type, and what exact conditions produce No Change versus Unable to Verify Automatically?
- How are assessment rule versions stored and referenced so the original result can be reproduced exactly?
- How does a corrected rule version declare the attempts and criteria it affects, and what deterministic conditions trigger re-evaluation?
- How is a corrected result displayed and linked to the original without overwriting prior evidence?
- What explicit dependency links or recalculation triggers are needed in the implementation so corrected results update only the affected Growth, recommendations, and future eligibility views while leaving unrelated records and already-started attempts unchanged?

## 9.5 Growth, local reliability, and future Backend requirements

**OPEN for current Frontend/Engine work:**
- What is the simplest useful learner-facing evidence view for the first task?
- What local data must survive pause, resume, reload, and ordinary interruption during prototype testing?
- What minimal state/version mechanism should order a corrected-result eligibility update against Attempt creation inside one local Engine instance, without prematurely building distributed concurrency infrastructure?
- What exact Scenario Bank refresh behavior and safe learner-facing wording should be used when an already-open case becomes unavailable or available again before start?
- What exact visual explanation should accompany a corrected result, superseded recommendation, and recalculated skill position?
- Which accessibility, Arabic/RTL, and usability requirements must be tested in the selected Frontend slice?

**Retain for later Backend design, do not implement now:**
- Which records must be durably stored server-side, and what backup/restore and retention behavior is required?
- What authentication and authorization model is appropriate for real multi-user use?
- How will server-side ownership, least privilege, audit logging, and protected evidence storage be enforced?
- What transaction/idempotency mechanism guarantees one Attempt when clients submit the same start request concurrently?
- What is the safe migration policy from local prototype/test data to production data?

Human trainer access, trainer notes, and trainer-response workflows are outside the current scope; do not treat them as open implementation tasks for this phase.

Do not design an elaborate system to answer questions that are not necessary for the validated Frontend/Engine workflow.

---

# 10. Validation checks — prototype first, production Backend later

The Frontend and Engine must pass the relevant local/prototype checks before Backend integration is designed. A polished interface or a successful scripted happy path is not enough. The following checks 1–32 should be exercised in the deterministic local/single-user environment where possible; they do not prove production durability, multi-user security, or cross-device guarantees.

1. **Beginner usability:** Can a genuine beginner understand the task, learn the relevant concepts, and find the next action without hidden assumptions?
2. **Professional validity:** Are the task, customer dialogue, decisions, outputs, and criteria grounded in verified travel-operations requirements and explicitly defined expected outcomes?
3. **Operational truth:** Does every taught and assessed operation match verified training-engine behavior? Are unsupported cases and unknown behavior explicitly marked?
4. **Task correctness:** Can the system detect an operationally accepted result that nevertheless fails the customer's confirmed request?
5. **Assistance integrity:** Can the system reliably distinguish help requested, help delivered, help denied, and work performed independently?
6. **Assessment integrity:** Can it keep hidden facts and protected answers from leaking and avoid awarding independent evidence when integrity cannot be verified?
7. **Recovery and changed requests:** Do interruptions, uncertain command outcomes, and customer-request changes preserve history and avoid blind re-execution or continuing against an obsolete request?
8. **Evidence trustworthiness:** Do the structured records preserve enough information to reconstruct what the learner did, what the engine returned, what help was received, and why the Engine assigned the outcome?
9. **Fairness and accessibility:** Are text alternatives, clear language, usable controls, and reasonable language/accent fairness in place for the included interaction modes?
10. **Claim integrity:** Do all public claims match the actual scope and evidence, without promising employment, certification, employer acceptance, or full job readiness beyond what was demonstrated?
11. **Valid no-reservation path:** Can a learner correctly respect customer withdrawal or escalate a case, and can the product record a professionally correct outcome without a PNR?
12. **Fair skill opportunity:** Does the system distinguish Not Assessed from Not Demonstrated and offer a relevant next opportunity without forcing an unnecessary full replay?
13. **Assessment variant validity:** Does each activated variant contain complete, versioned operational facts, target skills, assessment criteria, difficulty attributes, sensitivity mappings, and a valid activation state, with no missing rule that would make the variant ambiguous or unfair?
14. **Fair reassessment:** After an unsuccessful attempt, does the learner receive useful development guidance and a genuinely suitable later opportunity without answer leakage, retroactive editing, or fixed attempt penalties?
15. **Assessment entry and consent:** Does the learner understand the rules before starting, deliberately initiate the attempt, and retain eligibility fairly when they postpone it?
16. **Assistance and resource integrity:** Can the product distinguish operational outputs, ordinary UI functions, denied help requests, delivered instructional help, and assessment-specific external reference use without claiming unimplemented monitoring?
17. **Feedback integrity:** Does the learner receive a useful review after the result is secured without exposure of protected answers or solution sequences?
18. **Variant exposure and availability:** Does DEIXEN avoid reusing a fully exposed assessment variant with the same learner and provide a fair alternative or defer assessment when no suitable variant is available?
19. **Disclosure classification and learner-specific holds:** Does the software distinguish delivered from displayed content, record partial/full exposure, map exposed fragments to affected skills, apply deterministic validity states, and hold only the affected learner/variant when rules are insufficient?
20. **Result issue reporting:** Can a learner report a possible result error, see a truthful deterministic status, and continue Learning/Practice without the report silently changing the result?
21. **Reproducible assessment decisions:** Can DEIXEN reproduce a finalized result using the exact original case/variant and assessment rule versions?
22. **Safe rule correction:** When an assessment rule defect is corrected, does the system create a new version, identify only the affected attempts, create linked corrected-result records where appropriate, and preserve all original rules/results/history?
23. **Corrected-result identity:** Does the corrected result become the current result for the same Attempt, remain linked to the preserved superseded result, and enter Growth only once without being counted as a new performance attempt?
24. **Dependency propagation:** Does a correction update only dependent skill positions, recommendations, and future eligibility/access outputs, supersede stale recommendations without deleting them, and explain material progress changes to the learner?
25. **Attempt time boundaries:** Are unstarted activities rechecked, in-progress attempts protected under their starting eligibility/rule version, and completed attempts retained unless their own performance or assessment basis was affected?
26. **Evidence-set recalculation:** Is current competency recalculated from all relevant valid evidence, using the corrected result instead of its superseded original while retaining other valid attempts and avoiding double-counting?
27. **Attempt start boundary:** Does previewing/opening a case leave it unstarted; does the actual start flow recheck current eligibility and bind the created Attempt to the exact case, variant, eligibility snapshot, and rule versions?
28. **Safe attempt creation:** Does the Engine block all operational commands until one Attempt record has been successfully created; do failed or uncertain creation states avoid consuming an attempt or creating an unverified second record?
29. **Duplicate start protection:** Do repeated clicks/resubmissions for the same start action resolve to one Attempt, with the existing Attempt recovered where appropriate, rather than creating duplicates?
30. **Correction/start ordering:** When an eligibility-changing correction and a start request occur close together, does the Engine apply a consistent order so the Attempt uses the eligibility state applied before its successful creation boundary, without silently rewriting an already-created Attempt?
31. **Eligibility loss while a case is open:** If eligibility changes after preview but before start, does the open case view refresh, block start, create no Attempt, and explain the change only to the extent that the reason is safe and known?
32. **Eligibility restoration before start:** If eligibility is restored while the case is still unstarted, does the case become available again without auto-starting or consuming an Attempt, and does a fresh explicit start recheck current eligibility?

## 10.1 Later Backend/production checks — not current build tasks

Before a real production launch to external learners, separately verify:

- server-side durable storage and recovery of all required records;
- authentication, authorization, ownership, least-privilege access, and secure handling of learner data;
- server-side transaction/uniqueness/idempotency guarantees for simultaneous requests across clients/devices;
- protection against client-side tampering with assessment results, evidence, rule versions, and exposure records;
- backup/restore, monitoring, security logging, and operational incident/recovery procedures;
- safe data migration or explicit exclusion of local prototype data.

Local Frontend tests for Stages 150–155 do not prove these Backend guarantees. They validate the user flow and Engine behavior only. Do not start this Backend checklist during the current Frontend/Engine phase unless needed to record a design constraint.


The founder can be an early pilot learner, but one person's experience is not sufficient proof that the product works for all beginners or target markets.

---

# 11. Scope exclusions and safeguards

The following must not be inferred from this register:

- that any feature listed here has already been implemented;
- that a complete institutional administration or HR product is approved or included in future Backend scope;
- that DEIXEN has an Amadeus partnership or live system connection;
- that a successful individual task proves full workplace readiness or guarantees employment;
- that a visual reference or future World direction is an approved design;
- that every proposal provisionally retained in this draft must be implemented in the current Frontend/Engine phase;
- that local persistence provides production durability, multi-user safety, or tamper resistance;
- that Backend implementation must begin before the Frontend/Engine is validated;
- that deferred World/LLM capabilities or human/institutional workflows are required before the core product can progress.

The software should enforce clear, repeatable product rules where appropriate. Human professional judgments, institution-specific policies, legal obligations, employment decisions, external reviewer contracts, and disciplinary procedures must not be disguised as automatic product logic.

---

# 12. Continuity and proposal-management rules

When continuing the DEIXEN UX/workflow proposal work:

- Work on one meaningful product proposal at a time.
- Explain the actual user/product problem before proposing a feature.
- Distinguish **PROVISIONAL — accepted for review**, **NOW — Frontend/Engine priority**, **LATER — Backend**, **FUTURE — World/LLM/Expansion**, **OUT OF CURRENT SCOPE**, and **OPEN**. These implementation labels do not turn a proposal into a final product decision.
- A stage-level owner approval is provisional acceptance of the proposal wording for this review draft only; it does not finalize a feature, complex workflow, UI design, data schema, or implementation.
- Prefer the smallest software capability that protects the core learning, task, assessment, evidence, and privacy goals.
- Challenge additions that expand DEIXEN into generic LMS, HR, enterprise administration, investigation management, or an open-world game.
- Do not allow Backend implementation, future World/LLM, voice, multi-GDS, trainer administration, or institutional workflows to delay the current Frontend/Engine vertical slice. Backend remains required before a real production launch to external learners, but its timing follows successful Frontend/Engine validation and the owner's decision to move into that phase.
- Do not invent Amadeus commands, responses, system behavior, or operational support. Verify uncertain behavior or keep it out of scope.
- Preserve original learner evidence; corrections and later reviews are additive and traceable.
- Keep learner evidence private by default and limit access to an explicit, relevant purpose.
- Update this register when the owner asks or when a meaningful cluster of decisions warrants synchronization; do not issue a new version after every small stage.
- Do not claim implementation, repository status, Backend readiness, or production launch readiness without current evidence.
- For every new proposal provisionally retained in the draft, identify what can be built/tested now in Frontend/Engine and what guarantee or service must wait for Backend.
- Do not downgrade or delete a useful proposal solely because it needs Backend; record its production infrastructure requirement and defer its implementation explicitly.
- Do not introduce human/trainer/institutional workflows as Backend requirements unless the owner separately reopens that product scope.

# 13. Review status, source package, and handoff route

## 13.1 Status of this proposal set

- The proposal round is closed at **Stage 155** for this iteration. No Stage 156 is being opened before review.
- Stages 1–155 remain a working proposal set. Stage-level owner agreement means provisional inclusion in this draft only.
- No proposal becomes a final product decision, approved specification, or build authorization solely because it appears here or received a stage-level “موافق”.
- The next step is a challenge-oriented review of all three documents together. Findings may cause proposals to be revised, merged, rejected, deferred, or retained as written.

## 13.2 Three-document review package

1. `DEIXEN_Objectives_and_Founder_Goals_Reference_v0.2.md` — objectives, founder goals, long-term ambitions, and preferred way of building DEIXEN. Its own status is a consolidated working reference, not final approved strategy or implementation specification.
2. `DEIXEN_Product_Feature_Ideas_Inventory_v0.2.md` — product pages, feature ideas, UX/workflow themes, World/AI hypotheses, and prior observed product reality. Its own status is a discussion-derived inventory, not an approved product specification or a verified current repository inventory.
3. `DEIXEN_UX_Workflow_Proposal_Register_v2.4.md` — this more detailed proposal set for product UX/workflow, current Frontend/Engine priority, deferred Backend requirements, future expansions, and out-of-scope boundaries.

The register elaborates selected themes from the two companion references. It must not be assumed to supersede them or to have captured every idea. Reviewers should explicitly identify where the three documents align, conflict, leave gaps, or use different maturity/status language. In particular:

- Distinguish a feature's **strategic/product importance** in the Feature Ideas Inventory from the owner's **current implementation sequence** (Frontend/Engine now, Backend later, World/LLM future).
- Distinguish long-term business/institutional ambitions in the Objectives reference from the scope of the current software product.
- The Feature Ideas Inventory §11 contains an earlier tentative model-allocation hypothesis (including Fable as a possible 3D/scene specialist and Opus as a possible software-architecture specialist). The owner's later role instruction recorded here supersedes that tentative split for the present project plan: Fable 5.2 is final reviewer/project lead; Opus 5.5, Sonnet 5.5, and Haiku 5.5 are the implementation models directed by Fable.
- The register does not cover every inventory idea (for example, visual identity, Coach avatar presentation, and the speed/time-to-correct-work concept may require their own decision work). Reviewers should identify what is intentionally outside this workflow register and what has been omitted unintentionally.

The two companion references are included unchanged in the review package; this revision does not silently rewrite their history.

## 13.3 Review responsibilities and sequence

**Current collaboration:** the owner is currently working with ChatGPT and Claude Sonnet 5.5.

**Second review — Claude Sonnet 5.5:** perform an independent challenge-oriented review of all three files. Do not treat the owner's provisional stage acceptances as final authority over product correctness. Test the reasoning, challenge unnecessary complexity, identify missing workflows, contradictions, unsupported assumptions, unclear status labels, premature Backend abstractions, and scope creep. Separate findings by severity and recommend retain / revise / merge / reject / defer.

**Final review and project leadership — Claude Fable 5.2:** receive the package and Sonnet's findings, conduct the final review, set the resulting project direction, and lead the project handoff into implementation. Under the owner's planned model allocation, Fable directs Claude Opus 5.5, Sonnet 5.5, and Haiku 5.5 as the implementation models. This document records the owner's planned role allocation; it does not assert that Fable's final review or implementation has occurred.

**Implementation gate:** no item in this proposal set should be treated as finally approved for implementation until the owner accepts the resulting review direction and the final project lead resolves the findings. The owner's immediate sequence remains Frontend + deterministic Engine first; Backend later; World/LLM future.

## 13.4 Questions every reviewer must answer

- Which proposals are correct, useful, and necessary for the core product—and what evidence or reasoning supports that view?
- Which proposals are unnecessarily complex, duplicative, or trying to solve future infrastructure problems during the Frontend/Engine phase?
- Are there contradictions between the three documents, within the register, or between the proposed user experience and the current deterministic-engine constraint?
- Are any rules impossible to implement/test without undefined facts, hidden human decisions, unsupported external system behavior, or LLM inference?
- Are NOW, LATER, FUTURE, and OUT OF CURRENT SCOPE classifications applied consistently to every relevant capability?
- What essential user journeys, error paths, or state transitions are missing? Which apparent gaps are intentionally deferred?
- Which proposals need more evidence from the repository, training engine, Amadeus references, target learners, or practitioners before they can be finalized?
- What is the smallest coherent core product and vertical slice that should be built first?
- Which proposals should be rejected rather than merely moved to a later phase?

**End of working proposal register — v2.4.** Stages 153–155 have been added. The proposal round is closed for this iteration at Stage 155. The entire stage set remains provisional and awaits Claude Sonnet 5.5's second review and Claude Fable 5.2's final review/project leadership. The current development sequence is Frontend and deterministic Program Engine first; Backend implementation later but not cancelled; DEIXEN World/LLM as future expansion; human/trainer/institutional workflows outside the current software scope. Local prototype tests do not establish production durability, cross-device concurrency, account security, or repository implementation status.
