# Cycling Sport and Perceived Human Development:
## Exploratory Construction of a Multidimensional Index among Young Cyclists from Bogotá

![Research Status](https://img.shields.io/badge/status-exploratory%20research-blue)
![Language](https://img.shields.io/badge/code-R-blue)
![Field](https://img.shields.io/badge/field-Applied%20Economics%20%7C%20Human%20Development-green)

---

# Overview

This repository contains the complete analytical workflow for the exploratory construction of the **Perceived Human Development Index (PHDI)** among young cyclists participating in an organized cycling sport context in Bogotá, Colombia.

The project examines whether participation in cycling sport is associated with changes in perceived human development dimensions through a multidimensional index approach.

Rather than measuring development exclusively through economic indicators, this project follows a broader human development perspective that incorporates personal, emotional and social dimensions.

The study uses an exploratory **pre-post design** to compare participants' perceived development before and after their participation in a cycling team.

---

# Research Question

**How is participation in organized cycling sport associated with perceived changes in multidimensional human development among young cyclists?**

---

# Research Objective

The objective of this project is to construct and explore a multidimensional indicator capable of capturing perceived changes in human development dimensions within a sport context.

The project focuses on three main dimensions:

1. Psychological Well-being
2. Social Capital
3. Personal Development

---

# Conceptual Framework

The project is based on a multidimensional understanding of human development.

Development is considered not only as an economic outcome, but as an expansion of individuals' capabilities, opportunities and social conditions.

The Perceived Human Development Index (PHDI) operationalizes this perspective by combining personal and social dimensions measured through participant perceptions.

---

# Perceived Human Development Index (PHDI)

The PHDI is an exploratory composite index constructed from three equally weighted dimensions.

The global index is calculated as:

\[
PHDI =
\frac{
Psychological\ Well-being +
Social\ Capital +
Personal\ Development
}{3}
\]

Equal weighting was selected because each dimension represents an independent conceptual component of perceived human development and no empirical basis was available to assign differential weights.

---

# Dimensions and Indicators

## 1. Psychological Well-being

This dimension captures perceived emotional and relational well-being.

Indicators included:

- Joy
- Gratitude
- Tranquility
- Relationships with others
- Care and protection

---

## 2. Social Capital

This dimension captures collective capabilities and social relationships developed within the cycling environment.

Indicators included:

- Teamwork
- Communication
- Leadership
- Respect

---

## 3. Personal Development

This dimension captures perceived individual growth and personal capabilities.

Indicators included:

- Positive attitude and mindset
- Adaptability
- Personal development

---

# Indicator Selection and Measurement Constraints

Indicator selection was constrained by the original survey instrument.

Although autonomy and self-confidence are relevant dimensions in capability-based approaches, they were not included because the questionnaire did not contain direct measures for these constructs.

Therefore, only constructs with direct observable measures in the original survey were incorporated into the PHDI.

---

# Data Description

## Study Context

The study focuses on young cyclists participating in the Kronos MTR cycling team in Bogotá, Colombia.

## Sample

Initial sample:

- 25 participants

Complete paired observations were used for pre-post statistical comparisons after excluding missing values.

---

# Analytical Workflow

The project follows a reproducible analytical pipeline:
PHDI-cycling-human-development/
│
├── Data/
│   ├── raw/
│   └── processed/
│
├── Scripts/
│   ├── 01_data_cleaning.R
│   ├── 02_variable_processing.R
│   ├── 03_PHDI_construction.R
│   ├── 04_descriptive_analysis.R
│   ├── 05_visualization.R
│   ├── 06_statistical_analysis.R
│   └── 07_results_tables.R
│
├── Output/
│   ├── Figures/
│   └── Tables/
│
├── Documentation/
│   └── PHDI_Master_Document.pdf
│
├── Manuscript/
│   └── Article_Draft.pdf
│
└── README.md


---

# Analytical Methods

The analysis included:

## 1. Descriptive Analysis

Comparison of mean scores before and after cycling sport participation.

---

## 2. Normality Assessment

The distribution of individual PHDI differences was evaluated using the Shapiro-Wilk test.

Result:

\[
W=0.985
\]

\[
p=0.969
\]

The distribution of change scores did not show evidence of significant deviation from normality.

---

## 3. Paired Comparison

A paired samples t-test was used to evaluate whether the mean difference between pre and post measurements differed from zero.

Formula:

\[
t=
\frac{\bar d}
{s_d/\sqrt n}
\]

where:

- \(\bar d\) = mean individual difference
- \(s_d\) = standard deviation of differences
- \(n\) = number of paired observations

---

## 4. Robustness Analysis

A Wilcoxon signed-rank test was included as a non-parametric robustness analysis.

---

## 5. Effect Size

The magnitude of change was estimated using paired Cohen's d.

Formula:

\[
d=
\frac{\bar d}{s_d}
\]

Effect size was reported because statistical significance alone does not describe the practical magnitude of observed changes.

---

# Main Results

Among participants with complete pre-post measurements:

\[
n=23
\]

The Perceived Human Development Index increased from:

\[
PHDI_{pre}=3.39
\]

to:

\[
PHDI_{post}=4.13
\]

representing a mean increase of:

\[
\Delta=0.78
\]

---

# Statistical Results

## Paired t-test

\[
t(22)=6.31
\]

\[
p<0.001
\]

95% Confidence Interval:

\[
[0.52,\ 1.03]
\]

---

## Wilcoxon Signed-Rank Test

\[
W=263
\]

\[
p<0.001
\]

---

## Effect Size

Paired Cohen's d:

\[
d=1.32
\]

The observed change represents a large standardized difference between pre and post measurements.

---

# Dimension-Level Results

| Dimension | Pre | Post | Mean Change |
|---|---:|---:|---:|
| Psychological Well-being | 3.35 | 4.15 | +0.79 |
| Social Capital | 3.38 | 4.10 | +0.72 |
| Personal Development | 3.46 | 4.15 | +0.69 |

---

# Dimension-Level Effect Sizes

| Dimension | Cohen's d |
|---|---:|
| Psychological Well-being | 0.93 |
| Social Capital | 1.04 |
| Personal Development | 0.83 |

Social Capital showed the largest standardized change, suggesting the strongest observed improvement relative to participant variability.

---

# Interpretation

The findings indicate that participants reported higher perceived human development scores after cycling sport participation.

However, results should be interpreted as exploratory associations rather than causal effects.

The study design does not allow the conclusion that cycling sport directly caused improvements in human development.

---

# Individual Variation

Although the overall pattern showed increased perceived human development scores, individual trajectories were heterogeneous, including some participants with negative change scores.

This indicates that participants did not experience identical patterns of change.

Future research should investigate factors explaining individual differences, including participation duration, previous experience, social support and personal characteristics.

---

# Limitations

This project has several limitations:

- Small sample size.
- Exploratory pre-post design.
- Absence of a comparison group.
- Self-reported perception measures.
- Limited ability to establish causal relationships.

The results should therefore be interpreted as evidence of perceived changes associated with cycling sport participation.

---

# Reproducibility

All analytical procedures are documented through R scripts.

The repository allows researchers to reproduce:

1. Data preparation.
2. Variable transformation.
3. PHDI construction.
4. Statistical analysis.
5. Visualization.
6. Table generation.

---

# Future Research

Future developments may include:

- Validation of the PHDI with larger samples.
- Confirmatory factor analysis.
- Longitudinal designs.
- Comparison between different sport contexts.
- Inclusion of additional capability-based indicators.

---

# Technologies Used

- R
- tidyverse
- rstatix
- ggplot2
- CSV-based data workflow
- Reproducible research practices

---

# Author

[Your Name]

Research project:
**Cycling Sport and Perceived Human Development: Exploratory Construction of a Multidimensional Index among Young Cyclists from Bogotá**

---

# License

This repository is intended for academic and research purposes.
