# Stroke Risk Factors Analysis (Exploratory Data Analysis & Statistics)

## Overview
This project investigates **key factors associated with stroke risk** using a publicly available healthcare dataset. Working as **Team 2**, we performed data cleaning, exploratory data analysis, statistical testing, and visualization to answer clinically relevant questions about stroke prevalence across demographic, lifestyle, and health-related variables.

The project combines:
- Individual analytical notebooks from team members
- A consolidated team presentation summarizing findings and interpretations

---

## Research Question
**What factors significantly affect the likelihood of having a stroke?**

Guided by this question, we examined relationships between stroke occurrence and:
- Hypertension
- Heart disease
- Age
- Average glucose level
- BMI
- Marital status
- Work type
- Residence type (urban vs rural)

---

## Dataset
- **Source:** Kaggle – Stroke Prediction Dataset  
  https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset
- **Description:** Patient-level health and demographic data including medical history, lifestyle indicators, and stroke outcomes.

---

## Technologies Used
- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib / Seaborn**
- **SciPy (statistical tests)**
- **Jupyter Notebook**

---

## Analysis Highlights

### Hypertension & Heart Disease
- Individuals with **hypertension** or **heart disease** have a **significantly higher probability of stroke**
- Chi-squared tests show **extremely small p-values (< 1e-19)**, indicating strong statistical significance
- Probability-based analysis was used instead of raw counts to account for class imbalance

---

### Glucose Level & BMI
- **Median glucose levels** are significantly higher in stroke patients
- Glucose distributions are right-skewed, with notable outliers
- **BMI** is also significantly higher in stroke patients (p = 0.006), though more normally distributed

---

### Age & Stroke Risk
- Stroke probability increases sharply with age
- Older adults represent the highest-risk group
- Linear correlation between age and stroke count (R ≈ 0.68)
- Exponential modeling suggests risk accelerates in later age groups

---

### Marital Status & Work Type
- Unmarried males show higher stroke prevalence than married males
- Self-employed individuals exhibit higher stroke rates than private or government employees
- Government workers show the lowest stroke prevalence

---

### Residence Type (Urban vs Rural)
- Slightly higher rates of heart disease and stroke in **urban areas**
- Differences are modest and likely influenced by population density
- Residence type alone is not sufficient to explain stroke risk

---

## Key Statistical Methods
- Probability-based comparisons (mean of binary outcomes)
- Chi-squared tests for categorical variables
- Box plots and distribution analysis
- Linear and exponential regression modeling
- Outlier identification and interpretation

---

## Key Takeaways
- Stroke risk is **multifactorial**, with strong associations to age, cardiovascular conditions, and metabolic indicators
- Proper statistical framing (probabilities vs raw counts) is essential for imbalanced medical data
- Correlation does not imply causation—results should be interpreted in clinical context
