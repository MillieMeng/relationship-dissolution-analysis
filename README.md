# Relationship Dissolution & Social Cognition Analysis

## Overview

This independent social cognition project examines psychological adjustment following relationship dissolution ("ghosting"). It combines a quantitative survey of **119 participants** with qualitative interviews from **19 participants** to investigate the role of rumination, self-attribution bias, and trust erosion in post-dissolution adjustment.

The repository is designed as a reproducible, privacy-conscious research portfolio. Raw participant data are excluded; the analysis notebook defaults to a simulated dataset with the same structure.

---

## Verified quantitative findings

### Sample demographics (N = 119)
- **Gender:** Female 52.1% (n = 62), Male 46.2% (n = 55), Undisclosed 1.7% (n = 2)
- **Age:** 47.1% aged 21–25; 28.6% aged 15–20; 17.6% aged 26–30
- **Experienced ghosting:** 97.5% (n = 116 of 119)

### Ghosting experience
| Duration | n | % |
|---|---|---|
| Resolved within days | 38 | 32.8% |
| 1–4 weeks | 38 | 32.8% |
| 2–6 months | 21 | 18.1% |
| 6+ months | 8 | 6.9% |
| Never reconnected | 11 | 9.5% |

### Psychometric scale (0–5 Likert, n = 116)
| Item | M | SD |
|---|---|---|
| Confusion & disorientation (断联初期，我感到强烈的不解与困惑) | 3.49 | 1.40 |
| Rumination / self-blame (我曾反复反思自己是否做错了什么) | 3.66 | 1.56 |
| Self-worth doubt (这段经历让我怀疑自己的价值) | 3.35 | 1.40 |
| Trust erosion (我对他人的信任感明显降低) | 3.19 | 1.26 |
| **Total score** | **13.34** | **5.29** |

All four items scored significantly above the scale midpoint (2.5).

### Reliability & factorial validity
- **Cronbach's α = .891** (high internal consistency)
- **KMO = .812** (meritorious sampling adequacy; Bartlett's test *p* < .001)
- Inter-item correlations range from *r* = .549 to *r* = .773 (all *p* < .001)

### Key inferential findings
- **Self-attribution prevalence:** 62.9% of participants scored ≥ 4 on rumination; 59.5% on self-worth doubt — consistent with a dominant internal attribution pattern following ambiguous rejection.
- **Duration effect:** Pearson correlations between ghosting duration (ordinal) and all four scale items were non-significant (*r*s = −.038 to −.105, all *p* > .26), suggesting the psychological impact does not diminish proportionally with time.
- **Gender differences:** No significant gender differences on rumination or self-worth doubt (*p*s > .39), indicating the self-attribution pattern is consistent across gender.

### Perceived causes & coping (multi-select; n = 116)
Top attributed causes: emotional detachment (62.1%), conflict avoidance (57.8%), personal psychological issues (45.7%), new relationship (36.2%).  
Top coping strategies: actively seeking explanation (57.8%), confiding in friends (54.3%), work/study distraction (46.6%), counselling (27.6%).

### Lasting impact & attitudes
- **73.3%** reported lasting effects: more cautious/sensitive (49.1%) or difficulty entering new relationships (24.1%).
- **69.0%** view ghosting as "absolutely unacceptable"; 26.7% as "understandable in specific contexts."
- **30.2%** (n = 35) reported having ghosted someone themselves; of those, 65.7% reported mild or strong guilt.

---

## Research questions

1. How is attachment anxiety related to rumination following relationship dissolution?
2. Do the study scales demonstrate adequate reliability and factorability?
3. Which social-cognitive and emotional variables are associated with post-dissolution adjustment?
4. How do interview themes contextualize the quantitative patterns?

---

## Methods

**Quantitative phase (N = 119):** Psychometric survey measuring confusion, rumination, self-worth doubt, and trust erosion on a 0–5 Likert scale, deployed via WeChat. Additional items measured ghosting duration, perceived causes, coping strategies, lasting impact, and attitude toward ghosting.

**Qualitative phase (n = 19):** Semi-structured interviews modelling the phenomenological transition from situational curiosity to dispositional self-doubt, coded thematically into three stages: Signal Search → Narrative Construction → Internalization.

**Data pipeline:** Cleaning, reliability analysis, EFA, ANOVA, and visualization in R (dplyr, ggplot2, psych). Descriptive and correlational analyses cross-validated in Python (pandas, scipy).

---

## Data availability and ethics

**The real raw data are not public.** Survey responses and interview materials contain confidential participant information and are excluded from this repository. The analysis notebook defaults to a reproducible simulated dataset with the same broad variable structure.

Anyone adapting this repository should place authorized local data in a non-versioned `data/` directory and confirm that sharing and analysis comply with the relevant consent, ethics, and data-governance requirements.

---

## Reproduce the template

1. Install R and RStudio.
2. Open `analysis.Rmd`.
3. Install packages listed in the setup chunk.
4. Keep `use_simulated_data <- TRUE` for the public demonstration.
5. Knit or run chunks interactively.

To use authorized real data locally, set `use_simulated_data <- FALSE` and add `data/relationship_dissolution_data.csv` with columns matching the codebook.

---

## Repository structure

```text
relationship-dissolution-analysis/
├── README.md              # Project overview and verified findings
├── analysis.Rmd           # Reproducible R workflow
├── codebook.md            # Variable schema and verification checklist
├── LICENSE                # MIT license for code and documentation
├── .gitignore             # Excludes private data and generated files
├── figures/
│   └── .gitkeep
└── results/
    └── .gitkeep
```

---

## Skills demonstrated

R · Python · R Markdown · psychometric reliability · KMO/EFA · correlation analysis · data visualization · mixed-methods research design · privacy-conscious data handling · reproducible research

---

## License

Code and documentation are available under the MIT License. This license does **not** apply to participant data, interview materials, instruments, or third-party content.
