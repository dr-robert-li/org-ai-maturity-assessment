# Organisational AI Maturity Assessment & Adoption Toolkit

A comprehensive set of documentation, frameworks, and tools to help organisations develop fluency in — and adopt — AI tooling as quickly as possible. Largely centred on the **Anthropic Claude** ecosystem, though the assessment frameworks are platform-agnostic.

## Who Is This For?

- **AI consultants and engineers** running adoption engagements
- **RevOps, operations, and business teams** building fluency with Claude
- **Internal champions** driving AI adoption across their organisation
- **Team leads and managers** responsible for upskilling their people

## Repository Structure

```
├── individual-assessment/       # Individual fluency rubric and checklist
│   ├── fluency-checklist.md     # Tick-box checklist for assessing individual Claude fluency
│   └── fluency-rubric.md        # Scored rubric (1–4) across five dimensions
│
├── org-assessment/              # Organisation-wide maturity assessment
│   └── ai-maturity-self-assessment.md   # MIT CISR framework — 30 yes/no questions
│
├── adoption-templates/          # Ready-to-use templates for running adoption programs
│   ├── pilot-program-charter.md         # Structured charter for AI pilot projects
│   ├── quarterly-red-teaming-checklist.md  # Quarterly safety and testing cadence
│   ├── victory-journal.md               # Daily and weekly victory tracking
│   ├── sprint-demo-agenda.md            # Sprint demo format for AI project reviews
│   ├── human-in-the-loop-review.md      # Review form for AI-assisted outputs
│   ├── success-metrics-dashboard.md     # 30-60-90 day metrics tracking
│   └── quarterly-okr-template.md        # OKR template for AI adoption goals
│
├── tooling-reference/           # Canonical harnesses, skills, plugins, and MCP servers
│   └── claude-ecosystem-reference.md    # Curated guide to Claude skills and tooling
│
├── roadmap/                     # Adoption roadmap frameworks
│   └── 90-day-adoption-roadmap.md       # Phased framework for org-wide AI adoption
│
├── CHANGELOG.md
└── README.md
```

## How to Use This Repository

### For Individual Assessment

Start with `individual-assessment/fluency-checklist.md` to tick off what the person is already doing. Then score them using `individual-assessment/fluency-rubric.md` to identify specific gaps and generate targeted recommendations.

### For Organisation-Wide Assessment

Use `org-assessment/ai-maturity-self-assessment.md` to survey the organisation across six dimensions. This is best done as a listening tour — interview 5–10 people across departments and aggregate scores.

### For Running an Adoption Program

1. Use the **90-Day Adoption Roadmap** (`roadmap/90-day-adoption-roadmap.md`) as the master plan
2. Pull in **Adoption Templates** as needed for specific activities (pilots, reviews, demos)
3. Reference the **Tooling Guide** (`tooling-reference/claude-ecosystem-reference.md`) when recommending specific Claude skills, plugins, and integrations

### For Non-Technical Users

All files are in Markdown format. They can be:
- Viewed directly on GitHub
- Downloaded and opened in any text editor
- Printed from GitHub (use the print button on any `.md` file)
- Copied into Google Docs, Notion, or any other documentation tool
- Converted to PDF using any Markdown-to-PDF converter

## Source Attribution

- **Individual Fluency Rubric**: Developed by [Dr. Robert Li](https://drli.blog) for Claude Desktop business user assessment
- **Organisation Maturity Assessment**: Adapted from the [MIT CISR AI Maturity Framework](https://cisr.mit.edu/) as described in [Emerging Practices in Team Building for an Agentic Internet](https://drli.blog/posts/emerging-practices-3t-team/)
- **Adoption Templates**: From Section F of [Emerging Practices in Team Building for an Agentic Internet](https://drli.blog/posts/emerging-practices-3t-team/)
- **Tooling References**: Community-maintained open-source repositories (individually attributed in the tooling guide)

## License

MIT — use freely, modify, and share. Attribution appreciated.
