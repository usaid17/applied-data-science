___
# Hypothesis-Driven Analysis of Telecom Customer Churn

## Project Overview

This project explores customer behavior and demographics to predict churn within the highly competitive Indian telecommunications sector (covering major providers like Airtel, Reliance Jio, Vodafone, and BSNL). Rather than solely building a predictive model, this analysis applies a rigorous, hypothesis-driven framework to diagnose model performance issues and deliver actionable data strategy recommendations.

## Repository Structure

* `data/`
* `telecom_demographics.csv`
* `telecom_usage.csv`


* `notebook/`
* `Hypothesis-Driven Analysis of Telecom...` (Jupyter Source File)


* `README.md`

## Methodology

1. **Data Merging & Preprocessing:** Combined demographic and usage datasets, applied One-Hot Encoding for categorical variables, and standardized numeric features.
2. **Baseline Modeling:** Trained Logistic Regression and Random Forest Classifiers to establish baseline metrics.
3. **Hypothesis Testing:** Investigated the models' inability to identify churners (0% recall) by systematically testing:
* Probability threshold adjustments.
* Class weight balancing to penalize minority class misclassifications.
* Feature predictiveness and distribution overlap.



## Key Findings

* **Model Performance:** Baseline models achieved ~80% accuracy but 0% recall, effectively acting as majority-class predictors.
* **Root Cause Analysis:** Adjusting thresholds and class weights failed to improve recall significantly. Exploratory Data Analysis (EDA) on the most important features revealed complete distribution overlap between churners and non-churners.
* **Conclusion:** The provided demographic and basic usage variables lack the necessary discriminative signal to predict customer churn effectively.

## Business Recommendations

To build a functional churn prediction model, the business must prioritize collecting highly correlated behavioral signals, including:

* Customer support interactions and network complaints.
* Competitor engagement or porting inquiries.
* Financial triggers such as late payments or rejected offers.
* Dynamic engagement metrics (e.g., 30-day usage trends).

## How to Run

1. Clone the master repository and navigate to this project's directory.
2. Ensure the `data/` folder contains both required CSV files.
3. Open the Jupyter Notebook in the `notebook/` directory to review the code, visualizations, and complete analysis.