# DEIXEN — Product, Pages & Feature Ideas Inventory

**Version:** 0.2  
**Prepared:** 15 November 2026

**Update:** Added the end-to-end UX/workflow architecture workstream, the Founder-Learner Pilot, and clarified that the existing learning sequence is not yet a complete UX workflow.  
**Purpose:** Consolidate the product ideas, feature directions, page responsibilities, and open questions discussed so far. This is a discussion-derived inventory, not an approved product specification or a verified repository inventory.

---

## 0. How to read this document

This inventory deliberately distinguishes four states. Version 0.2 adds a dedicated UX/workflow inventory and the founder-as-first-learner validation route; it does not convert proposed concepts into implemented features or final technical decisions.

- **Established direction:** A product principle or structural decision already established in the project context.
- **Owner-supported direction:** An idea the owner has explicitly agreed should be prioritized or carried forward, but which may still need detailed design and validation.
- **Proposal / hypothesis:** An idea discussed as a possible design or architecture. It is not yet an approved implementation requirement.
- **Implemented / observed in a prior snapshot:** Something previously observed in an application or repository snapshot. It does not guarantee that the latest repository still contains it or that it is production-ready.

The list captures what has surfaced in the conversations and handoff context. It does **not** claim that every historical repository document or every past conversation has been re-audited in this session.

## 1. DEIXEN's central purpose and product identity

### 1.1 Core purpose

DEIXEN's central purpose is to develop **real professional capability** and reduce the gap between someone who completes a course and someone who must perform actual work inside a travel company.

The intended learner journey is from knowledge to progressively independent performance—not simply command memorization or course completion.

The product should help a learner:

1. Understand a customer's request and discover missing information.
2. Ask suitable questions and clarify requirements.
3. Advise, make decisions, and confirm the intended action.
4. Execute the operational work in the GDS environment.
5. Verify that the result actually satisfies the customer's task—not merely that the system accepted the commands.
6. Recover from errors, handle changes, or escalate appropriately.
7. Communicate, close, and follow up professionally.

### 1.2 Product category / positioning hypothesis

A useful working description is:

**Professional Work Competence & Training System for Travel Operations.**

DEIXEN should not be reduced to an LMS, a GDS command simulator, an AI roleplay tool, or a 3D game. Its potential differentiation is the integration of customer interaction, professional judgement, operational execution, task correctness, recovery, and credible evidence of independent performance.

### 1.3 Four types of correctness that must remain distinct

- **Input / syntax correctness:** Were the commands and data entered correctly?
- **Operational correctness:** Did the GDS engine accept the action and produce the expected operational state?
- **Customer / task correctness:** Did the result actually fulfil the customer's request and constraints?
- **Professional / business correctness:** Was the decision, advice, communication, and handling appropriate?

Customer satisfaction is important, but it is not a substitute for task correctness or professional correctness. A system-accepted booking can still be wrong for the customer.

---

## 2. Top-level product structure

The established top-level structure is five areas:

1. **Home**
2. **Learning**
3. **Terminal**
4. **Scenario Bank**
5. **Growth**

**Ghost** and **Coach** are capabilities that work across the product; they are not separate top-level areas. **DEIXEN World** is a proposed immersive mode/experience associated with Scenario Bank, not a sixth top-level area.

### 2.1 Home

**Known direction:** Home is the current name; it supersedes the older “Flight Deck” label in the current product-area vocabulary.

**Role:** The entry point into the product and the place from which a learner understands where to continue.

**Ideas discussed or implied, but not fully specified yet:**

- Show the learner's current learning and practice journey.
- Make the next useful action understandable rather than presenting a generic SaaS dashboard.
- Connect progress across Learning, Terminal, Scenario Bank, and Growth.
- Surface relevant next steps without using unsupported readiness percentages or decorative gamification.

**Still open:** Exact Home layout, widgets, information hierarchy, and whether it is primarily a launchpad, progress overview, or contextual workspace. Do not invent a final Home specification from the name alone.

### 2.2 Learning

**Purpose:** Build knowledge and mental models before and alongside practical performance.

**Learning ideas discussed:**

- Beginner-friendly progression for someone with little or no operational GDS knowledge.
- An Amadeus learning track as the initial operational foundation.
- A Customer Service Track alongside the technical track, because professional work begins with understanding and serving the customer—not with typing commands.
- Lessons should prepare the learner for work tasks and later scenarios, rather than exist as disconnected theory.
- Connect learning topics to related scenarios; for example, a Customer Service concept should later appear in a customer-facing case.
- Use worked examples and demonstrations, prediction/retrieval prompts, guided practice, fading support, meaningful variation, spaced practice, delayed assessment, and transfer to unfamiliar situations where evidence supports their value.
- Make the learner understand why a step is taken and what state or consequence it creates—not merely memorize a sequence.
- Use professional situations and examples to teach both operational concepts and workplace communication.

**Language-learning direction:**

- English should be the primary language of the DEIXEN World experience.
- Teach English used in travel operations through realistic work, not only through separate vocabulary lessons.
- The learner should hear, read, and use customer-service and operational English inside tasks.
- Arabic support may be available as optional scaffolding, explanations, or translations; it should not automatically replace the English-first work environment.
- Language support should fade as the learner becomes more capable.

**Learning should not:**

- Treat course completion as proof of competence.
- Let a learner pass an independent assessment merely because they followed a demonstration.
- Use Ghost or Coach assistance as evidence of independent performance.
- Expand into advanced specializations before Priority 1 and Priority 2 have been successfully designed and validated.

**Prior implementation snapshot:** A beginner L01–L10 Learning sequence and bilingual lesson material were previously observed in the app context and associated with an accepted F-08/D96 record. This is a historical observation, not a fresh verification of the current repository.

**Still open:** Final curriculum map, exact Customer Service Track structure, learning outcomes, lesson-to-task traceability, language levels, and evidence-based instructional design validation.

### 2.3 Terminal

**Purpose:** The operational center where learners execute work in the GDS training environment.

**Established direction:**

- Scenario execution belongs inside Terminal as a mode; Scenario Bank is the case library/page, not a separate place where a parallel terminal exists.
- A case opened from Scenario Bank should launch Terminal in **Scenario Mode**, not send the learner into Learning Mode.
- Terminal must distinguish Practice, Scenario, and Independent Assessment modes where applicable.
- The learner should see genuine output from the training engine, not invented output presented as real Amadeus behavior.
- Any added training explanation should be clearly labelled as training content and must not be confused with operational GDS output.
- The current training engine must be described as a simulator, not a live Amadeus connection.

**Amadeus simulation slice previously described:**

- A narrow deterministic workflow covering commands around AN, SS, NM, AP, SRCTCM/CTC, TK, RF, ER, FXP, with FQD treated as optional in an earlier slice.
- One adult, one segment, one fare in the narrow initial workflow.
- The exact command naming/coverage varies between historical descriptions and must be checked against the current code and approved references before being treated as canonical.

**Terminal-related ideas:**

- Preserve a real command-line workflow and meaningful Amadeus-style output.
- Provide a clear distinction between command validity, system state, and whether the task is professionally correct.
- Support recovery and correction—not only happy-path success.
- Let task instructions and scenario context accompany the terminal without hiding the actual operational work.
- Capture a trace of actions, errors, corrections, and final state for later evidence.
- Avoid fabricating unsupported Amadeus behavior; mark unknown or unverified behavior explicitly.

**Prior implementation snapshot:** A deterministic command engine, practice/scenario/assessment modes, a rule-based Coach, Ghost demonstration using the engine, and a localStorage-based evidence mechanism were previously observed. The engine was narrow and not live Amadeus. Current status must be verified against the latest repository.

**Still open:** Exact command scope, broader operational coverage, source-of-truth rules for every command, how the engine will expand, backend transition from localStorage, and how task-level validation will relate to operational validation.

### 2.4 Scenario Bank

**Purpose:** A structured library of professional cases organized so learners can find and progressively unlock relevant work situations.

**Established direction:**

- Scenario Bank is the case library / case page.
- A learner selects a category or professional area, then a case.
- Opening a case should launch Terminal in Scenario Mode—not Learning Mode.
- The case should be connected to relevant Learning tracks and prerequisites.
- Scenario access may unlock gradually after relevant Amadeus and Customer Service learning/practice progress.
- Scenario execution should not be detached from the Terminal.

**Potential category/family organization discussed:**

- Customer Service: new customer requests, difficult customers, complaints, clarification, communication, follow-up.
- Reservations: new reservations, changes, booking errors, retrieval, customer-specific constraints.
- Further professional domains can be added based on validated job tasks rather than invented categories.

**Professional case structure:**

A scenario should include, as appropriate:

- Customer's stated request.
- Hidden facts, intent, preferences, and constraints.
- Facts that must be discovered through questions.
- Customer persona, communication style, and response rules.
- The professional task and permitted choices.
- Operational actions expected in the GDS.
- Task-level correctness criteria.
- Professional communication and service criteria.
- Known failure modes and recovery options.
- Assessment criteria and evidence requirements.
- Variants that test transfer rather than repeat a memorized answer.

**Examples discussed:**

- A technically accepted booking that is professionally wrong because the passenger name or customer requirement is mismatched (e.g. Ahmed/Ahmad).
- A customer request misunderstood even though commands were syntactically valid.
- Errors, warnings, changes, complaints, or difficult situations.
- Cases where the learner must identify missing facts rather than receive all details immediately.

**Case Package Definition — New Reservation (CP-001):**

- It was identified as a working candidate, not approved production case content.
- Practitioner review remains pending.
- Operational questions U-12 and U-14 were recorded as unresolved.
- Do not treat CP-001 as approved merely because it exists in the Knowledge files.

### 2.5 Growth

**Purpose:** Show development over time and preserve credible evidence of what the learner can demonstrate.

**Ideas discussed:**

- A learner evidence portfolio rather than a decorative points dashboard.
- Show which tasks or skills were demonstrated, under what conditions, and with what degree of independence.
- Preserve evidence of assistance, errors, correction, recovery, transfer to a changed case, and performance under pressure where assessed.
- Make the difference between guided success and independent competence visible.
- Show growth areas and useful next practice steps.
- Support continued professional development after employment, with meaningful refreshers, new hard cases, changing operational knowledge, and role progression.
- Potential future Shift Evidence Records for work-shift assessments.

**Important constraints:**

- Avoid unsupported readiness percentages or a single numeric “job readiness” score.
- A completed course, lesson, simulation, or booking is not by itself proof of independent competence.
- Explain the conditions and limitations of each evidence item.

**Still open:** Exact portfolio layout, evidence presentation, learner sharing/export, employer view, trainer view, and the continuing-development offer.

---

## 3. Shared capabilities that work across pages

### 3.1 Ghost — Demonstration capability

**Purpose:** Let learners observe and inspect an operational demonstration.

**Ideas / direction:**

- Ghost demonstrates real workflows using the same training engine rather than showing unrelated scripted outputs.
- Demonstrations can be cumulative across connected workflows, helping the learner understand how steps connect.
- Ghost should explain rationale and resulting state, not only replay command syntax.
- Ghost is a learning aid, not evidence that the learner can perform independently.
- Ghost should not be available as assistance inside a protected independent assessment.

**Prior implementation snapshot:** A Ghost workflow using the actual narrow engine and a demonstration booking was previously observed. D97 describes a stricter cumulative demonstration/assessment boundary, but the claimed implementation status requires repository verification.

### 3.2 Coach — From tips assistant to professional supervisor

**Owner-supported priority:** The Coach should be treated as a meaningful professional development supervisor inside the virtual company—not merely a tool that waits for the learner to request a hint.

**Intended role:**

- Welcome and orient the trainee on their first day.
- Explain workplace responsibilities and the nature of the job.
- Brief the learner before a task without revealing the solution.
- Teach concepts and professional reasoning.
- Ask questions and guide thinking during practice.
- Observe performance and identify recurring errors.
- Review decisions and performance after a task.
- Recommend the next useful challenge.
- Gradually reduce assistance so the learner becomes more independent.

**Progressive assistance model discussed:**

1. High Guidance — explicit explanation and demonstrations for beginners.
2. Guided Independence — prompts and questions rather than step-by-step answers.
3. Reduced Assistance — intervene only when needed.
4. Independent Assessment — no prohibited Coach hints or rescue.

**Coach must remain separate from the customer.** The customer provides task information and behaves according to the case; the Coach provides learning support only in permitted modes.

**Coach's behavior should be context- and mode-aware.** The Coach should know whether the learner is learning, practicing, executing a scenario, or in protected assessment. Customer statements must never be confused with coaching hints.

**Prior implementation snapshot:** The Coach was previously described as rule-based, not powered by a live LLM runtime. More advanced dialogue/voice behavior is a future direction, not established current capability.

### 3.3 Coach visual identity / avatar

**Direction:** Non-human Coach / mascot, connected to the DEIXEN brand mark rather than a generic human instructor.

**Exploratory ideas previously discussed:**

- A robot-like or desktop-monitor-like head.
- `</>` as a possible eye/content cue, or a double-eye variant.
- A simple line as a mouth.
- A stand/collar or other shape that suggests a professional role.
- A robot/avatar reading is not automatically a problem; it could be a positive signal of simulation and virtual-company identity.

These are exploration ideas, not an approved final avatar or logo.

### 3.4 English learning and language support

**Owner-supported direction:** The DEIXEN World environment should be English-first because English is central to travel operations and the user wants learners to improve job-related English through work situations.

**Ideas:**

- Coach and customer dialogue primarily in English.
- Workplace signs, task briefings, common phrases, and professional communication in English.
- Natural exposure to travel terminology and service language.
- Captions/subtitles, replay, and potentially adjustable speech speed.
- Optional Arabic explanation or translation as scaffolding, not as the default replacement for English.
- Gradual reduction of language support as ability grows.
- Evaluate whether the learner communicates clearly and effectively, not whether they imitate a native accent.
- Voice input should have a text fallback; accent and speech-recognition fairness must be considered.

**Open voice options:**

- Clone the owner's voice for the Coach.
- Use a professionally selected English voice.
- Test a hybrid or adjusted version only if it remains natural and consistent.

The owner noted that his English accent is not strong and wants the virtual world in English. The voice choice is therefore a hypothesis to test—not a decision to clone his voice automatically. The target is clear, natural, understandable professional English, not an artificial requirement to sound American or British.

### 3.5 Evidence and assessment

**Core principle:** Correct final state is not enough; the system needs evidence of how the learner got there and how independently they acted.

Evidence should distinguish:

- Learner action versus Coach/Ghost assistance.
- Independent action versus guided action.
- Correctness of commands versus correctness of the customer's task.
- Errors, recovery, corrections, and escalation.
- Transfer to changed or unfamiliar situations.
- Performance under realistic pressure where appropriate.

**Independent assessment direction:**

- A fresh task instance or meaningful unseen variant.
- A new assessment session and clean booking context where required.
- No Ghost in the protected assessment session.
- No prohibited Coach assistance.
- Evidence for all required skills in the same assessment chain.
- Customer responses remain task data, not hints or coaching.
- Critical criteria should not be compensated by unrelated strengths.

**D97:** A decision record describes cumulative Ghost and independent assessment rules, including a fresh session, clean booking, no Ghost in the session, a distinct unpractised task instance, and independent evidence across required skills. Its implementation in the accessible app snapshot was not verified; do not claim implementation until checked.

**Future idea:** Shift Evidence Record for a complete work-shift simulation showing customer interactions, decisions, commands, errors/corrections, difficult situations, final task states, and independence.

### 3.6 Speed / time-to-correct-work concept

A concept was discussed for measuring time to produce a correct booking or task outcome:

- Distinguish thinking/decision time from typing/execution time where useful.
- Do not begin with a countdown timer that distorts learning.
- Consider later multi-task runs (for example, three tasks) once the core task model is validated.
- Speed must never compensate for incorrect or unsafe professional work.

This remains a validation idea, not a finalized scoring system.

---

## 4. DEIXEN World — immersive virtual company experience

### 4.1 What it is intended to be

DEIXEN World is a future immersive mode/experience within Scenario Bank. It is not the entire DEIXEN product and not a sixth top-level area.

The purpose is to make professional work feel situated and meaningful: the learner enters a virtual travel company, encounters customers and workplace situations, and performs real training tasks within that world.

### 4.2 Visual direction

The current visual exploration preference for the world is **Stylized Cinematic Low-Poly 3D Character Art**:

- Faceted geometry and expressive stylized faces.
- Chunky, stylized hair and clear character silhouettes.
- Soft cinematic lighting and readable environments.
- Professional but engaging virtual-company spaces.

This 3D world direction is separate from the still-open logo/brand identity. It does not authorize reviving rejected logo or design-system decisions.

### 4.3 The expanded cinematic idea — story-driven professional scenarios

The latest owner explanation expands the idea beyond simple camera transitions. The aim is to make Scenario Bank and the world enjoyable to watch and motivating to complete, with a storyline-like experience similar to a narrative game—but centered on learning a real profession.

**A possible learner flow:**

1. The learner selects a professional category in Scenario Bank.
2. The learner selects a case.
3. The case opens in Terminal Scenario Mode, not Learning Mode.
4. In DEIXEN World, a cinematic introduction begins before execution.
5. On the first visit, the Coach may welcome the learner, introduce the company, explain work challenges, and connect the experience to relevant Learning content such as Customer Service.
6. For each case, the Coach briefs the learner on the situation and professional responsibility without revealing the answer.
7. The camera may move to observe the customer from a distance, showing personality, behavior, emotion, urgency, and non-verbal cues.
8. The cinematic introduction ends and the learner takes control of the task.
9. The learner speaks with the customer and executes the work in Terminal Scenario Mode.
10. Meaningful story events may occur during the task if the task state warrants them.
11. After completion, a closing scene or Coach debrief may review the outcome and prepare the next learning step.

### 4.4 Two different cinematic systems

Do not conflate:

- **Cinematic transitions:** Short camera moves between customer, employee, workstation, and Terminal. An earlier proposed transition target was approximately 180–260 ms, but that was only a tentative idea and should be usability-tested.
- **Narrative / story cutscenes:** Longer animated scenes that introduce a task, explain a workplace situation, present an emergency, show customer behavior, or conclude an episode.

The second type may last several seconds or longer according to the story purpose. It is not bound by the transition timing idea.

### 4.5 Narrative possibilities

- First-day-at-work orientation.
- Coach briefings before cases.
- Customer introductions and observational scenes.
- Emergency or urgent events.
- Customer complaints and emotional situations.
- A manager or colleague handing over a task.
- Workplace interruptions or changing conditions.
- Consequences of an incorrect professional decision.
- Post-task review and debrief scenes.
- Environmental storytelling: a busy office, ringing phones, visible work queues, colleagues helping each other, and other contextual details.
- Dynamic scenes triggered by task state rather than always playing as fixed videos.

### 4.6 Story continuity and recurring characters

A further proposal is to make the virtual company feel like a continuing world:

- A recurring Coach who develops a relationship with the trainee.
- Colleagues and managers who appear in different situations.
- Returning customers who may appear in later cases.
- Independent episodes as well as connected story arcs.
- Later progression from individual cases to multiple customers and a complete work shift.

This should be used where it supports professional learning. Do not force every case into one long story if independent cases are more useful.

### 4.7 Scene controls and accessibility

Ideas to preserve:

- Allow the learner to skip a scene where appropriate.
- Allow replay of useful briefings or explanations.
- Captions/subtitles and text alternatives.
- Reduced Motion support.
- Ensure scenes do not become long repetitive barriers before the task.
- Avoid revealing hidden facts, expected answers, or assessment criteria that should be independently discovered.

### 4.8 Staged development hypothesis

A previously discussed gradual path:

1. One customer, one cinematic opening, and transition to Terminal.
2. Customer personality states, interruptions, and optional voice with text fallback.
3. Multiple customers, recurring characters, and connected workplace situations.
4. Full independent work-shift assessment and Shift Evidence Record.

This is a proposed progression, not an approved delivery roadmap.

---

## 5. Customer simulation and scenario intelligence

### 5.1 Deterministic-first customer simulation

A customer should not be a generic chatbot that invents facts. The simulation should be governed by the case definition:

- Known and hidden facts.
- Customer intention and preferences.
- Constraints and required information.
- Personality and communication style.
- Emotional state and permitted reactions.
- Dialogue branches and information-discovery rules.
- Conditions that trigger new information or changes.

### 5.2 Role of AI / language models

A model may help express the customer's language naturally, vary wording, or provide voice/personality. It must not become the authority for:

- Case facts.
- Passenger or booking data.
- Operational Amadeus behavior.
- Task success criteria.
- Hidden assessment answers.

The scenario engine and operational engine remain authoritative for their respective domains.

### 5.3 Customer vs Coach separation

- The customer communicates needs, facts, preferences, constraints, and reactions as defined by the scenario.
- The Coach teaches and guides only in permitted learning/practice modes.
- Customer responses are part of the task, not clues from the Coach.
- A customer may be dissatisfied even where the system accepted an action; this should be represented separately from professional correctness.

---

## 6. Task Runtime and supporting architecture ideas

### 6.1 What Task Runtime means

Task Runtime is a proposed behind-the-scenes coordinator for a running professional task. It is not a learner-facing page and not a replacement for the GDS engine.

Its potential responsibilities:

- Start and maintain the current task/session state.
- Coordinate the case facts and task requirements.
- Coordinate customer interaction and permitted dialogue state.
- Send operational work to the GDS training engine and receive its result.
- Inform the Coach which mode and support rules apply.
- Trigger narrative/cinematic events when appropriate.
- Coordinate task-level validation separately from operational acceptance.
- Record evidence and assessment events.
- Ensure the protected assessment rules are respected.

### 6.2 Separate sources of truth

A proposed architecture separates:

1. Case / scenario facts.
2. Customer simulation state.
3. Operational GDS engine state.
4. Coach behavior and permissions.
5. Narrative / cinematic presentation state.
6. Assessment and evidence state.

Task Runtime coordinates them; it must not invent their truths or become one unbounded “mega-engine.”

### 6.3 Learner visibility

The learner should not see or operate a feature labelled “Task Runtime.” The learner sees the task instructions, customer, terminal, Coach when permitted, scenes, and task results. Some task status or requirements may be shown, but hidden facts and assessment logic should remain protected.

### 6.4 Status

Task Runtime is an architectural concept discussed in the design conversations. A complete implementation has not been established. Stage 2 should test whether it should be a distinct module/service or whether these responsibilities belong to smaller coordinated components.

---

## 7. Virtual Company / work-shift assessment

A future expansion of Scenario Bank / DEIXEN World:

- One task first, followed by connected customer cases.
- Later, multiple customers or a work queue.
- Employee responsibilities and handoffs.
- Changing priorities and interruptions.
- Coach available in practice, but absent during protected independent shift assessment.
- A complete Shift Evidence Record.

The purpose is to assess customer handling, decisions, operational execution, recovery, communication, and independence across a connected shift—not merely one booking command sequence.

This is future scope. It should not delay the first validated professional task and core P1/P2 work.

---

## 8. Visual identity and design-system reset

### 8.1 Owner instruction

The following repository documents are being removed by the owner and their visual-identity direction is rejected:

- `04 Design System`
- `DEIXEN — Identity Closure`

All visual identity concepts, rules, or directions in those files must be treated as withdrawn / unapproved. They are not authoritative references for the new identity exploration.

The historical Stage 1 package and report must not be silently rewritten. Any record of their former presence or later withdrawal should be handled transparently, through a dated addendum or current-state record if needed.

### 8.2 New identity exploration

- No final logo is approved.
- The brand identity is open for fresh exploration based on the strategy and product reality.
- Do not treat the task as polishing or continuing the rejected identity.
- Avoid generic AI/template aesthetics, gradients/glow, obvious aviation clichés (aircraft, wings, boarding passes, radar, maps), generic IDE/code imagery, and empty abstract geometry.
- The user is open to a serious, modern advanced-software identity and potentially a dark visual direction.
- A non-human Coach avatar may become part of the brand expression, but should not dictate the logo prematurely.
- Earlier desktop-display/D-shape/`</>`/stand/collar ideas are hypotheses only, not binding requirements.
- AI-only exploration has been preferred; no human designer/executor is assumed.

**Important separation:** Rejecting old visual identity material does not automatically reject every non-visual UX or functional principle that might appear in those files. Those should be assessed independently.

---

## 9. Market, commercial, and institutional direction

These are strategic directions and hypotheses, not validated market conclusions.

- Intended audiences include learners, employees, and companies, with an ambition to serve broader international travel-operations markets.
- Saudi Arabia, Oman, and the UAE are important target markets; Egypt may provide an early pilot environment. The founder's personal job objectives should remain separate from DEIXEN's long-term market scope.
- Long-term ambition includes a specialized vocational training institution using DEIXEN's proprietary training environment, not only a subscription SaaS product.
- Potential relationships with Amadeus may be explored, but no partnership or affiliation should be claimed without approval.
- A free Explore experience and paid foundational access / continuing professional development have been discussed as pricing and packaging hypotheses.
- A continuing membership is only valuable if DEIXEN keeps delivering useful refreshers, updated practice, difficult cases, and professional development after employment.
- Employer-facing evidence and training-provider partnerships may help validate value before broad commercial scaling.
- AI roleplay alone is not a defensible differentiator; the potential distinction is linking realistic customer interaction to operational work, task-level correctness, and credible independence evidence.

---

## 10. Priorities and scope boundaries

### Priority 1 — core now

Entry-level job-entry competence: the basic professional tasks a beginner needs to perform credibly in a travel-operations role.

### Priority 2 — core now

Additional capabilities that help beginners perform more confidently and stand out professionally. P1 and P2 are both current core priorities and should be designed, built, and tested now.

### Priority 3 — future

Advanced specializations should remain future scope until P1 and P2 have succeeded in implementation and validation.

### Avoid premature expansion

- Do not build a large 3D world before proving the value of one vertical slice.
- Do not make voice mandatory; keep text fallback.
- Do not let an open-ended LLM control case facts or operational GDS truth.
- Do not expand to multiple GDS platforms before the first operational foundation is validated.
- Do not build a full subscription/institution infrastructure before willingness to pay and delivery viability are tested.
- Do not add numerical readiness scores or superficial gamification as a substitute for evidence.

---

## 11. What has been discussed about implementation tools

A preliminary division of work was discussed:

- **Fable 5.2** as a candidate for 3D environments, scene construction, motion, camera work, and cinematic prototypes.
- **Opus 5.5** as a candidate for software architecture, Task Runtime-related engineering, integration with Terminal, system logic, and tests.

This is a tool-allocation hypothesis, not a final production decision. The models should be compared on the same bounded vertical slice, including code quality, scene quality, editability, integration effort, performance, and total cost.

A reasonable prototype slice would be one office, one customer, one Coach briefing, one customer observation scene, one transition into Terminal Scenario Mode, one task, and one closing debrief.

---

## 12. Prior observed product reality — do not confuse it with the vision

Earlier read-only repository work described the app snapshot as a narrow deterministic Amadeus-style training simulator, not a live Amadeus system.

Previously observed elements included:

- React application structure.
- Beginner Learning content, including L01–L10.
- A narrow deterministic command engine.
- Terminal modes for practice, scenarios, and assessment.
- Ghost using the engine for demonstration.
- A rule-based Coach.
- Scenario Bank cases with execution in Terminal.
- Evidence/event recording and derived growth information.
- localStorage as a transitional persistence approach.

Previously unobserved in that app snapshot:

- A complete customer dialogue engine.
- A complete task-level semantic validator.
- A fully implemented Task Runtime as described here.
- DEIXEN World / 3D company environment.
- Cinematic narrative scene system.
- Voice roleplay / voice cloning.
- Full shift simulation.
- Payment/subscription infrastructure and institutional controls.

The exact current state must be verified against the latest repository and commit before planning implementation. The presence of a concept in Knowledge does not prove it exists in code.

---

## 13. End-to-end UX and workflow architecture — a required design workstream

### 13.1 Why this is now a major product concern

DEIXEN is becoming a product with multiple connected capabilities: Learning, Terminal modes, Scenario Bank, Ghost, Coach, Customer Simulation, Assessment, Evidence, and a future cinematic DEIXEN World. The product may be technically rich, but that richness must not become a burden the learner has to understand or coordinate.

The owner has explicitly raised UX and workflow as a major gap in the previous discussions. The current Learning → Demonstration / Ghost → Guided Practice → Independent Practice → Scenarios → Independent Assessment → Evidence → Growth sequence is a useful **pedagogical progression**, but it is not a complete end-to-end UX design. It does not yet specify all entry points, page transitions, task states, recovery routes, assistance rules, or user journeys.

A dedicated **End-to-End UX & Workflow Architecture Audit** must therefore be included in Stage 2 and carried into the Master Blueprint.

### 13.2 Core UX principle

**Complexity belongs in the system, not in the learner's experience.**

The product may contain complex operational, assessment, narrative, and evidence logic. The learner should experience a coherent journey with clear context, understandable choices, and a useful next step.

Design principles to evaluate:

- Progressive disclosure: show the learner the information and controls needed for the current stage, while keeping relevant navigation discoverable.
- Clear next action: help the learner understand what to do next and why it is appropriate.
- Context preservation: moving between a case, cinematic scene, customer interaction, and Terminal must not make the learner lose task context or entered work.
- Mode clarity: Practice, Scenario, and Independent Assessment must be visibly distinguishable, with their support rules made clear.
- Consistency: similar actions and states should behave consistently across pages and modes.
- Recovery: errors, interruptions, incomplete tasks, and returns should have understandable recovery paths.
- Accessibility: captions, text alternatives, replay, reduced motion, usable controls, and a text alternative to voice must be considered.
- Low unnecessary friction: remove avoidable navigation, duplicated instructions, and interruptions, without hiding information needed for sound decisions.
- Evidence-aware feedback: feedback should explain what happened and what the learner can improve, without reducing performance to a simplistic readiness number.

### 13.3 Four connected workflow maps are required

The audit should map these as separate but connected flows:

**A. Learner Journey**

From first entry and orientation through baseline understanding, relevant Learning tracks, demonstrations, guided practice, independent practice, scenario work, independent assessment, evidence review, and continued development.

**B. Professional Work Task Workflow**

Customer request → clarify / discover → advise / decide / confirm → perform GDS work → validate task correctness → recover / escalate where necessary → communicate → close / follow up.

**C. Learning and Assistance Workflow**

Determine what the learner needs → choose the right learning resource or demonstration → guided attempt → observe difficulty → offer proportionate support → fade assistance → verify independent transfer. The Coach and Ghost must respect the active mode and assessment restrictions.

**D. Scenario and Assessment Workflow**

Browse category → select case → confirm prerequisites / objective → enter the case → optional DEIXEN World narrative opening → customer observation / briefing → Terminal Scenario Mode → customer dialogue and operational execution → meaningful task events → validation → debrief when permitted → evidence → next practice or assessment step.

These workflows should not be designed as isolated mini-products. They must share the same task context and preserve the correct distinction between learning, execution, story presentation, and assessment.

### 13.4 Scenario Bank → DEIXEN World → Terminal flow

A specific owner-supported interaction direction must be preserved:

1. The learner organizes scenarios by professional area/category and selects a case.
2. Opening the case takes the learner into **Terminal Scenario Mode**, not Learning Mode.
3. When the immersive World is enabled, the case may first present a narrative/cinematic layer: first-day orientation, Coach briefing, workplace context, customer behavior, urgency, or relevant background.
4. The camera may observe the customer from a distance to communicate visible behavior and non-verbal cues. The scene must not reveal hidden facts the learner is meant to discover through questions.
5. When the scene ends, control passes to the learner for the actual task in Terminal Scenario Mode.
6. Further cinematic events may appear only when they meaningfully reflect the story or task state; they must not perform the learner's work.
7. The result may lead to a Coach debrief and Growth evidence, depending on the mode. In protected independent assessment, prohibited Coach guidance and answer-revealing scenes are not allowed.

The World is a presentation and interaction experience around the professional task; it must not create a parallel task workflow that contradicts Terminal Scenario Mode.

### 13.5 Non-linear learning loops and adaptive routes

The learner journey should not be a rigid one-way funnel. A learner may need to return to a relevant concept, repeat a guided exercise, attempt a different case variant, or proceed to a new challenge after demonstrating competence.

Potential routing logic to validate:

- A gap in customer discovery routes to the relevant Customer Service learning/practice, not automatically to a generic restart.
- An operational syntax error may route to the relevant command concept or Ghost demonstration.
- An accepted system state that is wrong for the customer should route to task reasoning and validation, not only command correction.
- Repeated dependence on help should lead to targeted practice before independent assessment.
- Demonstrated competence should allow progression without unnecessary repetition, subject to approved prerequisites.
- Different prior experience levels may justify a diagnostic entry route rather than forcing every learner through identical beginner content. This should not expand launch scope without evidence.

### 13.6 Exceptions and recovery flows that must be designed

The UX audit must cover more than the ideal happy path. Examples include:

- The learner does not understand a task instruction.
- The learner asks the customer an ineffective or ambiguous question.
- The learner enters an invalid command.
- The system accepts an action but the booking/task does not satisfy the customer request.
- The customer changes or clarifies the request mid-task.
- A task requires escalation or is outside the simulator's verified capability.
- The learner pauses, exits, loses connection, or resumes later.
- A scene is skipped, replayed, or unavailable.
- The learner needs Arabic clarification while the World remains English-first.
- Voice input fails or speech recognition misunderstands an accent; text must remain a viable fallback.
- The learner requests Coach/Ghost help in a mode where some or all help is restricted.
- A task ends incomplete or unsuccessful and must lead to useful recovery rather than a dead end.
- An assessment attempt must be protected from contamination by practice history, hints, or a rehearsed case variant.

### 13.7 UX and workflow validation criteria

Do not judge workflow quality only by clicks, speed, visual polish, or task completion. Evaluate whether learners can:

- Understand where they are and what mode they are in.
- Identify the next useful action without repeated external explanation.
- Move between customer interaction, World scenes, and Terminal without losing context.
- Understand what is expected without being given the answer.
- Recover from errors and resume work without unnecessary confusion.
- Use Coach and Ghost appropriately without becoming dependent on them.
- Distinguish operational output, narrative content, coaching, and assessment feedback.
- Complete the task with a manageable cognitive load.
- Transfer learning to a changed or unfamiliar case.

Usability, learning effectiveness, professional correctness, accessibility, and commercial appeal must be evaluated as separate dimensions. A workflow that is enjoyable is not automatically educationally effective; a workflow that is operationally correct is not automatically usable.

### 13.8 Required Stage 2 and Master Blueprint outputs

Stage 2 should provide evidence and recommendations—not implement or silently finalize the UX. Required outputs should include:

- Primary user roles and their goals for the current scope, with future employee / trainer / organization journeys kept separate.
- End-to-end learner journey maps.
- Page-to-page navigation and entry/exit maps.
- Professional task flow maps.
- Learning/assistance mode and Coach/Ghost permission maps.
- Scenario lifecycle and Terminal mode transition maps.
- Key task state transitions and interruption/recovery flows.
- A list of confusing, duplicated, missing, or premature UX steps.
- Proposed wireframe-level information hierarchy where evidence supports it.
- UX test questions, acceptance criteria, and a practical usability validation plan.

The final Master Blueprint should contain a coherent UX/workflow model before Opus implementation begins. Do not assume that existing pages or the historical workflow must be preserved unchanged.

### 13.9 Founder-Learner Pilot as an early UX and product validation route

The founder wants to become the first real learner using DEIXEN because the training-to-work gap is a personal, directly experienced problem. This creates an early pilot opportunity that should be connected to UX and workflow validation, not treated as a substitute for independent testing.

The pilot should document:

- A baseline of the founder's current GDS understanding and task ability before using the relevant product journey.
- The actual path taken through Home, Learning, Ghost, Coach, Terminal, Scenario Bank, and Growth as those capabilities become usable.
- Places where the founder hesitates, misunderstands, loses context, cannot find the next step, or needs external explanation.
- Whether instructions, customer interactions, English-language support, and cinematic briefings prepare the learner without revealing the solution.
- Where Coach or Ghost assistance is useful, excessive, unavailable, or accidentally creates dependency.
- Performance on independent and changed-case tasks after learning, including errors, correction, and transfer.
- Practitioner review of operational and professional performance; founder confidence or internal product feedback alone is not proof of competence.

Use the founder's experience to expose defects and improve the workflow, but do not design exclusively around one person's prior knowledge, preferences, language level, or habits. Follow with independent beginner usability and learning tests.

### 13.10 Current status

**Status: newly identified high-priority audit and design workstream.** The owner has agreed that UX/workflow must be developed alongside the rest of the product strategy. The existing high-level learning sequence and page structure are starting points only. No complete, validated end-to-end UX workflow has been established, and the requirements above are not proof of implementation.

---

## 14. Open decisions and questions to resolve

1. What is the final detailed purpose and information hierarchy of Home?
2. What is the complete P1/P2 professional competency map?
3. What is the approved Learning Track structure, including Customer Service and Amadeus?
4. What is the exact first end-to-end Professional Work Task, and what practitioner evidence validates it?
5. What is the canonical command/behavior scope of the initial GDS engine?
6. How will task-level validation detect accepted-but-wrong work?
7. What exact conditions define guided practice versus independent assessment?
8. What is the complete data structure for a Scenario Package?
9. How should Scenario Bank categories, cases, prerequisites, and variants be organized?
10. What story format should the World use: standalone episodes, recurring characters, arcs, or a mix?
11. How frequently should narrative scenes appear without interrupting practice?
12. What should the Coach say, know, observe, and be allowed to do in each mode?
13. How should the English learning path, Arabic support, subtitles, replay, and voice input work?
14. Should the Coach use the owner's cloned voice, a professional synthetic voice, or another approach?
15. What is the smallest valuable DEIXEN World vertical slice?
16. Should Task Runtime be one module or a set of smaller components?
17. How should cinematic scene triggers read task state without changing case truth or assessment outcomes?
18. How will customer facts and dialogue remain deterministic and testable while still sounding natural?
19. How will recurring characters and story continuity work without contaminating the independence of assessment variants?
20. What is the minimum useful Growth evidence portfolio and employer-facing evidence format?
21. What should be deferred until P1/P2 validation?
22. What belongs in the final canonical documentation architecture and Opus-ready specifications?
23. What is the complete end-to-end UX and workflow model across all five product areas?
24. What should the first-time learner journey and baseline/diagnostic route look like?
25. How should the product route learners between Learning, Ghost, guided practice, Scenario Bank, Terminal, assessment, and Growth without losing context?
26. What are the authoritative state transitions and recovery paths for pausing, resuming, failing, correcting, or escalating a task?
27. How should progressive disclosure and the next-best-action guidance work without hiding important navigation or creating dependence?
28. How should Scenario Bank, narrative scenes, customer observation, and Terminal Scenario Mode form one coherent workflow?
29. Which UX decisions should be consistent across practice and assessment, and which must deliberately differ?
30. How should the founder's own learning pilot and independent beginner usability tests be used without overfitting the product to one learner?

---

## 15. Recommended end-to-end learner experience (current synthesis)

1. **Home:** Understand where to continue and what useful next step is available.
2. **Learning:** Build the relevant technical and customer-service knowledge.
3. **Ghost:** Watch an operational demonstration and understand why each step occurs.
4. **Scenario Bank:** Select a professional case from an organized library.
5. **World introduction (future immersive mode):** Meet the Coach, understand the workplace context, and watch a cinematic case opening.
6. **Customer observation:** See the customer's behavior and situation without being given hidden answers.
7. **Terminal Scenario Mode:** Speak with the customer, discover facts, decide, execute, validate, recover, and communicate.
8. **Cinematic events (only when useful):** Present meaningful changes or developments without replacing the learner's decisions.
9. **Coach debrief:** Review the work and gradually reduce guidance across future tasks; no Coach help in protected independent assessment.
10. **Growth:** Preserve evidence of what the learner actually demonstrated and identify the next development step.

---

## 16. Current synthesis in one sentence

**DEIXEN should help learners live realistic, story-driven travel-operations work situations, learn the professional English and judgement required, execute the operational task themselves, and build credible evidence that they can perform increasingly complex work with decreasing assistance.**

This is the current direction emerging from the discussions—not yet the final approved Master Blueprint.
