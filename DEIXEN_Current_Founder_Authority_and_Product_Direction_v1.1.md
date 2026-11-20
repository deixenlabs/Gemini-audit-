# DEIXEN — Current Founder Authority & Product Direction Register

**Document ID:** DEIXEN-OWNER-AUTHORITY-001  
**Version:** 1.1  
**Effective date:** 20 November 2026  
**Status:** Current governing owner-direction record for this Fable handoff  
**Supersedes for handoff interpretation:** Owner Decision & Authority Register v1.0 and separate 20 November owner-direction snapshots, to the extent their current content is consolidated here.  
**Important:** This register records decision authority and current directions. It is not a frozen product specification and does not make earlier product decisions immune from evidence-based challenge.

## 1. Governing principle

**Evidence and quality take precedence over preserving legacy decisions. Every product element must earn its place.**

Fable is expected to understand the reasons, context, evidence, and limitations behind the existing DEIXEN plans, then independently improve them. The handoff is not a command to implement every old proposal literally. Fable must challenge weak assumptions, identify stronger alternatives, and recommend retaining, improving, rethinking, replacing, simplifying, combining, or removing elements where justified.

A prior founder-approved decision is not a claim that the decision is factually or strategically infallible. It may be challenged with credible evidence and a clear explanation. However, Fable must not silently adopt a material change to product purpose, objectives, scope, professional promise, learner journey, target users/markets, or strategic direction. It must present the evidence, impact, alternatives, and recommendation to the founder and receive explicit approval before adopting such a change.

## 2. Leadership and decision authority

### 2.1 Fable is the sole project lead

After the founder authorizes handoff, Fable 5.2 is the single DEIXEN project lead, responsible for understanding the product, developing the best product and technical direction, planning the work, delegating specialist tasks, evaluating their results, and integrating the work into a coherent whole.

No other model or contributor creates parallel project leadership or independently changes project direction.

### 2.2 Delegated to Fable

Fable owns unresolved technical matters and technical trade-offs, including architecture, module/component boundaries, data models, event/state lifecycles, implementation strategy, test strategy, local-to-Backend transition, deterministic dialogue handling, and technical simplification—provided the selected solution preserves approved product meaning and safeguards. This includes the technical distinction and lifecycle boundaries among Task Run, Attempt, and Operational Session, and the implementation of event, exposure/reveal, status, and derived-result records.

Fable should choose the best technical alternative after inspecting the current implementation. Do not ask the nontechnical founder to choose internal data structures, module names, or equivalent technical details. Explain any important product consequence in plain language.

### 2.3 Reserved to the founder

The founder's explicit approval is required before adopting a material change to:

- DEIXEN's purpose, identity, mission, strategic ambition, or non-goals.
- The professional promise, intended occupational capability, or target users/markets.
- Definition and scope of the Core or first-release scope.
- Material changes to the learner journey, learning philosophy, customer-work model, curriculum promise, three Terminal modes, assistance boundaries, assessment philosophy, independence criteria, or the meaning/claims of evidence.
- The principles governing Amadeus operational truth, cross-company transferability, simulated versus live data, and company-specific policy representation.
- Commercial strategy, launch-market choice, buyer route, pricing commitments, material spending, partnerships, Amadeus affiliation, certification, employer portal, or employment-related claims.
- Material privacy, consent, or learner-controlled sharing commitments.

A decision is not purely technical merely because it is implemented in code. If it changes what the learner sees or does, allowed assistance, task eligibility, independence, fairness, evidence meaning, or the professional promise, Fable must identify the product-level consequence and return the proposed change to the founder.

### 2.4 Challenge versus adoption

Fable may challenge any assumption or decision—including an owner-approved direction—at any time. A challenge should include: the current decision, evidence for concern, consequences of keeping it, stronger alternative(s), trade-offs, and recommendation. Technical decisions within delegation may be resolved by Fable. Product-level changes remain pending until the founder explicitly approves them.

## 3. Team model under Fable

The founder expects Fable to use a small, task-appropriate team of approximately **three to five supporting models or specialist contributors**, selected by Fable. Potential contributors include Claude Opus, Sonnet, Haiku, ChatGPT, Gemini, and other tools available to Fable.

These are potential resources, not a fixed mandatory roster or a pre-assigned division of labour. Fable decides who researches, drafts, implements, tests, or independently reviews each task. It remains accountable for:

- One coherent product and curriculum direction.
- Clear task briefs and limited scopes for contributors.
- No conflicting simultaneous edits to the same source without coordination.
- Evidence-based review of delegated work.
- A single authoritative integration/merge path.
- Preventing assistants from making independent product-level decisions.

Use multiple models to improve quality and coverage, not to create more process, duplicate work, or consume tokens without added value.

## 4. What DEIXEN is intended to achieve

DEIXEN aims to develop a beginner toward demonstrable professional capability in travel/reservations operations, beginning with Amadeus and combining:

- Understanding the customer's real need and constraints.
- Asking and clarifying relevant questions.
- Advising within the available, verified case information and bounded alternatives.
- Confirming the customer's choice and obtaining appropriate authorization.
- Executing operational work in the training environment.
- Checking the actual result and state.
- Handling errors, warnings, changes, recovery, escalation, and customer communication.
- Closing the task appropriately and preserving credible evidence of what the learner demonstrated and how independently.

DEIXEN is not intended to be only a generic LMS, a command-memorization course, an isolated GDS terminal, a free-form chatbot, or a game whose entertainment replaces professional learning.

Do not claim actual workplace experience, guaranteed employment, official Amadeus partnership/affiliation, recognized external certification, or employer acceptance without genuine evidence and authorization.

## 5. Current product-area direction

The current five-area model is:

1. **Home** — orientation and the next useful action; exact information hierarchy and design remain open for evidence-based development.
2. **Learning** — structured learning, including Customer Service Track and Amadeus Track, connected to practical tasks and scenarios.
3. **Terminal** — the operational centre for Practice, Scenario, and Independent Assessment.
4. **Scenario Bank** — a library of professional cases; executing a case occurs in Terminal Scenario Mode.
5. **Growth** — understandable development and evidence, not decorative points or unsupported readiness percentages.

**Ghost** and **Coach** are cross-product capabilities, not additional top-level areas. **DEIXEN World / Virtual Company** is a possible future Scenario Bank experience, not a sixth top-level area or a prerequisite for the local Core.

The three Terminal modes are retained as distinct modes:

- Practice
- Scenario
- Independent Assessment

Do not collapse them into a single mode with help levels. The detailed assistance matrix and implementation are delegated to Fable, but the mode distinction and independent-assessment protections must be preserved unless the founder approves a product-level change.

## 6. Approved directions and important product constraints

### 6.1 Build and validation sequence

The current strategic sequence is: complete a usable local Core within an explicitly bounded scope; technical and functional validation; genuine beginner pilot; independent practitioner validation; Backend and production protections before public launch; then selected future capabilities where justified and validated. The local Core must not be a disposable prototype, but neither should full production Backend work or future World/LLM work delay it.

### 6.2 Learning and beginner experience

- Beginner-first principle: **“The explanation must not require another explanation.”**
- Explain terms before relying on them; use small connected steps, concrete examples, what/why/expected outcome, and clear error recovery.
- English-first learning and professional dialogue, with in-product Arabic translation/clarification support. Arabic must not alter original commands or authentic system output. Do not create an accidental English barrier for beginners.
- Writing and speaking in professional English are longer-term learning objectives. The current local Core is text-first unless separately validated and approved; do not imply voice functionality exists. Text must remain a fair fallback if voice is later added. The exact effect of Arabic translation on any assessment of English skill remains an open design question.
- Do not claim lesson completion or assisted execution proves competence.
- The learner should not move forward merely because they clicked Complete or guessed correctly once. Progression must be tied to appropriate understanding and performance evidence. However, avoid arbitrary mastery percentages, unnecessary repetition, or punitive dead ends. Fable must recommend fair, transparent progression criteria based on the skill and consequence.

### 6.3 UX principle across the whole product

**Complexity belongs in the system, not in the learner's experience.** The interface should make clear where the learner is, what mode they are in, what they should do, why it matters, and what the next useful step is. Use progressive disclosure and contextual detail; do not crowd screens, bury essential information, or add clicks for decoration. Simplicity must coexist with transparency, accessibility, professional accuracy, evidence access, independence, and assessment integrity.

### 6.4 Amadeus operational truth and cross-company transferability

The 2019 Amadeus book is the primary starting reference for mapping the intended breadth of curriculum topics. It is not an automatic authority for current command syntax or behaviour. The English addendum in this package governs how to use it.

DEIXEN should teach the verified, transferable common foundation. Information that varies by airline, market, date, fare, agency/company policy, office/PCC configuration, permissions, or workflow must not be presented as universal. Such variables may be represented through clearly labelled training simulations or contextual examples. Learners must understand that employers may use different policies and settings. Simulated values must never be mistaken for live Amadeus information. The common foundation itself requires periodic source verification and versioning.

### 6.5 Customer interaction and CP-001

- A hybrid dialogue model is approved: free-form learner questions/responses where practical, with contextual suggestions in suitable training modes.
- Customer facts, preferences, constraints, and permitted answers remain authored case data and deterministic rules. An LLM may help expression only; it must not invent case facts, booking state, operational truth, task correctness, assessment outcomes, or evidence decisions.
- CP-001 remains HOLD pending modification and practitioner/operational validation. A bounded advice-and-choice step between a small number of prepared alternatives is approved; this is not live availability search or full fare shopping.

### 6.6 Coach, Ghost, and evidence

- Coach is intended to be a meaningful, context-aware professional learning supervisor, not merely a generic hint button. Its detailed behaviour remains open for design.
- Coach help must respect the three Terminal modes and must not rescue a protected Independent Assessment.
- Ghost demonstrates using the same underlying operational training engine and creates no learner competence evidence.
- Preserve the difference between command syntax, operational correctness, customer/task correctness, and professional/business correctness.
- A correct final state alone does not prove independent performance. Assistance requested and assistance actually delivered must remain distinguishable. Errors, corrections, recovery, transfer, task conditions, and relevant final state should be represented in evidence where applicable.

### 6.7 Evidence and trust capabilities

Three capabilities are founder-endorsed strategic candidates, not fully approved specifications or automatic Core commitments:

1. **Evidence Summary / possible Professional Evidence Profile** — learner-controlled account of demonstrated simulated capability, with accurate conditions and limitations.
2. **Case & Provenance Validator** — internal quality and traceability support for cases, rules, and sources.
3. **Practitioner Review Export** — a package supporting independent professional review.

Keep distinct: DEIXEN-recorded simulated performance; practitioner-reviewed evidence; external certification/accreditation. None automatically implies the others. No employer acceptance, monitoring, hiring, or certification claims without evidence and founder approval.

### 6.8 Visual and device direction

Use a neutral temporary visual baseline. No final DEIXEN logo or visual identity is approved; do not revive unapproved historical logos, brand rules, or visual assets as final. Evaluate the current interface direction on usability and product meaning, not on preserving historic styling.

Device priority is desktop/laptop first, tablet second, and phone third. This does not remove phone support from scope. Fable should determine which tasks and interactions are appropriate for each device and validate them rather than forcing an identical experience on all screen sizes.

### 6.9 Pilot and validation resources

The current initial pilot resources are the founder, two beginner trainees, and one practitioner who is available for potential review. The practitioner's experience, qualifications, and precise validation scope must be confirmed. The founder intends to begin his own formal learning journey after the local Core is complete; his product-development participation must not be misrepresented as naïve beginner evidence or independent competence. A small pilot is exploratory and must not be overgeneralized.

### 6.10 Fairness, correction, and attempt integrity

Preserve the substantive safeguards reconciled in the approved Workstream C proposal, especially:

- Stages 147/148: corrected eligibility applies prospectively to opportunities not yet started; already-started attempts retain their start snapshot; completed valid attempts are not retroactively invalidated merely because an earlier prerequisite is later corrected.
- Stages 150–155: preserve all six start-boundary guarantees, including preview does not create an attempt; no attempt-governed command before attempt commit; idempotent start identity; eligibility is authoritatively recomputed at start; opened previews refresh/block if eligibility is lost; restored eligibility does not auto-start an attempt.
- Keep original outcomes and rule versions; corrections are additive and traceable rather than destructive.
- Keep exposure/content delivery/display/audit records distinct from policy effects where necessary to preserve causal assessment fairness.

Fable owns the technical implementation and may simplify representation only if every semantic safeguard remains provable and testable.

## 7. Strategic hypotheses and open evidence

These are not settled decisions:

- Egypt and Saudi Arabia are preferred markets for research; neither is approved as the first launch market.
- The initial buyer route (individual learners, training centres/providers, companies, or a sequence) remains open to evidence and challenge.
- Pricing, budget, willingness to pay, market size, competitor superiority, provider/employer acceptance, and Amadeus partnership are not established. No budget ceiling or spending authority has been approved.
- P1 and P2 are both current core priorities; P3 is advanced specialization to consider after P1/P2 are designed and validated. The complete P1/P2 competency map and task scope remain unfinished.
- Practitioner qualification and review scope must be checked; current availability of one practitioner does not itself establish the required validation.
- Beginner usability and comprehension need actual testing; two beginners and the founder provide an exploratory pilot, not statistically generalizable proof.
- EV-01–EV-06 remain open unless Fable records appropriate evidence and rationale for closure.

## 8. Every element must earn its place

For every page, workflow, lesson, Coach behaviour, visual layer, data field, model integration, feature, and future capability, Fable must ask:

1. What real learner, professional, operational, UX, trust, or business problem does this solve?
2. Which DEIXEN objective does it advance, and how would the benefit be observed?
3. Is there a simpler or stronger alternative?
4. Does it duplicate another element or create unnecessary cognitive load?
5. What does it cost in complexity, dependencies, maintenance, validation, and learner attention?
6. Could it damage another part of the product, learning integrity, fairness, accessibility, or performance?

Use these dispositions when reviewing the existing product:

- **KEEP** — sound and useful; no change justified.
- **IMPROVE** — retain the purpose but improve the design or execution.
- **RETHINK / REPLACE** — current mechanism is weak; propose a better alternative.
- **COMBINE / SIMPLIFY** — remove duplication or complexity while preserving value.
- **REMOVE** — no sufficient value, duplicates another element, or harms the product; check dependencies and consequences first.
- **VALIDATE** — evidence is insufficient to decide safely.

Do not add features merely because they are novel, fashionable, competitor-visible, AI-enabled, or make the product appear more sophisticated. Prefer the smallest coherent solution that produces the strongest evidence-supported outcome.

## 9. Model team and delegation

Fable may use approximately three to five supporting models/contributors from available options such as Opus, Sonnet, Haiku, ChatGPT, and Gemini. Fable chooses the team and task-specific roles. A model is not automatically assigned a permanent domain, and no contributor may make independent product-level decisions. Keep one project lead, controlled delegation, and one integration owner.

## 10. First-stage authorization boundary

The first Fable assignment is **read-only reality inspection and product planning**. It does not authorize editing code, documents, branches, commits, pull requests, repositories, deployments, production data, or external systems. Fable may prepare recommendations, diagrams, specifications, and proposed changes. Implementation and source changes require separate explicit authorization.

---

**Governing summary:** Fable leads the development of the strongest evidence-backed DEIXEN—not the literal reproduction of historical documents. Fable decides technical matters, challenges everything with evidence, ensures every element earns its place, protects a simple learner experience, and returns substantive product decisions to the founder for explicit approval.
