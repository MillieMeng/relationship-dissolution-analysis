# 🧠 Social Cognition — Mixed-Methods Analysis of Relationship Dissolution

[![R](https://img.shields.io/badge/R-tidyverse%20%7C%20psych-276DC3?style=flat-square&logo=r&logoColor=white)](https://github.com/MillieMeng/relationship-dissolution-analysis)
[![Method](https://img.shields.io/badge/Method-Mixed%20Methods-9b59b6?style=flat-square)](https://github.com/MillieMeng/relationship-dissolution-analysis)
[![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=flat-square)](https://github.com/MillieMeng/relationship-dissolution-analysis)

## Overview

Independent social cognition study examining psychological adjustment following "ghosting" — a form of relationship dissolution with no explicit communication. Combines a quantitative psychometric survey with qualitative interviews to identify key patterns in rumination, self-attribution, and trust erosion.

**Sample:** Survey N = 119 · Qualitative interviews n = 19 · Data collected via WeChat

> Raw participant data are excluded for privacy. The analysis notebook runs on a reproducible simulated dataset by default.

---

## Business Question

> What psychological mechanisms drive post-dissolution adjustment, and can they be reliably measured across a general population sample?

---

## Method

**Quantitative Phase (N = 119)**
Psychometric survey measuring four dimensions on a 0–5 Likert scale: confusion/disorientation, rumination/self-blame, self-worth doubt, and trust erosion. Additional items captured ghosting duration, perceived causes, coping strategies, and lasting impact.

**Qualitative Phase (n = 19)**
Semi-structured interviews coded thematically into three stages: Signal Search → Narrative Construction → Internalization.

**Analysis Pipeline (R)**
Data cleaning, reliability analysis (Cronbach's α, KMO/Bartlett), EFA, ANOVA, correlation analysis, and visualization using `dplyr`, `ggplot2`, and `psych`. Descriptive and correlational analyses cross-validated in Python (`pandas`, `scipy`).

---

## Results

**Scale Reliability:** Cronbach's α = .891 (high internal consistency); KMO = .812 (meritorious sampling adequacy); Bartlett's test p < .001. Inter-item correlations ranged from r = .549 to r = .773.

**Self-Attribution Prevalence:** 62.9% scored ≥ 4 on rumination; 59.5% on self-worth doubt — consistent with a dominant internal attribution pattern following ambiguous rejection.

**Duration Effect:** Pearson correlations between ghosting duration and all four scale items were non-significant (rs = −.038 to −.105, all p > .26), suggesting psychological impact does not diminish proportionally with time.

**Gender Differences:** No significant differences on rumination or self-worth doubt across gender (ps > .39), indicating the self-attribution pattern is consistent.

**Lasting Impact:** 73.3% reported lasting effects — 49.1% became more cautious or sensitive; 24.1% reported difficulty entering new relationships.

| Scale Item | M | SD |
|---|---|---|
| Confusion & disorientation | 3.49 | 1.40 |
| Rumination / self-blame | 3.66 | 1.56 |
| Self-worth doubt | 3.35 | 1.40 |
| Trust erosion | 3.19 | 1.26 |

All four items scored significantly above the scale midpoint (2.5).

---

## Skills

| Domain | Tools & Methods |
|---|---|
| **Statistical Analysis** | EFA · Cronbach's α · KMO/Bartlett · Pearson correlation · ANOVA |
| **R** | `dplyr` · `ggplot2` · `psych` · `RMarkdown` |
| **Python** | `pandas` · `scipy` |
| **Research Design** | Mixed-methods · psychometric scale construction · privacy-conscious data handling |
| **Reporting** | Reproducible workflow · simulated data · stakeholder findings report |
