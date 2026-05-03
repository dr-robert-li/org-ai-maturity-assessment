# Individual AI Fluency Checklist — Technical

> **Purpose**: Use this checklist to assess what a technical user (SWE, SRE, data/ML, designer, technical PM) is currently doing with Claude (Desktop, Code, API, and integrations). Tick items off during a discovery conversation or self-assessment.
>
> **Companion checklist**: For non-technical roles, use the [Non-Technical Fluency Checklist](fluency-checklist.md).
>
> **Relationship to the Rubric**: Each domain below maps 1:1 to the technical track in the [Fluency Rubric](fluency-rubric.md). Items mirror the rubric's "What good looks like" statements. Use the standard levels:
>
> - **Learner** → Score 1
> - **Practitioner** → Score 2
> - **Multiplier** → Score 3
> - **Champion** → Score 4

---

## Levels

- **Learner**: Just starting. Uses Claude for real but small technical tasks with guidance.
- **Practitioner**: Uses Claude regularly on real code and docs; follows safe patterns.
- **Multiplier**: Designs AI-assisted workflows, integrations, and evals; shares skills/prompts; amplifies the team.
- **Champion**: Shapes team/org engineering practice with AI; owns shared tools, skills, and guardrails.

Tick every statement that is true of the person today. A person's level in each domain is determined by the highest level at which all (or nearly all) items are checked.

---

## Section 1: Foundations — Basic Usage (Technical)

- [ ] **Learner** – Has used Claude to help with real code or technical tasks (e.g. fix a bug, explain an error, refactor a small function, draft a technical doc).
- [ ] **Learner** – Understands the difference between ephemeral chats and Projects/workspaces and uses Projects (with CLAUDE.md or equivalent) for ongoing feature work.
- [ ] **Practitioner** – Can describe what Claude is good at (refactors, tests, docs, reasoning over a snippet) vs when to rely on local tools (IDE, debugger, CI).
- [ ] **Multiplier** – Uses Claude appropriately across interfaces (Desktop for design discussions, Code for in-repo work, API for scripts) and can justify the choice.

---

## Section 2: Prompting & Problem Decomposition (Technical)

- [ ] **Learner** – Provides relevant code and context (snippet, surrounding types, errors, goal) rather than just pasting an error message.
- [ ] **Practitioner** – Breaks complex problems into smaller, reviewable steps (outline → step-by-step implementation) instead of asking for one giant patch.
- [ ] **Multiplier** – Uses iteration and counter-prompts to pressure-test designs ("What are the failure modes?", "Propose two alternatives and their trade-offs").
- [ ] **Champion** – Maintains reusable prompts, skills, or CLAUDE.md patterns for recurring problems (PR review, migrations, incident triage) that teammates adopt.

---

## Section 3: Code & System Integration

- [ ] **Learner** – Commits Claude-assisted code only after reading it line-by-line, running local tests, and making their own edits where appropriate.
- [ ] **Practitioner** – Understands context windows and how to scope what Claude sees (right files/snippets, trimmed noise, Projects/repo context).
- [ ] **Multiplier** – Has connected Claude to at least one real system via connectors / skills / MCP (GitHub, Jira, Slack, internal MCP server, custom skill) and uses it in normal workflows.
- [ ] **Champion** – Owns or maintains a shared skill, tool, or agent that teammates use (e.g. code-review bot, MCP server, repo-scoped CLAUDE.md set).

---

## Section 4: Strategy & Value in My Role (Technical)

- [ ] **Practitioner** – Can name at least 1–2 technical tasks where Claude has measurably helped (e.g. PR review time, test migration, boilerplate generation).
- [ ] **Practitioner** – Can distinguish high-leverage AI coding tasks (refactors, tests, docs, scaffolding) from low-leverage or risky ones (novel distributed-systems design, security-critical code).
- [ ] **Multiplier** – Has proposed concrete AI-driven improvements to team or platform workflows (e.g. "Use Claude in CI to auto-summarise PRs") with rough cost/benefit.
- [ ] **Champion** – Contributes to decisions about engineering strategy around AI-assisted development (tools, guardrails, shared practices) at team or org level.

---

## Section 5: Working With Data (Technical)

- [ ] **Practitioner** – Knows the data sources, schemas, and boundaries relevant to their work (and flags PII-sensitive queries).
- [ ] **Practitioner** – Sanity-checks data/code Claude produces (runs generated SQL on a sample, reads plans/explanations before running at scale).
- [ ] **Multiplier** – Uses Claude to co-develop reusable data workflows (scripts, notebooks, pipelines, DAGs) with tests/validations checked into the repo.
- [ ] **Champion** – Contributes to data governance practices around AI (what datasets can be used, secrets/PII handling, documented team rules).

---

## Section 6: Collaboration, Documentation & Review

- [ ] **Learner** – Is transparent about AI-assisted work (mentions in PRs/commits where Claude meaningfully contributed).
- [ ] **Practitioner** – Uses Claude to improve documentation and onboarding (turns notes into clear READMEs, runbooks, onboarding docs).
- [ ] **Multiplier** – Uses Claude to accelerate code review and knowledge sharing (PR summaries, review checklists, explanations of unfamiliar code).
- [ ] **Champion** – Codifies and teaches AI-assisted engineering practices (maintains team CLAUDE.md / skill packs / runbooks, runs internal training).

---

## Section 7: Safety, Testing & Observability

- [ ] **Learner** – Always reviews Claude-generated code before committing or deploying, especially in security-sensitive or infra code.
- [ ] **Practitioner** – Writes or runs tests for AI-generated code (unit/integration tests added or updated, or Claude-generated tests verified).
- [ ] **Practitioner** – Respects data, secrets, and licensing boundaries (no secrets, customer data, or sensitive IP in prompts; knows off-limits repos/datasets).
- [ ] **Multiplier** – Sets up evaluation and guardrails for recurring AI-assisted workflows (simple evals or review gates to catch regressions).
- [ ] **Champion** – Owns or contributes to safety, logging, and observability for AI usage (API/agent logging, cost monitoring, prompt-injection defences, red-team reviews).

---

## Scoring Summary

For each section, record the highest level at which all (or nearly all) items are ticked. Convert to the 1–4 scale using Learner = 1, Practitioner = 2, Multiplier = 3, Champion = 4.

| Section | Items Checked | Level (L/P/M/C) | Score (1–4) |
|---------|:------------:|:---------------:|:-----------:|
| 1. Foundations — Basic Usage (Technical) | ___ / 4 | | |
| 2. Prompting & Problem Decomposition | ___ / 4 | | |
| 3. Code & System Integration | ___ / 4 | | |
| 4. Strategy & Value in My Role (Technical) | ___ / 4 | | |
| 5. Working With Data (Technical) | ___ / 4 | | |
| 6. Collaboration, Documentation & Review | ___ / 4 | | |
| 7. Safety, Testing & Observability | ___ / 5 | | |
| **Average** | | | **___/4** |

### Interpreting the Average

| Average Score | Stage | Interpretation |
|:-------------:|-------|----------------|
| **3.5–4.0** | **Champion** | Internal champion for AI-assisted engineering. Involve in org-level tooling, guardrails, and training. |
| **2.5–3.4** | **Multiplier** | Designs and improves AI-assisted workflows; shares skills/prompts; mentors peers. |
| **1.5–2.4** | **Practitioner** | Uses Claude reliably on real engineering work; ready to move from "follows patterns" to "designs patterns". |
| **1.0–1.4** | **Learner** | Needs structured onboarding and pairing with a Multiplier. |

> See the [Fluency Rubric](fluency-rubric.md) for detailed descriptors, "What good looks like" examples, and recommendations by level.

---

## Notes

_Use this space to capture observations, quotes, or context from the assessment conversation._

```
[Date]:
[Assessor]:
[Subject]:
[Track]: Technical

Observations:



Key Gaps:



Recommended Next Steps:


```
