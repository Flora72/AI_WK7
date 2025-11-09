
#  COMPAS Fairness Audit – Practical Ethics in Action

This repository contains the technical audit for **Part 3: Practical Audit** of the AI Ethics assignment, themed *“Designing Responsible and Fair AI Systems.”* It focuses on identifying and mitigating racial bias in the COMPAS Recidivism dataset using IBM’s **AI Fairness 360** toolkit.

---

##  Objective

Audit the COMPAS dataset for racial bias in recidivism predictions, focusing on disparities in **false positive rates** between African-American and Caucasian defendants. Use fairness metrics and visualizations to support findings and propose remediation.

---

## Tools & Libraries

- **AI Fairness 360** – fairness metrics, bias mitigation
- **Pandas** – data manipulation
- **Matplotlib** – visualizations
- **Scikit-learn** – logistic regression model

---

##  Project Structure

```
 compas-fairness-audit/
├── COMPAS_Fairness_Audit.ipynb     # Main notebook with code, metrics, and visuals
├── requirements.txt                # Reproducible environment
├── .gitignore                      # Clean repo hygiene
└── README.md                       # Practical audit overview
```

---

##  Key Steps

1. **Load and preprocess** the COMPAS dataset using `CompasDataset` from AIF360  
2. **Define privileged/unprivileged groups** based on race  
3. **Train a logistic regression model** to simulate predictions  
4. **Evaluate fairness metrics** using `BinaryLabelDatasetMetric` and `ClassificationMetric`  
5. **Visualize false positive rate disparities** between racial groups  
6. **Apply reweighing** as a bias mitigation strategy  
7. **Summarize findings** in a 300-word report

---

##  Findings

- African-American defendants had a significantly **higher false positive rate** than Caucasian defendants  
- The **disparate impact ratio** was below the fairness threshold of 0.8  
- **Reweighing** improved fairness metrics, reducing disparity

---

## Visualization

A bar chart was generated to compare false positive rates by race, clearly illustrating the disparity and supporting the need for mitigation.

---

## Summary Report

A 300-word summary is included in the notebook, detailing:
- Bias findings
- Ethical implications
- Remediation steps

---
##  Assignment Document

You can view the full assignment brief [here](https://docs.google.com/document/d/1ekAhZ2qVHhMAvRAaz-YDXs62dkCasZPVEqa6k--kysM/edit?usp=sharing).
