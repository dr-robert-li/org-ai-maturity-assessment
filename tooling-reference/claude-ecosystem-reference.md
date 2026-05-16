# Claude Ecosystem Tooling Reference

> **Purpose**: A curated guide to harnesses, skills, plugins, and MCP servers that can accelerate Claude adoption. Each entry describes what it does and who it is for.
>
> **Important**: These tools do not all need to be used together. Pick what you need based on your team's maturity, use cases, and technical comfort. Installing too many skills simultaneously can cause semantic confusion when Claude tries to decide which to invoke. Start lean and add as you grow.

---

## How Claude Extensibility Works

Claude can be extended in several ways:

- **Skills** — Folders of instructions (a `SKILL.md` file plus optional scripts and templates) that Claude loads dynamically to improve performance on specific tasks. Skills teach Claude how to complete tasks in a repeatable way.
- **Plugins** — Installable packages for Claude Code that add commands and workflows.
- **MCP Servers** — Model Context Protocol servers that give Claude access to external tools, APIs, and data sources.
- **Harnesses / Frameworks** — Opinionated development workflows that orchestrate Claude's behaviour across an entire project lifecycle.
- **Prompt Libraries** — Curated sets of prompts and templates for specific domains.

For the official specification on how skills work, see [agentskills.io](https://agentskills.io).

---

## Development Harnesses and Frameworks

### Superpowers

| | |
|---|---|
| **Repository** | [obra/superpowers](https://github.com/obra/superpowers) |
| **What it does** | A complete software development workflow for coding agents. Provides composable skills that trigger automatically — from brainstorming and spec writing through to implementation, testing, code review, and branch management. Enforces test-driven development (RED-GREEN-REFACTOR), systematic debugging, and subagent-driven development where fresh agents work through each task with two-stage review (spec compliance, then code quality). |
| **Best for** | Development teams and technical users who want a structured, opinionated workflow for building software with Claude Code. |
| **Key capabilities** | Brainstorming → spec → implementation plan → subagent execution → code review → branch management. Skills trigger automatically based on context. |
| **Install** | `/plugin install superpowers@claude-plugins-official` (Claude Code) |
| **Technical level** | Developer |

### Get Shit Done (GSD)

| | |
|---|---|
| **Repository** | [gsd-build/get-shit-done](https://github.com/gsd-build/get-shit-done) |
| **What it does** | A lightweight meta-prompting, context engineering, and spec-driven development system. Solves "context rot" — the quality degradation that happens as Claude fills its context window — by breaking projects into small, well-defined tasks, each executed in a fresh 200K-token context window by specialised sub-agents. The main session stays lean while heavy lifting happens in isolated environments. |
| **Best for** | Solo developers and small teams who want consistent quality without enterprise ceremony. Particularly effective for multi-session projects and large codebases. |
| **Key capabilities** | Project initialisation → phased roadmaps → parallel subagent execution → atomic git commits → user acceptance testing → session resume. 22+ commands including `/gsd:new-project`, `/gsd:plan-phase`, `/gsd:execute-phase`, `/gsd:verify-work`. |
| **Install** | `npx get-shit-done-cc --claude --global` or `/plugin install get-shit-done` (Claude Code). Also supports OpenCode, Gemini CLI, Codex, Cursor, Windsurf, and other runtimes. |
| **Technical level** | Developer |

---

## Official Anthropic Resources

### Anthropic Skills Repository

| | |
|---|---|
| **Repository** | [anthropics/skills](https://github.com/anthropics/skills) |
| **What it does** | Anthropic's official collection of skills demonstrating what is possible with Claude's skills system. Includes skills ranging from creative applications (art, music, design) to technical tasks (web app testing, MCP server generation) to enterprise workflows (communications, branding). Also contains the document creation and editing skills (`docx`, `pdf`, `pptx`, `xlsx`) that power Claude's built-in document capabilities. |
| **Best for** | Anyone using Claude. The document skills are particularly relevant for business users. Example skills serve as patterns for creating custom skills. |
| **Key capabilities** | Document skills (Word, PDF, PowerPoint, Excel), creative skills, development skills, enterprise communication skills, plus the official skill template for building your own. |
| **Install** | Already available on paid Claude.ai plans. For Claude Code: `/plugin marketplace add anthropics/skills` then install specific sets. |
| **Technical level** | All levels |

### Claude Cookbooks

| | |
|---|---|
| **Repository** | [anthropics/claude-cookbooks](https://github.com/anthropics/claude-cookbooks) |
| **What it does** | A collection of notebooks and recipes with copy-able code snippets for building with the Claude API. Covers classification, retrieval-augmented generation, summarisation, tool use, multimodal capabilities (vision), sub-agents, PDF handling, automated evaluations, JSON mode, content moderation, and prompt caching. |
| **Best for** | Developers building API integrations. Not directly relevant for business users, but useful for the technical team supporting them. |
| **Key capabilities** | 27.4k+ stars. Jupyter notebooks covering tool use (customer service, SQL, calculator), RAG with vector databases, vision (charts, forms, images), and advanced patterns. |
| **Install** | Clone and run notebooks. Requires a Claude API key. |
| **Technical level** | Developer |

---

## Enterprise and Business Skills

### Enterprise AI Skills

| | |
|---|---|
| **Repository** | [sruthir28/enterprise-ai-skills](https://github.com/sruthir28/enterprise-ai-skills) |
| **What it does** | Open-source AI skills for enterprise professionals, built by a former McKinsey consultant. Includes consulting frameworks (SCPR, Issue Trees, Storyline Builder), decision-making tools (Decision Memo Builder, Prioritisation), meeting preparation, data analysis, and a multi-agent deck pipeline (Strategist → Builder → Critic → Fixer). |
| **Best for** | PMs, consultants, strategists, and ops leaders who want to apply proven frameworks instantly rather than writing prompts from scratch. Highly relevant for RevOps and business operations teams. |
| **Key skills** | SCPR Framework, Decision Memo Builder, Issue Tree Builder, Storyline Builder, Prioritisation (RICE/Impact-Effort), Meeting Prep Kit, AI Use-Case Scorer, Data Insights, McKinsey Critic, Deck Pipeline. |
| **Install** | Download `.skill` files → Claude.ai Settings → Skills → Add Skill. Or clone repo for Claude Code. |
| **Technical level** | Business user / Non-technical |

---

## Scientific and Research Skills

### Claude Scientific Skills

| | |
|---|---|
| **Repository** | [K-Dense-AI/claude-scientific-skills](https://github.com/K-Dense-AI/claude-scientific-skills) |
| **What it does** | 118+ ready-to-use scientific skills that transform Claude into a research assistant. Covers bioinformatics, cheminformatics, proteomics, clinical research, healthcare AI, medical imaging, machine learning, materials science, physics, engineering, data analysis, laboratory automation, and scientific communication. Provides direct API access to 25+ scientific databases (PubMed, ChEMBL, UniProt, COSMIC) and integrations with 50+ Python packages. |
| **Best for** | Research teams, scientists, and healthcare/biotech organisations. Not needed for general business adoption. |
| **Key capabilities** | 118+ skills across 15 scientific domains, 25+ database APIs, 50+ Python package integrations, automatic skill discovery. |
| **Install** | Clone repo or install via MCP server. |
| **Technical level** | Technical / Scientific |

---

## Skill Discovery and Conversion Tools

### Skill Seekers

| | |
|---|---|
| **Repository** | [yusufkaraaslan/Skill_Seekers](https://github.com/yusufkaraaslan/Skill_Seekers) |
| **What it does** | Universal preprocessing layer that converts documentation sites, GitHub repos, PDFs, videos, notebooks, wikis, and 18 other source types into structured AI skills. Outputs to 12 LLM platforms (Claude, Gemini, OpenAI, etc.) and 8 RAG/vector targets (LangChain, LlamaIndex, Pinecone, etc.). Converts days of manual data preparation into 15–45 minutes. |
| **Best for** | Technical teams who need to create custom skills from existing documentation or codebases. Useful when you want to teach Claude about your organisation's specific processes, tools, or domain knowledge. |
| **Key capabilities** | 18 source types → 20+ output targets. Smart SPA discovery, PDF OCR, video transcript extraction, GitHub repository analysis, conflict detection, automatic categorisation. 12.8k+ stars. |
| **Install** | `pip install skill-seekers` |
| **Technical level** | Developer |

---

## Curated Skill Collections

### Awesome Claude Skills (BehiSecc)

| | |
|---|---|
| **Repository** | [BehiSecc/awesome-claude-skills](https://github.com/BehiSecc/awesome-claude-skills) |
| **What it does** | A curated list of Claude skills organised by category: Document Skills, Development & Code Tools, Data & Analysis, Writing & Research, Learning & Knowledge, Media & Content, Collaboration & Project Management, Security & Web Testing, and Utility & Automation. 1.6k+ stars. |
| **Best for** | Anyone looking to discover useful skills across categories. Good starting point for browsing what is available. |

### Awesome Claude Skills (travisvn)

| | |
|---|---|
| **Repository** | [travisvn/awesome-claude-skills](https://github.com/travisvn/awesome-claude-skills) |
| **What it does** | A curated list of Claude Skills, resources, and tools for customising Claude AI workflows, with a focus on Claude Code. |
| **Best for** | Developers looking for Claude Code-specific skills and workflow customisations. |

### Claude Code Skills (daymade)

| | |
|---|---|
| **Repository** | [daymade/claude-code-skills](https://github.com/daymade/claude-code-skills) |
| **What it does** | 48 production-ready skills for Claude Code including a meta-skill for building/validating/packaging custom skills (`skill-creator`), GitHub operations, document conversion, research tools, QA testing, prompt optimisation, and more. Includes skill suites (e.g., `daymade-docs` bundles document-related skills). 847+ stars. |
| **Best for** | Claude Code users who want a broad set of pre-built development and productivity skills. |
| **Install** | `/plugin marketplace add daymade/claude-code-skills` (Claude Code) |
| **Technical level** | Developer |

---

## Marketplace

### SkillsMP (Agent Skills Marketplace)

| | |
|---|---|
| **URL** | [skillsmp.com](https://skillsmp.com/) |
| **What it does** | A marketplace with 25,000+ agent skills compatible with Claude Code, Codex CLI, and ChatGPT. Skills follow the open-standard `SKILL.md` format. Browse, search, and install skills directly. |
| **Best for** | Anyone looking for a specific skill. Searchable directory covering every domain. |
| **Technical level** | All levels (for browsing); Developer (for installation) |

### Tessl Registry

| | |
|---|---|
| **URL** | [tessl.io/registry](https://tessl.io/registry) |
| **What it does** | A skill-specific package manager and discovery platform for agent skills. Unlike browsing GitHub — which is general-purpose and gives no signal beyond stars and a README — Tessl treats each skill as a versioned package with automated evaluations (quality, impact uplift vs. baseline, and Snyk-powered security scanning) on every publish. Versioning lets developers pin to specific releases and update intentionally, rather than tracking a moving `main` branch. Skills can be installed via CLI, e.g., `npx tessl i github:<owner>/<repo> --skill <name>`. |
| **Best for** | Teams that need reproducible, evaluated skill installs rather than ad-hoc GitHub clones. Useful when you want signal on whether a skill actually improves agent behaviour, and when version stability across environments matters. |
| **Technical level** | Developer |

---

## Choosing the Right Tools

### For Non-Technical Business Users (RevOps, Operations, Analysts)

Start here:
1. **Anthropic Skills** (already built into Claude.ai) — document creation, editing
2. **Enterprise AI Skills** — consulting frameworks, meeting prep, data insights
3. **SkillsMP** — browse for domain-specific skills

### For Technical Teams Supporting Adoption

Add:
4. **Claude Cookbooks** — reference patterns for API integrations
5. **Skill Seekers** — convert your internal documentation into custom skills
6. **Awesome Claude Skills lists** — discover community-built skills

### For Development Teams

Add:
7. **Superpowers** or **GSD** (pick one, not both — they are opinionated workflows that may conflict)
8. **Claude Code Skills (daymade)** — broad set of development-oriented skills

### Anti-Patterns to Avoid

- **Do not install multiple competing harnesses** (e.g., Superpowers + GSD). They have overlapping triggers that will confuse skill selection.
- **Do not install dozens of skills at once.** Start with 2–3, build fluency, then add more. Too many skills create semantic confusion — Claude may invoke the wrong one or none at all.
- **Do not assume non-technical users need developer tools.** Claude.ai with built-in skills and a few enterprise skill files covers most business use cases without any CLI or plugin installation.
