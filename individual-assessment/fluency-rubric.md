# Individual AI Fluency Rubric

> **Purpose**: Assess an individual's AI fluency across a set of role-relevant domains, using four standard levels: **Learner**, **Practitioner**, **Multiplier**, **Champion**. Use this rubric alongside the companion checklists:
>
> - [Non-Technical Fluency Checklist](fluency-checklist.md)
> - [Technical Fluency Checklist](fluency-checklist-technical.md)
>
> **Two tracks**: This rubric is split into two parallel tracks so the same framework can be applied fairly to both non-technical roles (sales, marketing, CS, ops, HR, finance, non-technical PMs) and technical roles (SWE, SRE, data/ML engineers, designers, technical PMs).
>
> **Relationship to the org assessment**: Individual domain scores roll up into the [MIT CISR-aligned AI Maturity Self-Assessment](../org-assessment/ai-maturity-self-assessment.md) via a documented mapping.
>
> **About this variant**: This is the **stricter-scoring variant** of the rubric. Tier names were renamed from `Learning / Competent / Practitioner / Power-User` to `Learner / Practitioner / Multiplier / Champion` to (a) remove the semantic blur between "Competent" and "Practitioner" and (b) replace "Power-User" with "Champion" to reflect strategic capability rather than tool intensity. See [CHANGELOG.md](../CHANGELOG.md) for the rationale.

---

## Levels

We use four levels of individual AI fluency. These are *role-relative* (non-technical vs technical) but conceptually consistent.

- **Learner**
  Just starting to use Claude or other AI tools in their work. Needs examples, checklists, and guidance. Uses AI in a few tasks, usually with help from others.

- **Practitioner**
  Uses Claude regularly for common tasks in their role. Follows basic safety and evaluation checklists. Can explain what they are doing to a peer, but usually follows patterns created by others.

- **Multiplier**
  Designs and improves workflows that incorporate Claude. Proactively evaluates outputs and updates prompts/skills based on error patterns. Shares working prompts/skills with others and adapts them to new situations. *Their impact extends past their own work — they amplify what teammates can do.*

- **Champion**
  Acts as a local AI champion. Teaches others, codifies best practice, and shapes how the team uses Claude. Connects Claude into other tools (e.g. connectors, skills, integrations) and thinks in systems (team-wide or org-wide usage).

### Numeric mapping

For scoring purposes (individual → team → org), use:

| Level | Score |
|-------|:-----:|
| Learner | 1 |
| Practitioner | 2 |
| Multiplier | 3 |
| Champion | 4 |

### How to use each item

Every rubric item below includes:

- A short description.
- A `Level:` tag — the level at which this behaviour is expected.
- A **What good looks like** section with concrete, procedural steps so assessors can recognise the behaviour in real work.
- (Optional) `Feeds org dimensions:` — which MIT CISR dimensions this item informs.

---

## Non-Technical Individual Fluency Rubric

This section is for non-technical roles such as:

- Sales, marketing, and customer success
- Operations, HR, finance, and general business roles
- Non-technical product roles, project/program managers

Examples mention specific artefacts (e.g. campaign brief, QBR), but should be interpreted in the context of the person's role.

### Domains (Non-Technical)

1. Foundations — Basic Usage
2. Prompting & Communication
3. Role-Relevant Applications
4. Strategy & Value in My Role
5. Working With Data (Non-Technical)
6. Collaboration & Team Behaviour
7. Safety & Critical Thinking (incl. Ethics & Escalation)

---

### Foundations — Basic Usage (Non-Technical)

- **Has logged into and regularly uses Claude Desktop**
  - Level: Learner
  - What good looks like: Uses Claude at least several times per week to support actual work tasks (e.g. drafting emails, summarising notes), not just tests or demos.
  - Feeds org dimensions: Talent & Culture

- **Understands the difference between a one-off chat and a Project**
  - Level: Learner
  - What good looks like: Uses Projects (or equivalent persistent context) for ongoing work like a long-running initiative, and uses fresh chats for one-off questions.
  - Feeds org dimensions: Talent & Culture

- **Has created at least one Artifact for their own work**
  - Level: Learner
  - What good looks like: Uses Claude to generate a document, table, checklist, or structured plan that is then saved and reused (e.g. a recurring meeting agenda or template).
  - Feeds org dimensions: Talent & Culture

- **Can describe what Claude is good at vs where it makes mistakes**
  - Level: Practitioner
  - What good looks like: Can say in their own words, for their role, "I use Claude for drafts, summaries, and brainstorming, but I always double-check facts, numbers, and sensitive topics such as legal or financial advice."
  - Feeds org dimensions: Talent & Culture, Governance

---

### Prompting & Communication (Non-Technical)

- **Writes prompts with clear instructions rather than one-line questions**
  - Level: Learner
  - What good looks like: Provides role, task, and desired format (e.g. "Act as my editor. Rewrite this email to be shorter and more polite. Keep it under 120 words.").

- **Iterates on a prompt when the first response is weak**
  - Level: Practitioner
  - What good looks like: After a poor response, adjusts the prompt (adds missing context, changes tone instructions, provides an example) rather than accepting the first output.

- **Uses multi-turn conversation to refine outputs**
  - Level: Practitioner
  - What good looks like: Builds on Claude's previous response across messages ("Good — now make it 30% shorter and add a warmer tone") instead of starting over each time.

- **Asks Claude to critique its own output or offer alternatives**
  - Level: Multiplier
  - What good looks like: After drafting, asks "What are the weaknesses here?" or "Give me two alternative versions with different tones," and uses the critique to improve the output.

- **Captures and shares their best prompts with the team**
  - Level: Champion
  - What good looks like: Maintains a short library of proven prompts (in Notion, a Google Doc, or a Slack canvas) and adds a new prompt whenever they find one that works well.

---

### Role-Relevant Applications (Non-Technical)

- **Used Claude to draft, summarise, or restructure a work document**
  - Level: Learner
  - Examples: policy, campaign brief, customer email, meeting agenda, performance review note.
  - What good looks like: Copies a messy draft or bullet notes into Claude and gets back a clearer, structured version they then lightly edit before use.
  - Feeds org dimensions: Talent & Culture

- **Used Claude to analyse or interpret structured information**
  - Level: Practitioner
  - Examples: CSV, table, dashboard screenshot, export from a CRM or HRIS.
  - What good looks like: Pastes or describes data and asks Claude for trends, outliers, or key takeaways, then cross-checks at least a few numbers against the source tool.
  - Feeds org dimensions: Strategy & Use Cases, Data

- **Used Claude to build or improve a template**
  - Level: Practitioner
  - Examples: meeting template, intake form, scorecard, email template, checklist.
  - What good looks like: Asks Claude to propose a template, then edits it and reuses it at least twice in real work.

- **Used Claude to support cross-functional communication**
  - Level: Multiplier
  - Examples: translating a technical process into exec language, adapting a message for a different audience.
  - What good looks like: Rewrites an internal memo for an executive audience or a customer-facing version and checks the tone against the audience's expectations.

- **Uses Claude in recurring reporting or review workflows**
  - Level: Multiplier
  - Examples: weekly KPI recap, campaign performance summary, customer health review, hiring pipeline report.
  - What good looks like: On a recurring basis (e.g. weekly), uses Claude to help draft a report and always checks key metrics before sharing.
  - Feeds org dimensions: Strategy & Use Cases

- **Redesigns a team workflow around Claude end-to-end**
  - Level: Champion
  - What good looks like: Rebuilds a recurring process (e.g. QBR prep, onboarding) so Claude is embedded at each step, and documents it as a repeatable playbook for others.

---

### Strategy & Value in My Role (Non-Technical)

- **Can name at least 1–2 tasks where Claude has already delivered meaningful value**
  - Level: Practitioner
  - What good looks like: Can say "Using Claude for this type of email has reduced my prep time by about half," or "Claude helps me summarise customer calls so I can spend more time preparing for the meeting."
  - Feeds org dimensions: Strategy & Use Cases

- **Can distinguish between low-value and high-value AI use cases in their role**
  - Level: Practitioner
  - What good looks like: Treats "summarising random articles" as nice-to-have, but prioritises "automating pre-meeting call summaries" because it clearly improves a core workflow.
  - Feeds org dimensions: Strategy & Use Cases

- **Can suggest at least one new AI use case aligned with team or company goals**
  - Level: Multiplier
  - What good looks like: Proposes a specific AI use case (e.g. "use Claude to create monthly customer health summaries before QBRs") and shares it with their manager or team.
  - Feeds org dimensions: Strategy & Use Cases, Talent & Culture

- **Influences team or org strategy with concrete AI proposals**
  - Level: Champion
  - What good looks like: Brings a short, written proposal (problem → use case → rough impact → risk) to a team or leadership forum and drives a decision.
  - Feeds org dimensions: Strategy & Use Cases

---

### Working With Data (Non-Technical)

- **Knows which internal reports are the source of truth for key metrics they ask Claude about**
  - Level: Practitioner
  - What good looks like: Says "For our key metrics, I always check [named dashboard/report]; Claude can help me summarise, but I confirm the numbers there."
  - Feeds org dimensions: Data

- **Does basic sense checks on data-related outputs from Claude**
  - Level: Practitioner
  - What good looks like: When Claude summarises metrics, they check totals or averages against the original report for at least a few line items.
  - Feeds org dimensions: Data, Governance

- **Understands, in simple terms, what data Claude has seen and what it has not**
  - Level: Multiplier
  - What good looks like: Can explain "Claude only sees the data I paste or connect; it does not automatically have full access to our internal systems, so I choose carefully what to share."
  - Feeds org dimensions: Data, Technology & Infrastructure

- **Helps define team-level norms for data used with Claude**
  - Level: Champion
  - What good looks like: Contributes to (or writes) a short guideline on what data is and is not safe to share with Claude for their team, with concrete examples.
  - Feeds org dimensions: Data, Governance

---

### Collaboration & Team Behaviour (Non-Technical)

- **Has shared a Claude output with a teammate or stakeholder**
  - Level: Learner
  - What good looks like: Does not hide the fact that AI helped them; is comfortable sharing outputs (with their own review) with peers.

- **Has discussed with the team when to use Claude vs not**
  - Level: Practitioner
  - What good looks like: Participates in team discussions about what Claude should and should not be used for (e.g. "We agreed not to use Claude for final performance reviews.").
  - Feeds org dimensions: Talent & Culture, Governance

- **Has taught or shown a colleague a prompt technique**
  - Level: Multiplier
  - What good looks like: Has walked a colleague through one of their own prompts or workflows at least once, either 1:1 or in a team meeting.
  - Feeds org dimensions: Talent & Culture

- **Team has shared prompts, skills, or conventions they contribute to**
  - Level: Multiplier
  - What good looks like: There is a place where the team stores and reuses prompts/skills, and this person adds to it or improves items in it.

- **Drives adoption and shared practices across the team**
  - Level: Champion
  - What good looks like: Runs a regular show-and-tell, maintains the shared prompt library, or is named as the go-to person for AI on their team.
  - Feeds org dimensions: Talent & Culture

---

### Safety & Critical Thinking (Non-Technical)

- **Does not treat Claude outputs as final without review**
  - Level: Learner
  - What good looks like: Always reads and edits Claude-generated emails, docs, or messages before sending.
  - Feeds org dimensions: Governance

- **Has caught at least one incorrect or misleading output and corrected it**
  - Level: Learner
  - What good looks like: Notices a wrong number or statement in a summary, corrects it, and optionally tells Claude what was wrong.

- **Understands that Claude does not see live internal systems unless explicitly integrated**
  - Level: Practitioner
  - What good looks like: Does not ask Claude for live values; instead, asks for help interpreting known reports or writing queries.
  - Feeds org dimensions: Technology & Infrastructure, Governance

- **Is aware of data/privacy considerations and can give examples of what not to paste**
  - Level: Practitioner
  - What good looks like: Can list items such as "I never paste full contract PDFs, payroll spreadsheets, or customer PII. I anonymise or aggregate instead."
  - Feeds org dimensions: Governance, Data

- **Recognises high-stakes or sensitive contexts and escalates when needed**
  - Level: Multiplier
  - What good looks like: Avoids using Claude for final performance ratings or disciplinary letters; uses it only to tidy language and involves HR or legal for content and decisions.
  - Feeds org dimensions: Governance

- **Has documented or shared a written data handling / ethics norm for the team**
  - Level: Champion
  - What good looks like: Has contributed to a one-pager on data handling or ethical AI use that the team actually references.
  - Feeds org dimensions: Governance

---

## Technical Individual Fluency Rubric

This section is for technical roles such as:

- Software engineers and SREs
- Data engineers, ML engineers, and analysts with significant coding responsibilities
- Designers, front-end developers, and technical product roles

Examples assume access to codebases, repos, and/or design systems. Adapt to the specific stack where needed.

### Domains (Technical)

1. Foundations — Basic Usage (Technical)
2. Prompting & Problem Decomposition (Technical)
3. Code & System Integration
4. Strategy & Value in My Role (Technical)
5. Working With Data (Technical)
6. Collaboration, Documentation & Review
7. Safety, Testing & Observability

---

### Foundations — Basic Usage (Technical)

- **Has used Claude on real technical work**
  - Level: Learner
  - What good looks like: Uses Claude to help fix a real bug, explain an unfamiliar error, refactor a small function, or draft a technical doc — not just for toy problems.
  - Feeds org dimensions: Talent & Culture

- **Understands the difference between ephemeral chats and Projects/workspaces**
  - Level: Learner
  - What good looks like: Uses Projects or a persistent workspace (with a CLAUDE.md or equivalent context file) for ongoing feature work; uses fresh chats for throwaway questions.
  - Feeds org dimensions: Talent & Culture

- **Can describe what Claude is good at vs when to rely on local tools**
  - Level: Practitioner
  - What good looks like: Says "Claude is strong on refactors, tests, docs, and reasoning over a pasted snippet; for deep debugging I still reach for the IDE debugger and CI logs."
  - Feeds org dimensions: Talent & Culture

- **Uses Claude across multiple interfaces (desktop, Code, API) appropriately**
  - Level: Multiplier
  - What good looks like: Uses Claude Desktop for design discussions, Claude Code for in-repo work, and API/SDK for scripts — and can explain when each is the right choice.
  - Feeds org dimensions: Technology & Infrastructure

---

### Prompting & Problem Decomposition (Technical)

- **Provides relevant code and context in prompts, not just error messages**
  - Level: Learner
  - What good looks like: Includes the failing snippet, the surrounding types/interfaces, and the error/output, and clearly states the goal.

- **Breaks complex problems into smaller, reviewable steps**
  - Level: Practitioner
  - What good looks like: Asks Claude to first outline an approach, then implement step-by-step with checkpoints, instead of requesting one giant patch.

- **Uses iteration and counter-prompts to pressure-test designs**
  - Level: Multiplier
  - What good looks like: Asks "What are the failure modes of this design?" or "Propose two alternatives and their trade-offs," and uses the critique to refine the solution.

- **Builds reusable prompts, skills, or CLAUDE.md patterns for recurring problems**
  - Level: Champion
  - What good looks like: Maintains a small library of prompts/skills (e.g. for PR review, migration scripts, incident triage) that teammates can adopt.
  - Feeds org dimensions: Talent & Culture, Technology & Infrastructure

---

### Code & System Integration

- **Uses Claude to generate or refactor code that is then actually used**
  - Level: Learner
  - What good looks like: Commits Claude-assisted code after reading it line-by-line, running local tests, and adding their own edits where appropriate.
  - Feeds org dimensions: Technology & Infrastructure

- **Understands context windows and how to scope what Claude sees**
  - Level: Practitioner
  - What good looks like: Selects the right files/snippets to share, trims noise, and uses Projects or repo context to avoid pasting irrelevant code.

- **Uses Claude with connectors, skills, or MCP-style integrations**
  - Level: Multiplier
  - What good looks like: Has connected Claude to at least one real system (GitHub, Jira, Slack, an internal MCP server, a custom skill) and uses it in their normal workflow.
  - Feeds org dimensions: Technology & Infrastructure, Data

- **Designs or maintains an internal skill, tool, or agent used by others**
  - Level: Champion
  - What good looks like: Owns a shared skill/agent (e.g. an internal code-review bot, an MCP server, a repo-scoped CLAUDE.md set) that teammates use.
  - Feeds org dimensions: Technology & Infrastructure, Talent & Culture

---

### Strategy & Value in My Role (Technical)

- **Can name at least 1–2 technical tasks where Claude has measurably helped**
  - Level: Practitioner
  - What good looks like: Points to concrete examples — "Claude cut PR review time in half on this repo" or "Claude helped me migrate 40 tests from X to Y in a day."
  - Feeds org dimensions: Strategy & Use Cases

- **Can distinguish high-leverage AI coding tasks from low-leverage ones**
  - Level: Practitioner
  - What good looks like: Prioritises Claude for refactors, tests, docs, boilerplate, and scaffolding; treats it cautiously for novel distributed-systems design or security-critical code.
  - Feeds org dimensions: Strategy & Use Cases, Governance

- **Proposes AI-driven improvements to team or platform workflows**
  - Level: Multiplier
  - What good looks like: Proposes concrete uses (e.g. "Use Claude in CI to auto-generate PR summaries for reviewers") with a rough cost/benefit view.
  - Feeds org dimensions: Strategy & Use Cases

- **Shapes engineering strategy around AI-assisted development**
  - Level: Champion
  - What good looks like: Contributes to decisions about tools, guardrails, and shared practices for AI-assisted development at the team or org level.
  - Feeds org dimensions: Strategy & Use Cases, Technology & Infrastructure

---

### Working With Data (Technical)

- **Knows the data sources and schemas relevant to their work**
  - Level: Practitioner
  - What good looks like: Can point Claude to the right table, schema, or dataset, and flags when asked questions that cross data boundaries (e.g. PII-sensitive joins).
  - Feeds org dimensions: Data

- **Does sanity checks on data/code that Claude produces**
  - Level: Practitioner
  - What good looks like: Runs generated SQL against a small sample, compares against a known result, and reads plans/explanations before running at scale.
  - Feeds org dimensions: Data, Governance

- **Uses Claude to build reusable data workflows (scripts, notebooks, DAGs)**
  - Level: Multiplier
  - What good looks like: Co-develops a pipeline or analysis notebook with Claude, adds tests/validations, and checks it in so others can reuse it.
  - Feeds org dimensions: Data, Technology & Infrastructure

- **Contributes to data governance practices around AI use**
  - Level: Champion
  - What good looks like: Helps define what datasets can be used with Claude, how secrets/PII are handled, and documents these rules for the team.
  - Feeds org dimensions: Data, Governance

---

### Collaboration, Documentation & Review

- **Is transparent about AI-assisted work**
  - Level: Learner
  - What good looks like: Mentions in PR descriptions or commit messages where Claude meaningfully contributed (without being performative about it).

- **Uses Claude to improve documentation and onboarding**
  - Level: Practitioner
  - What good looks like: Uses Claude to turn scattered notes into clear READMEs, runbooks, or onboarding docs, and keeps them up to date.
  - Feeds org dimensions: Talent & Culture

- **Uses Claude to accelerate code review and knowledge sharing**
  - Level: Multiplier
  - What good looks like: Uses Claude to summarise large PRs, generate review checklists, or explain unfamiliar parts of the codebase to reviewers.
  - Feeds org dimensions: Talent & Culture

- **Codifies and teaches AI-assisted engineering practices**
  - Level: Champion
  - What good looks like: Maintains team-level CLAUDE.md, skill packs, or runbooks, and runs or contributes to internal training sessions.
  - Feeds org dimensions: Talent & Culture, Governance

---

### Safety, Testing & Observability

- **Always reviews Claude-generated code before committing or deploying**
  - Level: Learner
  - What good looks like: Reads every line, runs it locally, and never blindly accepts a diff — especially in security-sensitive or infra code.
  - Feeds org dimensions: Governance

- **Writes or runs tests for AI-generated code**
  - Level: Practitioner
  - What good looks like: Adds or updates unit/integration tests for changes, or asks Claude to generate tests and then verifies them.
  - Feeds org dimensions: Governance, Technology & Infrastructure

- **Understands and respects data, secrets, and licensing boundaries**
  - Level: Practitioner
  - What good looks like: Does not paste secrets, customer data, or sensitive IP into prompts; knows which repos/datasets are off-limits.
  - Feeds org dimensions: Governance, Data

- **Sets up evaluation and guardrails for recurring AI-assisted workflows**
  - Level: Multiplier
  - What good looks like: For repeatable AI tasks (e.g. auto-generated PR summaries), defines simple evals or review gates to catch regressions.
  - Feeds org dimensions: Governance, Technology & Infrastructure

- **Owns or contributes to safety, logging, and observability for AI usage**
  - Level: Champion
  - What good looks like: Helps establish logging for API/agent usage, cost monitoring, prompt-injection defences, or red-team style reviews.
  - Feeds org dimensions: Governance, Technology & Infrastructure

---

## Scoring From Individual to Organisation

Use the following approach to aggregate rubric scores:

1. **Assign numeric values to levels**: Learner = 1, Practitioner = 2, Multiplier = 3, Champion = 4.

2. **For each person**:
   - For each domain, calculate the average level across the relevant items (rubric items or their checklist mirrors).
   - Record a per-domain score and an overall average.

3. **For each team or function**:
   - Average individuals' domain scores to get a team-level view (e.g. "Marketing: strong in Applications, weak in Safety").

4. **For the organisation**:
   - Use the domain → MIT CISR mapping in [AI Maturity Self-Assessment](../org-assessment/ai-maturity-self-assessment.md) to aggregate domain scores into CISR dimensions (Strategy & Use Cases, Data, Technology & Infrastructure, Talent & Culture, Governance, and Organisational Culture).
   - Combine with the org-level depth-scored self-assessment to get a full picture.

Use these aggregates to identify priority areas for training and strategic investment.

---

## Assessment Worksheet

| Domain | Track | Level (L/P/M/C) | Score (1–4) | Evidence / Notes |
|--------|-------|:---------------:|:-----------:|------------------|
| Foundations — Basic Usage | Non-Tech / Tech | | | |
| Prompting & Communication / Decomposition | Non-Tech / Tech | | | |
| Role-Relevant Applications / Code & System Integration | Non-Tech / Tech | | | |
| Strategy & Value in My Role | Non-Tech / Tech | | | |
| Working With Data | Non-Tech / Tech | | | |
| Collaboration & Team Behaviour / Collaboration, Docs & Review | Non-Tech / Tech | | | |
| Safety & Critical Thinking / Safety, Testing & Observability | Non-Tech / Tech | | | |
| **Average** | | | **___/4** | |

---

## Generating Recommendations from Levels

### Learner (1) in any domain → Priority gap

| Domain at Learner | Recommended Actions |
|-------------------|---------------------|
| Foundations — Basic Usage | Pair the person with a Multiplier for a 30-minute onboarding session. Install Claude Desktop / Claude Code, set up Projects, and complete one real task together. |
| Prompting | Provide 3–5 worked examples of structured prompts for their role. Run a short coaching session on role/task/context/format framing. |
| Role-Relevant Applications / Code & System Integration | Map Claude to 2–3 specific recurring tasks. Demonstrate each one live. Set a two-week goal of using Claude for at least one of these tasks daily. |
| Strategy & Value | Help them identify one use case with clear, measurable value in their role. Track the before/after. |
| Working With Data | Walk through the team's data sources of truth and what can/cannot be shared with Claude. |
| Collaboration | Invite them to the team AI channel. Pair with a Multiplier or Champion to observe their workflow. |
| Safety & Critical Thinking / Safety, Testing & Observability | Provide the team's data handling one-pager. Introduce a simple verification habit: "Before sharing any Claude output, check one fact and one number." |

### Practitioner (2) → Strengthening opportunity

| Domain at Practitioner | Recommended Actions |
|------------------------|---------------------|
| Any domain | Move from "follows patterns" to "designs patterns" — have them document their best prompt/skill, embed Claude into one recurring cadence, and propose one new use case. |

### Multiplier (3) → Scale

| Domain at Multiplier | Recommended Actions |
|----------------------|---------------------|
| Any domain | Encourage them to lead show-and-tells, contribute skills or CLAUDE.md patterns, and mentor one Practitioner peer. |

### Champion (4) → Shape strategy

| Domain at Champion | Recommended Actions |
|--------------------|---------------------|
| Any domain | Position as internal AI champion. Involve in org-level strategy, policy drafting, and cross-team enablement. |

---

## Example: Completed Assessment (Non-Technical)

| Domain | Level | Score | Evidence |
|--------|-------|:-----:|----------|
| Foundations — Basic Usage | Practitioner | 2 | Uses Claude Desktop daily; has created several Artifacts; not yet using Projects consistently. |
| Prompting & Communication | Practitioner | 2 | Clear role/task prompts; rarely iterates or uses multi-turn. |
| Role-Relevant Applications | Multiplier | 3 | Uses Claude for drafts, data interpretation, and weekly summaries. |
| Strategy & Value in My Role | Practitioner | 2 | Can name time saved on emails; has not yet proposed a new use case. |
| Working With Data | Learner | 1 | Loose understanding of sources of truth; rarely cross-checks numbers. |
| Collaboration & Team Behaviour | Learner | 1 | Mostly a solo user; has not shared prompts with the team. |
| Safety & Critical Thinking | Practitioner | 2 | Understands broad data risks; no documented team norms. |
| **Average** | | **1.9** | **Practitioner-leaning** — solid individual use; priority is data literacy and team leverage. |

### Recommendations from this example

1. **Priority 1** (Working With Data, Collaboration): Walk through team's sources of truth; invite to team AI channel; pair with a Multiplier.
2. **Priority 2** (Strategy & Value, Safety): Identify one measurable use case; contribute to a team data-handling norm.
3. **Priority 3** (Prompting): Coach on multi-turn conversation and prompt iteration.
