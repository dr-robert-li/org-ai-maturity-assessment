# AI Maturity Self-Assessment

> **Purpose**: Assess your organisation's overall readiness and maturity for AI adoption across six dimensions. Stage names follow the [MIT CISR Enterprise AI Maturity Model](https://cisr.mit.edu/publication/2024_1201_EnterpriseAIMaturityModel_WeillWoernerSebastian) (Weill, Woerner, and Sebastian, © 2024 MIT Center for Information Systems Research).
>
> **How to use**: Score each question 0 / 1 / 2 using the depth-scoring key below. Sum scores for an overall maturity score (max 60). For best results, conduct this as a listening tour — interview 5–10 people across departments and aggregate responses. Questions can be modified to suit your organisation and specific AI offerings.
>
> **About this variant**: This is the **stricter-scoring variant** of the assessment. Compared to the binary Yes/No baseline, it adds (a) three-point depth scoring per question and (b) prerequisite gates on Data Infrastructure and Governance dimensions to prevent strong soft-dimension scores from masking structural gaps. See [CHANGELOG.md](../CHANGELOG.md) for the rationale.

---

## Depth Scoring Key

Use this scale for every question below. The "Partial" middle score is what makes this assessment honest — most real-world capabilities are partial, not fully evidenced.

| Score | Response | Description |
|:-----:|----------|-------------|
| **0** | **No** | Not in place. Either does not exist, or only exists as an aspiration / talking point. |
| **1** | **Partial** | Exists but is inconsistent, undocumented, scoped to a single team, or recently introduced without proven adoption. |
| **2** | **Yes — Evidenced** | Documented, consistently practised across the relevant scope, and someone outside the originating team could point to concrete artefacts (policy doc, dashboard, working pipeline, signed-off training, etc.). |

**Calibration rule of thumb**: If your first instinct is "yes, but…", the answer is **1 (Partial)**.

---

## Strategy and Vision

| # | Question | Score (0–2) |
|:-:|----------|:-----------:|
| 1 | Is there a written AI vision or strategy aligned with overall business objectives? | |
| 2 | Have high-value AI use cases supporting key goals been identified? | |
| 3 | Does executive leadership actively support and sponsor AI initiatives? | |
| 4 | Are there clear, quantified success metrics for AI projects? | |
| 5 | Is there a realistic, phased roadmap for AI adoption and scaling? | |

## Data Infrastructure

| # | Question | Score (0–2) |
|:-:|----------|:-----------:|
| 6 | Is quality, fit-for-purpose data readily available for critical AI use cases? | |
| 7 | Are core data sources consolidated rather than siloed across teams? | |
| 8 | Does the organisation follow formal data governance and stewardship policies? | |
| 9 | Are data privacy and security controls consistently enforced? | |
| 10 | Is there a standardised process for keeping data clean, well-structured, and up to date? | |

## Technology and Infrastructure

| # | Question | Score (0–2) |
|:-:|----------|:-----------:|
| 11 | Is current IT infrastructure (on-prem/cloud) technically equipped to run AI/ML workloads? | |
| 12 | Does the organisation leverage cloud or hybrid platforms for scalable AI resource needs? | |
| 13 | Can AI tools integrate smoothly with existing core business systems? | |
| 14 | Are there sufficient computing resources and storage for current and planned AI projects? | |
| 15 | Is the security architecture robust and regularly reviewed as AI scales? | |

## Talent and Skills

| # | Question | Score (0–2) |
|:-:|----------|:-----------:|
| 16 | Do most employees have a basic understanding of AI concepts and opportunities? | |
| 17 | Is there sufficient in-house expertise in data science, ML, or AI engineering? | |
| 18 | Are employees encouraged and willing to acquire AI-related skills? | |
| 19 | Does the organisation have or plan formal AI upskilling/training programs? | |
| 20 | Has a hiring or external consulting strategy addressed core AI skill gaps? | |

## Governance and Ethics

| # | Question | Score (0–2) |
|:-:|----------|:-----------:|
| 21 | Are responsibilities and frameworks for AI governance established and documented? | |
| 22 | Does the organisation have published AI ethical guidelines or principles? | |
| 23 | Are risk management and regulatory requirements assessed for each AI initiative? | |
| 24 | Are there checks in place for bias, fairness, and transparency in AI outputs? | |
| 25 | Can AI-driven decisions be clearly explained to non-technical stakeholders? | |

## Organisational Culture

| # | Question | Score (0–2) |
|:-:|----------|:-----------:|
| 26 | Does leadership promote innovation and calculated risk-taking with AI? | |
| 27 | Are teams open and responsive to change driven by new technology? | |
| 28 | Is there an organisational willingness to learn from failed or suboptimal AI projects? | |
| 29 | Do different departments actively collaborate on AI initiatives? | |
| 30 | Do employees tend to view AI as an opportunity, not a threat, for the business? | |

---

## Scoring

### Overall Score → Stage

Stage names follow the MIT CISR Enterprise AI Maturity Model. Bands are intentionally **asymmetric** — the Stage 2 → Stage 3 crossing is the widest, reflecting MIT CISR's empirical finding that this transition is the hardest and most consequential (it is where growth and profit move from negative to positive).

| Score (0–60) | Stage | % of Enterprises (MIT CISR 2024) | Description |
|:-----------:|------|:--------------------------------:|-------------|
| **0–20** | **Stage 1: Experiment and Prepare** | 28% | Exploration and education. AI is exploratory; focus on educating the workforce, setting acceptable-use policies, making data accessible, and identifying where humans need to remain in the loop. |
| **21–38** | **Stage 2: Build Pilots and Capabilities** | 34% | Business cases and pilots. Beginning to simplify and automate processes, creating use cases, sharing data via APIs, and using LLMs to augment work. *Still in net-investment phase — growth/profit typically negative.* |
| **39–52** | **Stage 3: Develop AI Ways of Working** | 31% | Scaling AI platforms and dashboards. Expanding process automation, test-and-learn working style, architecting for reuse, incorporating pretrained models, exploring autonomous agents. *Inflection point — growth and profit turn positive.* |
| **53–60** | **Stage 4: AI Future Ready** | 7% | Continuous innovation and new revenue streams. AI embedded into decision-making and processes; creating and selling AI-augmented business services; combining traditional, generative, agentic, and robotic AI. |

> **Why the bands are uneven**: MIT CISR data shows Stage 1 and Stage 2 enterprises run *negative* growth and profit (investment phase), Stage 3 produces +11.3pp growth / +8.7pp profit, Stage 4 produces +17.1pp / +10.4pp. The model treats Stage 2 → Stage 3 as the hardest crossing because the data says it is.

### Prerequisite Gates

Total score alone does not determine stage. Two gates apply:

#### Gate 1 — Cannot reach Stage 3 without baseline Data Infrastructure and Governance

A high-Culture, low-Data org can numerically score into Stage 3 territory while being structurally incapable of operating there. The gate prevents this.

To be classified as **Stage 3: Develop AI Ways of Working** or higher, BOTH must hold:

- **Data Infrastructure** dimension score ≥ **4 / 10**
- **Governance and Ethics** dimension score ≥ **4 / 10**

If either fails, overall score is **capped at 38** (top of Stage 2) regardless of total.

#### Gate 2 — Cannot reach Stage 4 without uniform Stage 3 strength

To be classified as **Stage 4: AI Future Ready**, ALL six dimensions must score ≥ **7 / 10**.

If any dimension falls short, overall score is **capped at 52** (top of Stage 3).

#### Reporting Gate Outcomes

When a gate fires, name it explicitly in the report:

```
⚠ Stage gate blocked: Data Infrastructure (3/10) — minimum 4/10 required to reach Stage 3.
  Raw score: 41 → Capped at Stage 2: Build Pilots and Capabilities.
  Recommendation: Close the Data Infrastructure gap before scaling AI ways of working.
```

This makes the structural blocker visible to stakeholders rather than burying it in a smoothed average.

---

## Summary Worksheet

| Dimension | Score | / Total |
|-----------|:-----:|:-------:|
| Strategy and Vision | | / 10 |
| Data Infrastructure | | / 10 |
| Technology and Infrastructure | | / 10 |
| Talent and Skills | | / 10 |
| Governance and Ethics | | / 10 |
| Organisational Culture | | / 10 |
| **Raw Total** | | **/ 60** |
| **Gate Adjustments** | | |
| **Final Score** | | **/ 60** |

**Stage**: _______________

**Gate Outcomes** (note any caps applied): _______________

---

## Assessment Notes

```
[Date]:
[Assessor]:
[Organisation]:
[Interviewees]:

Key Findings:



Strongest Dimensions:



Weakest Dimensions:



Gate Status (Data ≥ 4? Governance ≥ 4? All dimensions ≥ 7?):



Recommended Focus Areas:


```

---

## Mapping Individual Fluency to MIT CISR AI Maturity Dimensions

The [Individual Fluency Rubric](../individual-assessment/fluency-rubric.md) and its two checklists (non-technical and technical) feed directly into this org-level assessment. Use the mapping below to aggregate individual domain scores into the six CISR-aligned dimensions above.

> **Note on naming**: The six dimensions in this document (Strategy and Vision, Data Infrastructure, Technology and Infrastructure, Talent and Skills, Governance and Ethics, Organisational Culture) follow MIT CISR's framework. The rubric uses slightly shorter labels (e.g. "Strategy & Use Cases", "Data", "Technology & Infrastructure", "Talent & Culture", "Governance") that map 1:1.

### Domain → CISR Dimension Mapping

| Individual Fluency Domain (Non-Tech / Tech) | Primary CISR Dimension(s) |
|---------------------------------------------|---------------------------|
| Foundations — Basic Usage (both tracks) | Talent and Skills |
| Prompting & Communication (non-tech) / Prompting & Problem Decomposition (tech) | Talent and Skills |
| Role-Relevant Applications (non-tech) | Talent and Skills; Strategy and Vision |
| Code & System Integration (tech) | Technology and Infrastructure; Data Infrastructure |
| Strategy & Value in My Role (both tracks) | Strategy and Vision; Talent and Skills |
| Working With Data (both tracks) | Data Infrastructure; Technology and Infrastructure |
| Collaboration & Team Behaviour (non-tech) / Collaboration, Documentation & Review (tech) | Talent and Skills; Organisational Culture; Governance and Ethics |
| Safety & Critical Thinking (non-tech) | Governance and Ethics |
| Safety, Testing & Observability (tech) | Governance and Ethics; Technology and Infrastructure |

Each rubric item in [fluency-rubric.md](../individual-assessment/fluency-rubric.md) also carries a `Feeds org dimensions:` tag for finer-grained aggregation.

---

## Scoring From Individual to Organisation

This section explains how to combine individual rubric/checklist scores with the org-level depth scores above.

### 1. Numeric mapping for individual levels

| Level | Score |
|-------|:-----:|
| Learner | 1 |
| Practitioner | 2 |
| Multiplier | 3 |
| Champion | 4 |

### 2. Per-person domain scores

For each person assessed:

- For each domain in their track (non-technical or technical), calculate the average level across the checklist items in that domain.
- Record an overall average across domains.

### 3. Team / function aggregates

For each team or function:

- Average individuals' domain scores within the team.
- Note which domains sit below ~2.0 (structural gap) or above ~3.0 (team strength).

### 4. Org-level aggregation into CISR dimensions

For each CISR dimension:

1. Use the Domain → CISR mapping above to collect the relevant domain scores from all assessed individuals.
2. Average them to get an individual-side CISR score (on a 1–4 scale).
3. Convert the dimension's depth-scored total (0–10) into a 1–4 scale using:

| Dimension Score (0–10) | 1–4 Equivalent |
|:----------------------:|:--------------:|
| 0–3 | 1.0 |
| 4–5 | 1.5 |
| 6–7 | 2.5 |
| 8–9 | 3.5 |
| 10 | 4.0 |

4. Take a weighted average of the individual-side score and the org-side score (default 50/50; weight individual-side higher when many people have been assessed, org-side higher when only a few have).

The result is a combined CISR dimension score (1–4) that reflects both bottom-up behaviour and top-down structure.

### 5. Interpreting combined CISR scores (per dimension)

| Combined Score | Stage Equivalent | Implication |
|:--------------:|------------------|-------------|
| **1.0–1.4** | **Experiment and Prepare** | Dimension is underdeveloped both in practice and structure. Focus on awareness, basic enablement, and first use cases. |
| **1.5–2.4** | **Build Pilots and Capabilities** | Dimension has pockets of activity; formalise what exists and close the biggest gap in the next 90 days. |
| **2.5–3.4** | **Develop AI Ways of Working** | Dimension is working across multiple teams; focus on consistency and scaling. |
| **3.5–4.0** | **AI Future Ready** | Dimension is a strength; leverage it to pull weaker dimensions up and drive strategic differentiation. |

Use these combined scores to prioritise investment in the [90-Day Adoption Roadmap](../roadmap/90-day-adoption-roadmap.md).

---

## Dimension-by-Dimension Recommendations

Use this guide to translate dimension scores into action.

| Dimension Score (0–10) | Recommended Actions |
|:---------------------:|---------------------|
| **0–3** | Critical gap. Start with awareness — educate leadership and key stakeholders on why this dimension matters. Assign ownership. Dimension is at Stage 1 equivalent. |
| **4–5** | Foundations forming. Formalise what exists (document informal practices, create policies from habits). Set 90-day improvement targets. Dimension is at Stage 2 equivalent. **If this is Data or Governance, you are also blocking Stage 3 progress at the org level.** |
| **6–7** | Developing well. Focus on consistency — ensure practices are applied uniformly, not just by early adopters. Dimension is at Stage 3 equivalent. |
| **8–9** | Strong. Use as an organisational strength to accelerate weaker dimensions. **Note: must reach 10 to satisfy the Stage 4 gate.** |
| **10** | Fully evidenced. Maintain practice and contribute to external benchmarking / community of practice. |
