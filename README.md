# Cycling Sport and Perceived Human Development:
## Exploratory Construction of a Multidimensional Index among Young Cyclists from Bogotá

![Research Status](https://img.shields.io/badge/status-exploratory%20research-blue)
![Language](https://img.shields.io/badge/code-R-blue)
![Field](https://img.shields.io/badge/field-Applied%20Economics%20%7C%20Human%20Development-green)

---

# Overview

This repository contains the analytical workflow developed for the exploratory construction of the **Perceived Human Development Index (PHDI)** among young cyclists participating in an organized cycling sport context in Bogotá, Colombia.

The project examines whether participation in cycling sport is associated with changes in perceived human development dimensions through a multidimensional index approach.

Rather than considering development exclusively through economic indicators, this project follows a broader human development perspective that incorporates personal, emotional and social dimensions.

The study follows an exploratory **pre-post design**, comparing participants' perceived development before and after participation in a cycling team.

---

# Research Question

**How is participation in organized cycling sport associated with perceived changes in multidimensional human development among young cyclists?**

---

# Research Objective

The objective of this project is to construct and explore a multidimensional indicator capable of capturing perceived changes in human development dimensions within a sport context.

The analysis focuses on three dimensions:

1. Psychological Well-being  
2. Social Capital  
3. Personal Development  

---

# Conceptual Framework

Human development is understood as a multidimensional process that extends beyond economic outcomes.

The project follows a capability-oriented perspective, considering that development includes:

- personal capacities,
- emotional well-being,
- social relationships,
- opportunities for individual growth.

The **Perceived Human Development Index (PHDI)** was created as an exploratory measure to operationalize these dimensions within an organized cycling sport environment.

---

# Perceived Human Development Index (PHDI)

The PHDI is a composite index constructed from three equally weighted dimensions:

- Psychological Well-being
- Social Capital
- Personal Development

The global index is calculated as:

$$
PHDI=\frac{Psychological\ Well-being + Social\ Capital + Personal\ Development}{3}
$$

Equal weighting was selected because each dimension represents an independent conceptual component of perceived human development, and no empirical basis was available for assigning different weights.

---

# Dimensions and Indicators

## Psychological Well-being

This dimension captures perceived emotional and relational well-being.

Indicators:

- Joy
- Gratitude
- Tranquility
- Relationships with others
- Care and protection

---

## Social Capital

This dimension captures collective capabilities and social relationships developed within the cycling environment.

Indicators:

- Teamwork
- Communication
- Leadership
- Respect

---

## Personal Development

This dimension captures perceived individual growth and personal capabilities.

Indicators:

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

Participants were young cyclists belonging to the Kronos MTR cycling team in Bogotá, Colombia.

## Sample

| Description | Value |
|---|---:|
| Initial participants | 25 |
| Complete paired observations | 23 |

Statistical comparisons were performed using available complete pre-post measurements.

---

# Analytical Workflow

The project follows a reproducible research pipeline:
Raw survey data
        |
        v
Data cleaning
        |
        v
Variable transformation
        |
        v
PHDI construction
        |
        v
Descriptive analysis
        |
        v
Statistical testing
        |
        v
Visualization
        |
        v
Research outputs

---
PHDI-cycling-human-development/
│
├── Data/
│   ├── raw/
│   └── processed/
│
├── Scripts/
│   ├── Data preparation
│   ├── PHDI construction
│   ├── Visualization
│   ├── Statistical analysis
│   └── Results tables
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

# Statistical Methods

## Descriptive Analysis

Mean scores were calculated before and after cycling sport participation.

---

## Change Score

Individual change was calculated as:

$$
Change=PHDI_{post}-PHDI_{pre}
$$

Positive values indicate higher perceived human development scores after participation.

---

## Normality Assessment

The distribution of individual PHDI differences was evaluated using the Shapiro-Wilk test.

| Test | Result |
|---|---:|
| W | 0.985 |
| p-value | 0.969 |

The distribution of change scores did not show evidence of significant deviation from normality.

---

## Paired Comparison

A paired samples t-test was used to evaluate whether the average pre-post difference differed from zero.

Formula:

$$
t=\frac{\bar d}{s_d/\sqrt n}
$$

Where:

- $\bar d$ = mean difference
- $s_d$ = standard deviation of differences
- $n$ = paired observations

---

## Robustness Analysis

A Wilcoxon signed-rank test was included as a non-parametric robustness assessment.

---

## Effect Size

The magnitude of change was estimated using paired Cohen's d.

$$
d=\frac{\bar d}{s_d}
$$

Effect size was included because statistical significance alone does not describe the magnitude of observed changes.

---

# Main Results

Among participants with complete pre-post measurements:

**n = 23**

The Perceived Human Development Index increased from:

**3.39 before participation**

to:

**4.13 after participation**

representing a mean increase of:

**+0.78 points**

---

# Statistical Results

| Analysis | Result |
|---|---:|
| Paired t-test | t(22)=6.31 |
| p-value | <0.001 |
| 95% Confidence Interval | 0.52 to 1.03 |
| Wilcoxon signed-rank | W=263 |
| Wilcoxon p-value | <0.001 |
| Cohen's d | 1.32 |

---

# Dimension-Level Results

| Dimension | Before | After | Mean Change |
|---|---:|---:|---:|
| Psychological Well-being | 3.35 | 4.15 | +0.79 |
| Social Capital | 3.38 | 4.10 | +0.72 |
| Personal Development | 3.46 | 4.15 | +0.69 |

---

# Dimension Effect Sizes

| Dimension | Cohen's d |
|---|---:|
| Psychological Well-being | 0.93 |
| Social Capital | 1.04 |
| Personal Development | 0.83 |

Social Capital showed the largest standardized change, indicating the strongest observed change relative to participant variability.

---

# Interpretation of Findings

The findings indicate that participants reported higher perceived human development scores after cycling sport participation.

However, these findings should be interpreted as exploratory associations rather than causal effects.

The study design does not allow the conclusion that cycling sport directly caused improvements in human development.

---

# Individual Variation

Although the overall pattern showed increased perceived human development scores, individual trajectories were heterogeneous, including some participants with negative change scores.

This indicates that participants did not experience identical patterns of change.

Future research should investigate factors that explain these differences, including:

- participation duration,
- previous experience,
- social support,
- individual characteristics.

---

# Limitations

This project should be interpreted considering:

- exploratory design;
- small sample size;
- absence of comparison group;
- self-reported measures;
- limited causal inference.

The results represent perceived changes associated with cycling sport participation.

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

Future extensions may include:

- validation of the PHDI with larger samples;
- confirmatory factor analysis;
- longitudinal studies;
- comparison across sport contexts;
- inclusion of additional capability-based indicators.

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

**[Your Name]**

Research Project:

**Cycling Sport and Perceived Human Development: Exploratory Construction of a Multidimensional Index among Young Cyclists from Bogotá**

---

# License

This repository is intended for academic and research purposes.

