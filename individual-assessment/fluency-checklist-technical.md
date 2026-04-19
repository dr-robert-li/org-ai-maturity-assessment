# Individual AI Fluency Checklist — Technical

> **Purpose**: Use this checklist to assess what a technical user (SWE, SRE, data/ML, designer, technical PM) is currently doing with Claude (Desktop, Code, API, and integrations). Tick items off during a discovery conversation or self-assessment.
>
> **Companion checklist**: For non-technical roles, use the [Non-Technical Fluency Checklist](fluency-checklist.md).
>
> **Relationship to the Rubric**: Each domain below maps 1:1 to the technical track in the [Fluency Rubric](fluency-rubric.md). Items mirror the rubric's "What good looks like" statements. Use the standard levels:
>
> - **Learning** → Score 1
> - **Competent** → Score 2
> - **Practitioner** → Score 3
> - **Power-User** → Score 4

---

## Levels

- **Learning**: Just starting. Uses Claude for real but small technical tasks with guidance.
- **Competent**: Uses Claude regularly on real code and docs; follows safe patterns.
- **Practitioner**: Designs AI-assisted workflows, integrations, and evals; shares skills/prompts.
- **Power-User**: Shapes team/org engineering practice with AI; owns shared tools, skills, and guardrails.

Tick every statement that is true of the person today. A person's level in each domain is determined by the highest level at which all (or nearly all) items are checked.

---

## Section 1: Foundations — Basic Usage (Technical)

- [ ] **Learning** – Has used Claude to help with real code or technical tasks (e.g. fix a bug, explain an error, refactor a small function, draft a technical doc).
- [ ] **Learning** – Understands the difference between ephemeral chats and Projects/workspaces and uses Projects (with CLAUDE.md or equivalent) for ongoing feature work.
- [ ] **Competent** – Can describe what Claude is good at (refactors, tests, docs, reasoning over a snippet) vs when to rely on local tools (IDE, debugger, CI).
- [ ] **Practitioner** – Uses Claude appropriately across interfaces (Desktop for design discussions, Code for in-repo work, API for scripts) and can justify the choice.

---

## Section 2: Prompting & Problem Decomposition (Technical)

- [ ] **Learning** – Provides relevant code and context (snippet, surrounding types, errors, goal) rather than just pasting an error message.
- [ ] **Competent** – Breaks complex problems into smaller, reviewable steps (outline → step-by-step implementation) instead of asking for one giant patch.
- [ ] **Practitioner** – Uses iteration and counter-prompts to pressure-test designs ("What are the failure modes?", "Propose two alternatives and their trade-offs").
- [ ] **Power-User** – Maintains reusable prompts, skills, or CLAUDE.md patterns for recurring problems (PR review, migrations, incident triage) that teammates adopt.

---

## Section 3: Code & System Integration

- [ ] **Learning** – Commits Claude-assisted code only after reading it line-by-line, running local tests, and making their own edits where appropriate.
- [ ] **Competent** – Understands context windows and how to scope what Claude sees (right files/snippets, trimmed noise, Projects/repo context).
- [ ] **Practitioner** – Has connected Claude to at least one real system via connectors / skills / MCP (GitHub, Jira, Slack, internal MCP server, custom skill) and uses it in normal workflows.
- [ ] **Power-User** – Owns or maintains a shared skill, tool, or agent that teammates use (e.g. code-review bot, MCP server, repo-scoped CLAUDE.md set).

---

## Section 4: Strategy & Value in My Role (Technical)

- [ ] **Competent** – Can name at least 1–2 technical tasks where Claude has measurably helped (e.g. PR review time, test migration, boilerplate generation).
- [ ] **Competent** – Can distinguish high-leverage AI coding tasks (refactors, tests, docs, scaffolding) from low-leverage or risky ones (novel distributed-systems design, security-critical code).
- [ ] **Practitioner** – Has proposed concrete AI-driven improvements to team or platform workflows (e.g. "Use Claude in CI to auto-summarise PRs") with rough cost/benefit.
- [ ] **Power-User** – Contributes to decisions about engineering strategy around AI-assisted development (tools, guardrails, shared practices) at team or org level.

---

## Section 5: Working With Data (Technical)

- [ ] **Competent** – Knows the data sources, schemas, and boundaries relevant to their work (and flags PII-sensitive queries).
- [ ] **Competent** – Sanity-checks data/code Claude produces (runs generated SQL on a sample, reads plans/explanations before running at scale).
- [ ] **Practitioner** – Uses Claude to co-develop reusable data workflows (scripts, notebooks, pipelines, DAGs) with tests/validations checked into the repo.
- [ ] **Power-User** – Contributes to data governance practices around AI (what datasets can be used, secrets/PII handling, documented team rules).

---

## Section 6: Collaboration, Documentation & Review

- [ ] **Learning** – Is transparent about AI-assisted work (mentions in PRs/commits where Claude meaningfully contributed).
- [ ] **Competent** – Uses Claude to improve documentation and onboarding (turns notes into clear READMEs, runbooks, onboarding docs).
- [ ] **Practitioner** – Uses Claude to accelerate code review and knowledge sharing (PR summaries, review checklists, explanations of unfamiliar code).
- [ ] **Power-User** – Codifies and teaches AI-assisted engineering practices (maintains team CLAUDE.md / skill packs / runbooks, runs internal training).

---

## Section 7: Safety, Testing & Observability

- [ ] **Learning** – Always reviews Claude-generated code before committing or deploying, especially in security-sensitive or infra code.
- [ ] **Competent** – Writes or runs tests for AI-generated code (unit/integration tests added or updated, or Claude-generated tests verified).
- [ ] **Competent** – Respects data, secrets, and licensing boundaries (no secrets, customer data, or sensitive IP in prompts; knows off-limits repos/datasets).
- [ ] **Practitioner** – Sets up evaluation and guardrails for recurring AI-assisted workflows (simple evals or review gates to catch regressions).
- [ ] **Power-User** – Owns or contributes to safety, logging, and observability for AI usage (API/agent logging, cost monitoring, prompt-injection defences, red-team reviews).

---

## Scoring Summary

For each section, record the highest level at which all (or nearly all) items are ticked. Convert to the 1–4 scale using Learning = 1, Competent = 2, Practitioner = 3, Power-User = 4.

| Section | Items Checked | Level (L/C/P/PU) | Score (1–4) |
|---------|:------------:|:----------------:|:-----------:|
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
| **3.5–4.0** | **Power-User** | Internal champion for AI-assisted engineering. Involve in org-level tooling, guardrails, and training. |
| **2.5–3.4** | **Practitioner** | Designs and improves AI-assisted workflows; shares skills/prompts; mentors peers. |
| **1.5–2.4** | **Competent** | Uses Claude reliably on real engineering work; ready to move from "follows patterns" to "designs patterns". |
| **1.0–1.4** | **Learning** | Needs structured onboarding and pairing with a Practitioner. |

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
