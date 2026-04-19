# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

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
