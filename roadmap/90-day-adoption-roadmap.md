# 90-Day Organisation-Wide AI Adoption Roadmap

> **Purpose**: A phased framework for developing organisation-wide AI fluency and adoption, centred on the Claude ecosystem. Designed for organisations where some individuals are already using Claude but adoption is informal, uncoordinated, and lacks governance.
>
> **Prerequisites**: Complete the [Individual Fluency Rubric](../individual-assessment/fluency-rubric.md) using the [Non-Technical Checklist](../individual-assessment/fluency-checklist.md) and [Technical Checklist](../individual-assessment/fluency-checklist-technical.md) for key users, plus the [Organisation Maturity Self-Assessment](../org-assessment/ai-maturity-self-assessment.md) before starting. These inform where to focus effort.

---

## Root-to-Tip Adoption

This 90-day roadmap is **root-to-tip**:

- **Roots**: individual skills and habits (measured by the individual fluency rubric and the two track-specific checklists).
- **Trunk**: team-level patterns and playbooks (shared prompts, skills, CLAUDE.md, Slack channels, team evals).
- **Canopy**: organisation-level AI strategy and governance (measured using the MIT CISR AI maturity framework).

We deliberately avoid pure top-down mandates. Instead, we create lightweight structures so local experiments can spread and be standardised where they prove their value.

### Non-Mandate Principle

We do not mandate specific prompts, skills, or workflows across the entire organisation on Day 1.

Instead, we:

- Encourage teams to adopt patterns that work locally.
- Promote proven patterns upward via Slack, CLAUDE.md, and skills libraries.
- Standardise only what has already demonstrated value across multiple teams.

### Phase Overview

| Phase | Days | Focus | Primary Layer |
|-------|------|-------|---------------|
| Phase 1 | 0–30 | Seed the Roots — Individuals + Champions | Roots |
| Phase 2 | 31–60 | Grow the Trunk — Teams + Domains | Trunk |
| Phase 3 | 61–90 | Shape the Canopy — Org Strategy + Metrics | Canopy |

---

## Phase 1: Seed the Roots (Days 0–30)

**Theme**: Individuals and champions — governance basics, discovery, and quick wins.

### 1.1 Establish Governance Basics

| Action | Owner | Deliverable |
|--------|-------|-------------|
| Draft a data handling guideline — what can and cannot be pasted into Claude (no client PII, no raw revenue data without anonymisation) | AI Champion / Consultant | One-page data handling guideline |
| Agree on the guideline with the team — does not need legal sign-off to start; a team-agreed norm is enough | Team Lead | Acknowledged by all users |
| Clarify tool landscape — when to use Claude Desktop vs. chat integrations vs. Excel/PowerPoint add-ins | Consultant | Tool selection guidance document |

### 1.2 Identify Power-Users and Run a Listening Tour

| Action | Owner | Deliverable |
|--------|-------|-------------|
| Identify who in the org is already using Claude (formal or informal) across both non-technical and technical roles | AI Champion | List of current users with estimated fluency level (Learning / Competent / Practitioner / Power-User) |
| Conduct individual fluency assessments using the [rubric](../individual-assessment/fluency-rubric.md) plus the appropriate checklist — [non-technical](../individual-assessment/fluency-checklist.md) or [technical](../individual-assessment/fluency-checklist-technical.md) — for 3–5 key users per track | Consultant | Completed assessment worksheets per track |
| Run the [Org Maturity Self-Assessment](../org-assessment/ai-maturity-self-assessment.md) across departments | AI Champion + Consultant | Aggregate maturity score and dimension breakdown |
| Identify 2–3 Power-Users (and high Practitioners) who can become internal champions | Consultant | Named champions with buy-in |
| Invite identified Power-Users and high Practitioners to choose 1–2 workflows each to improve with Claude | Champions | Self-chosen local experiments (no mandates) |

### 1.3 Set Up Sharing Infrastructure

| Action | Owner | Deliverable |
|--------|-------|-------------|
| Create a shared Slack/Teams channel (e.g. `#ai-claude-best-practice`) for Claude tips, prompts, and wins | AI Champion | Active channel with initial seed content |
| Pin key prompts, skills, CLAUDE.md guidance, and the safety one-pager in the channel | AI Champion | Pinned resources available to all |
| Start a shared prompt library — even a Google Doc or Notion page with 5–10 prompts the team already uses informally | Champions | Living prompt library document |
| Encourage champions to pair up for mutual accountability | Consultant | Paired champions |

### 1.4 Quick Wins

| Action | Owner | Deliverable |
|--------|-------|-------------|
| Activate features users have not yet tried (e.g., Claude Excel add-in, PowerPoint, Google Workspace integration) | Consultant | Demo session completed |
| Show each power user one new Claude capability relevant to their workflow | Consultant | Individual recommendations delivered |
| Each champion uses Claude in at least one recurring task this month | Champions | Usage log or self-report |

### Phase 1 Exit Criteria

- [ ] Data handling guideline published and acknowledged
- [ ] 3+ individual fluency assessments completed per track (non-technical and technical)
- [ ] Organisation maturity score calculated
- [ ] Shared channel active with at least 2 contributors
- [ ] Prompt library started with 5+ entries
- [ ] Each identified Power-User / high Practitioner has chosen 1–2 local workflows to improve with Claude

---

## Phase 2: Grow the Trunk (Days 31–60)

**Theme**: Teams and domains — skill development, team patterns, and integration activation.

### 2.0 Aggregate Individual Scores by Team and Domain

| Action | Owner | Deliverable |
|--------|-------|-------------|
| Aggregate individual rubric/checklist scores by domain and team to reveal patterns (e.g. "Marketing strong in Applications, weak in Safety"; "Engineering strong in Code & System Integration, weak in Working With Data") | Consultant | Team-by-domain score matrix |
| Map domain scores to MIT CISR dimensions using the mapping in [ai-maturity-self-assessment.md](../org-assessment/ai-maturity-self-assessment.md) | Consultant | Preliminary CISR dimension view |
| Each team documents a small set of recommended prompts/workflows for their function, plus a short "When to use AI vs not" guide | Team Leads + Champions | Team playbook v0 |

### 2.1 Develop Prompting Skills

| Action | Owner | Deliverable |
|--------|-------|-------------|
| Coach champions on multi-turn conversation habits (treating Claude as a thinking partner, not a search engine) | Consultant | Coaching session completed |
| Introduce prompt versioning — when a prompt improves, note what changed and why | Champions | Version-tracked prompts in library |
| Run a 30-minute workshop: "Structured Prompting for [Your Domain]" | Consultant | Workshop delivered, recording available |

### 2.2 Activate Integrations

| Action | Owner | Deliverable |
|--------|-------|-------------|
| Demonstrate Claude Excel and PowerPoint add-ins in a domain-relevant context (e.g., pipeline data analysis, QBR slide prep) | Consultant | Demo completed, adoption started |
| If on Claude Team/Enterprise: introduce Claude Projects for persistent team context | Consultant | First Project created |
| Introduce Managed Agents and Routines if available on the plan | Consultant | Assessment of applicability |

### 2.3 Build Evaluation Habits

| Action | Owner | Deliverable |
|--------|-------|-------------|
| For the team's top 2–3 Claude use cases, define what a "good output" looks like (simple rubric or checklist) | Champions + Consultant | Output quality rubrics |
| Introduce the "test case" habit — save 2–3 example inputs and expected outputs alongside each prompt | Champions | Test cases for top prompts |
| Use the [Human-in-the-Loop Review Form](../adoption-templates/human-in-the-loop-review.md) for any Claude output going to external stakeholders | Team | Form in use |

### 2.4 First Team Ritual

| Action | Owner | Deliverable |
|--------|-------|-------------|
| Pilot the [Weekly Victory Sharing Circle](../adoption-templates/victory-journal.md) — 30 min weekly, champions share wins | AI Champion | 4 sessions completed |
| Host the first show-and-tell from a power user (5–10 min demo of their best Claude workflow) | Champion | Session completed |

### Phase 2 Exit Criteria

- [ ] Team-by-domain score matrix produced and shared with team leads
- [ ] Preliminary CISR dimension mapping completed
- [ ] Each participating team has a v0 playbook ("When to use AI vs not" + recommended prompts)
- [ ] At least one integration activated and in regular use (Excel, PowerPoint, Workspace, or an engineering integration)
- [ ] Output quality rubrics exist for 2+ use cases
- [ ] Victory Sharing Circle running weekly
- [ ] Multi-turn prompting demonstrated by champions
- [ ] Prompt library has 10+ entries with version history

---

## Phase 3: Shape the Canopy (Days 61–90)

**Theme**: Org strategy and metrics — embed Claude into workflows, expand beyond champions, formalise practices, and connect to MIT CISR dimensions.

### 3.1 Embed in Recurring Workflows

| Action | Owner | Deliverable |
|--------|-------|-------------|
| Pick one end-to-end workflow and rebuild it with Claude embedded at each step (e.g., weekly pipeline review, QBR prep, territory planning) | Champion + Consultant | Documented workflow with before/after comparison |
| Map Claude to the team's recurring calendar — identify every meeting, report, or review where Claude should be in the workflow | Champions | Claude workflow calendar |
| Measure time saved, quality improvement, or other impact metrics using the [Success Metrics Dashboard](../adoption-templates/success-metrics-dashboard.md) | AI Champion | Dashboard populated with 60 days of data |

### 3.2 Expand Beyond Champions

| Action | Owner | Deliverable |
|--------|-------|-------------|
| Run a broader workshop (all hands or department-wide) — "How We Use Claude in [Department]" led by champions | Champions | Workshop delivered |
| Champions each mentor 1–2 new users through their first week of Claude use | Champions | Mentees onboarded |
| Share the prompt library and data handling guideline with new users | AI Champion | Distribution confirmed |

### 3.3 Formalise and Sustain

| Action | Owner | Deliverable |
|--------|-------|-------------|
| Formalise the prompt library into a versioned, maintained asset (consider GitHub for versioning if the team is ready, otherwise keep in Docs/Notion) | AI Champion | Versioned library with maintenance owner |
| Set [Quarterly OKRs](../adoption-templates/quarterly-okr-template.md) for AI adoption for the next quarter | Team Lead + Consultant | OKRs published |
| Establish a quarterly review cadence using the [Red-Teaming Checklist](../adoption-templates/quarterly-red-teaming-checklist.md) | Consultant | First quarterly review scheduled |
| If the organisation is ready: pilot a [Pilot Program Charter](../adoption-templates/pilot-program-charter.md) for the next AI initiative | Team Lead | Charter drafted |

### 3.4 Assess, Report, and Set the Canopy

| Action | Owner | Deliverable |
|--------|-------|-------------|
| Re-run the [Organisation Maturity Self-Assessment](../org-assessment/ai-maturity-self-assessment.md) and compare to Day 1 baseline | Consultant | Before/after comparison |
| Re-assess individual fluency for champions (across both tracks) and compare to initial levels | Consultant | Progress report showing level transitions (Learning → Competent → Practitioner → Power-User) |
| Populate the MIT CISR AI maturity view using combined individual + org scores (per the scoring guidance in the org assessment) | Consultant | CISR dimension scorecard |
| Identify 2–3 strategic focus areas for the next 90 days (e.g. raise non-technical Safety, level up technical Code & System Integration, improve Data literacy) and align with org-level initiatives (training, connectors, policies) | Team Lead + Consultant | Next-quarter focus areas |
| Decide on a cadence (e.g. every 6–12 months) to re-run individual assessments and track progress at both individual and CISR dimension levels | Team Lead | Recurring review cadence |
| Prepare a business case summary: what worked, what the impact was, what the next 90 days should focus on | Consultant | Business case document |

### Phase 3 Exit Criteria

- [ ] Claude embedded in at least one recurring team workflow
- [ ] 2+ non-champion users actively using Claude in each participating team
- [ ] Before/after maturity comparison completed
- [ ] CISR dimension scorecard produced and 2–3 strategic focus areas agreed
- [ ] Recurring assessment cadence agreed (6–12 months)
- [ ] Quarterly OKRs set for next quarter
- [ ] Business case documented for leadership

---

## Post-90-Day: What Comes Next

Based on Day 90 maturity scores, the typical next moves are:

| Maturity Stage | Recommended Next Focus |
|----------------|------------------------|
| **Foundational (0–8)** | Continue Phase 1–2 activities. Focus on individual literacy and governance basics. Consider whether the right people are championing adoption. |
| **Developing (9–16)** | Focus on cross-departmental expansion. Start a formal training programme. Evaluate Claude Team/Enterprise plans for better governance and Projects. |
| **Mature (17–24)** | Invest in custom skills and integrations. Explore API-driven automation. Formalise a Centre of Excellence or AI Guild. Begin advanced use cases (agents, MCP servers). |
| **Leading (25–30)** | Shift to frontier innovation. Contribute to internal knowledge assets. Build proprietary skills. Evaluate competitive differentiation through AI. |

---

## Suggested Tooling by Phase

| Phase | Recommended Tools | Reference |
|-------|-------------------|-----------|
| Phase 1 | Claude Desktop, built-in document skills | [Tooling Reference](../tooling-reference/claude-ecosystem-reference.md) |
| Phase 2 | Claude Excel/PowerPoint add-ins, Enterprise AI Skills (consulting frameworks), Claude Projects | [Tooling Reference](../tooling-reference/claude-ecosystem-reference.md) |
| Phase 3 | Shared prompt library, SkillsMP for domain skills, consider Skill Seekers for custom skill creation | [Tooling Reference](../tooling-reference/claude-ecosystem-reference.md) |
| Post-90 | Claude Code + Superpowers or GSD (for dev teams), MCP servers, custom skills built from internal documentation | [Tooling Reference](../tooling-reference/claude-ecosystem-reference.md) |
