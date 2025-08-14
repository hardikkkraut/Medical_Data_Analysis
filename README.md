# Medical Data Analysis

## Overview
A statistical analysis of patient examination data to uncover relationships between lifestyle, vitals, and diagnostic outcomes. Includes cleaning, feature engineering, categorical plots, and correlation analysis with clear documentation.

## Dataset
# - **Location**: data/medical_examination.csv
# - **Examples**: age, height, weight, cholesterol, glucose, blood pressure, activity, smoking, alcohol
# - **Ethics**: anonymized data only; no attempt to re-identify subjects

## Implementation
# 1. Clean and validate units (e.g., cm vs. m) and compute BMI and binary risk flags.
# 2. Encode categorical variables and bin continuous variables where helpful.
# 3. Produce categorical plots (counts by risk factors) and violin/box plots for distributions.
# 4. Compute correlation matrix; visualize heatmap with triangular masking and annotated coefficients.
# 5. Document statistical tests used (e.g., chi-square, t-test/Mann–Whitney) with assumptions.

## Tech Stack
# Python, Pandas, NumPy, Matplotlib, Seaborn, SciPy/Statsmodels

## Results
# - Clear relationships between risk factors and outcomes visualized.
# - Correlation heatmap to highlight strongest associations.
# - Reproducible analysis pipeline for future datasets.

## How to Run
   python -m venv .venv
   .venv\Scripts\activate
   pip install -r requirements.txt
   python src/eda.py            # creates plots in reports/figures

## Project Structure
# - data/medical_examination.csv
# - src/eda.py
# - reports/figures/
# - requirements.txt
# - README.md

## Reproducibility
# - Python 3.9+ recommended
# - Install exact package versions via equirements.txt
# - Set a global random seed where applicable for deterministic splits

## Future Improvements
# - Add predictive modeling (logistic regression, tree-based models) with calibration curves.
# - Balance classes using stratified splits or resampling when needed.
# - Package reusable feature engineering steps into a scikit-learn pipeline.

# ---
Author: Hardik Raut • GitHub: https://github.com/hardikkkraut

