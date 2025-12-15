
---

# summary.md
# Project Summary: Predicting Electricity Usage in Steel Industry

**Objective:**  
Predict electricity consumption in the steel industry using historical operational data, and compare model performance between linear regression (with log-transformed targets) and Random Forest regression.

**Approach:**  
- Conducted EDA to understand distribution and skewness of key variables.
- Applied log transformation to reduce skew in linear regression experiments.
- Trained and evaluated:
  - Linear Regression
  - Random Forest Regression with 200–350 estimators and parallel computation (`n_jobs=-1`).
- Evaluated models using RMSE, MSE, R², and residual plots.

**Key Insights:**
- Linear regression with log-transform improves central prediction but **underestimates extreme high values**.
- Random Forest handles **nonlinear relationships** and skewed distributions well, achieving **low RMSE** and **high R²**.
- Residual analysis confirms Random Forest predictions are unbiased across the range of usage values.
- Feature importance highlights operational parameters most influencing electricity consumption.

**Technical Skills Demonstrated:**
- Python: pandas, numpy, matplotlib
- Machine Learning: Linear Regression, Random Forest, model evaluation
- Data preprocessing, log transformation, handling skewed distributions
- Visualizations: histograms, boxplots, residual plots

**Results & Impact:**
- Random Forest Regression closely matches the true distribution of electricity usage.
- Provides actionable insights for energy optimization in industrial settings.
