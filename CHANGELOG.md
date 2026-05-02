# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [0.4.0] - 2026-05-03 — Stricter Scoring & MIT CISR Alignment Variant

> **Branch variant**: Released on `refactor/stricter-scoring-and-mit-cisr-alignment`. The `main` branch retains the prior generous scoring as a separate variant. This variant exists in response to client feedback that the prior model produced inflated maturity ratings.

### Changed

- **Org Assessment** (`org-assessment/ai-maturity-self-assessment.md`):
  - **Depth scoring**: Replaced binary Yes/No (max 30) with three-point depth scoring `0 = No`, `1 = Partial`, `2 = Yes — Evidenced` (max 60). The "Partial" middle ground prevents a paper-only policy and a mature practice from scoring identically. Calibration rule: if the first instinct is "yes, but…", the answer is 1.
  - **Stage names aligned to MIT CISR**: `Foundational / Developing / Mature / Leading` renamed to `Stage 1: Experiment and Prepare / Stage 2: Build Pilots and Capabilities / Stage 3: Develop AI Ways of Working / Stage 4: AI Future Ready` per the [MIT CISR Enterprise AI Maturity Model](https://cisr.mit.edu/publication/2024_1201_EnterpriseAIMaturityModel_WeillWoernerSebastian).
  - **Asymmetric band thresholds**: 0–20 / 21–38 / 39–52 / 53–60. The Stage 2 → Stage 3 band is the widest because MIT CISR data shows it is the hardest, most consequential crossing (it is where growth and profit move from negative to positive).
  - **Prerequisite gates added**: To reach Stage 3, Data Infrastructure AND Governance dimensions must each score ≥ 4/10 — otherwise capped at Stage 2 ceiling (38). To reach Stage 4, ALL six dimensions must score ≥ 7/10 — otherwise capped at Stage 3 ceiling (52). Gate outcomes must be reported explicitly. This prevents strong soft-dimension scores (e.g. Culture) from numerically masking failed structural dimensions.
  - **Recalibrated dimension → 1–4 conversion** for individual+org roll-up: 0–3 → 1.0, 4–5 → 1.5, 6–7 → 2.5, 8–9 → 3.5, 10 → 4.0.
- **Individual Fluency Rubric** (`individual-assessment/fluency-rubric.md`) and both checklists (`fluency-checklist.md`, `fluency-checklist-technical.md`):
  - **Tier rename**: `Learning → Learner`, `Competent → Practitioner`, `Practitioner → Multiplier`, `Power-User → Champion`. Numeric mapping unchanged (1/2/3/4). Rationale: "Competent" and "Practitioner" had blurred semantics; "Power-User" implied tool intensity rather than strategic capability. "Multiplier" precisely names the Level 3 behavioural shift (amplifying teammates).
- **90-Day Adoption Roadmap** (`roadmap/90-day-adoption-roadmap.md`): Updated all level-name references; updated post-90-day Maturity Stage table to use new MIT CISR stage names and depth-scored thresholds; added explicit handling guidance when a prerequisite gate fires.
- **README.md**: Added branch-variant banner, repository structure updated for new tier names, "How to Use" section updated to explain the 0/1/2 depth scoring mechanic and prerequisite gates.

### Rationale

Client feedback indicated the prior model rated organisations too generously. Root-cause analysis identified two structural problems:

1. **Binary scoring hides depth** — a two-line Slack post and a 20-page board-approved strategy both scored 1.
2. **No prerequisite gates** — averaging across six dimensions allowed strong scores in low-bar dimensions (Culture, Talent) to numerically compensate for missing structural dimensions (Data, Governance), even though MIT CISR research treats those structural dimensions as load-bearing prerequisites.

MIT CISR data confirmed the calibration was off: only 7% of enterprises globally reach Stage 4, but the prior model granted "Leading" at 83% Yes (25/30) — far too accessible. The stage-2-to-3 crossing was treated as a uniform step when MIT CISR data shows it is where growth/profit go from negative to positive — a qualitative inflection.

Changes adopted: depth scoring (B) and prerequisite gates (C). Threshold-raising on top (A) was explicitly rejected — combined with B+C it would be exponentially punishing and eliminate the model's diagnostic utility.

## [0.3.1] - 2026-05-03

### Changed

- **License**: Switched from proprietary to **Apache License 2.0**. Added `NOTICE` file attributing inspiration from the MIT CISR Enterprise AI Maturity Model briefing (Weill, Woerner, and Sebastian, © 2024 MIT Center for Information Systems Research). Updated README license section.

## [0.2.0] - 2026-04-19

### Changed

- **Individual Fluency Rubric** (`individual-assessment/fluency-rubric.md`): Replaced legacy 1–4 Novice/Developing/Proficient/Fluent scale with standard levels **Learning / Competent / Practitioner / Power-User**. Restructured into two parallel tracks (non-technical and technical), each with seven domains, procedural "What good looks like" descriptors, and `Feeds org dimensions:` tags mapping items to MIT CISR dimensions.
- **Non-Technical Fluency Checklist** (`individual-assessment/fluency-checklist.md`): Rebuilt to mirror the non-technical rubric (Foundations, Prompting, Role-Relevant Applications, Strategy & Value, Working With Data, Collaboration & Team Behaviour, Safety & Critical Thinking). Uses per-item Learning / Competent / Practitioner / Power-User tagging.
- **AI Maturity Self-Assessment** (`org-assessment/ai-maturity-self-assessment.md`): Added "Mapping Individual Fluency to MIT CISR AI Maturity Dimensions" and "Scoring From Individual to Organisation" sections, including the aggregation method from individual → team → CISR dimension.
- **90-Day Adoption Roadmap** (`roadmap/90-day-adoption-roadmap.md`): Reframed as root-to-tip (Roots / Trunk / Canopy) with explicit non-mandate principle. Phases renamed to "Seed the Roots", "Grow the Trunk", "Shape the Canopy" with team-by-domain aggregation and CISR scorecard steps.

### Added

- **Technical Fluency Checklist** (`individual-assessment/fluency-checklist-technical.md`): New track-specific checklist mirroring the non-technical checklist structure for engineers, SRE, data/ML, designers, and technical PMs.
## [0.3.0] - 2026-04-19

### Changed

- **License**: Changed from MIT to a proprietary licence held by Dr. Robert Li and Australia GTM. Added `LICENSE` file and updated the README license section. All rights reserved; use, copying, modification, and distribution require prior written consent from the Owners.

## [0.1.0] - 2026-04-16

### Added

- **Individual Assessment**: Fluency checklist and scored rubric for assessing Claude Desktop proficiency (business user profile)
- **Organisation Assessment**: MIT CISR-adapted AI maturity self-assessment with 30 yes/no questions across six dimensions
- **Adoption Templates**:
  - Pilot Program Charter
  - Quarterly Red-Teaming Checklist
  - Victory Journal (daily and weekly)
  - Sprint Demo Agenda
  - Human-in-the-Loop Review Form
  - 30-60-90 Day Success Metrics Dashboard
  - Quarterly OKR Template
- **Tooling Reference**: Curated guide to Claude ecosystem harnesses, skills, plugins, and MCP servers
- **Roadmap**: 90-day organisation-wide adoption framework
- README with usage instructions and repository structure
