
# Executive A/B Experiment Analysis: Landing Page Conversion Test

This project demonstrates a complete analytics workflow for evaluating an A/B experiment conducted on an e-commerce landing page.

The goal of the experiment was to determine whether a new landing page increases the conversion rate compared to the existing page.

The project focuses not only on statistical testing but also on experiment validation, diagnostics, and producing a decision-ready executive report.

---

## Project Workflow

Dataset  
↓  
Python data validation  
↓  
A/B statistical analysis  
↓  
Experiment diagnostics  
↓  
AI executive report generation  
↓  
PDF business report

---

## Dataset

The dataset contains user-level observations from an A/B experiment with the following fields:

- **id** — unique user identifier  
- **time** — time of interaction  
- **con_treat** — experiment group (control / treatment)  
- **page** — page version (old_page / new_page)  
- **converted** — whether the user converted (1) or not (0)

The experiment tests whether the **new landing page improves conversion rate**.

---

## Data Validation & Cleaning

Before analysis, several validation steps were performed:

- removed inconsistent experiment assignments  
  - `control → new_page`  
  - `treatment → old_page`
- checked for duplicate users
- deduplicated dataset to ensure **one record per user**
- verified experiment traffic allocation

These steps ensure that the experiment results are reliable.

---

## A/B Statistical Analysis

The following metrics were calculated:

- number of users per group
- number of conversions
- conversion rate
- absolute uplift
- relative uplift

Statistical significance was evaluated using:

- **Two-proportion Z-test**
- **95% confidence interval**

---

## Experiment Diagnostics

Additional checks were performed to validate the experiment quality:

### Sample Ratio Mismatch (SRM)

A chi-square test was used to verify whether traffic was distributed correctly between experiment groups.

### Statistical Power

Power analysis was performed to estimate the **required sample size** for detecting a meaningful improvement in conversion rate.

---

## Results

The analysis shows that the difference between the new and old landing pages is **not statistically significant**.

- p-value > 0.05
- confidence interval includes 0

This indicates that the experiment does not provide sufficient evidence that the new page improves conversion.

---

## AI-Generated Executive Report

After completing the analysis, the experiment results are structured into JSON and sent to an AI model to generate a **decision-ready executive report**.

The report summarizes:

- experiment objective
- key metrics
- statistical conclusions
- business interpretation
- recommendations

---

## Final Output

The final deliverable is a **PDF executive report** generated automatically from the analysis results.

Pipeline:

