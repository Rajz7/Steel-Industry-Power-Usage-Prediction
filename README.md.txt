# README.md
# Predicting Electricity Usage in Steel Industry

## Project Overview
This project focuses on predicting electricity consumption (`Usage_kWh`) in the steel industry using historical operational data. We explore both linear regression and Random Forest regression to handle skewed data and capture nonlinear relationships in the dataset.

## Dataset
- Source: `steel_industry_data.csv`
- Key columns:
  - `Usage_kWh`: Electricity usage (target)
  - `Lagging_Current_Reactive.Power_kVarh`
  - `Leading_Current_Reactive_Power_kVarh`
  - `Lagging_Current_Power_Factor`
  - `Leading_Current_Power_Factor`
  - `NSM`: Number of shifts or operational measure
  - `CO2(tCO2)`: CO2 emissions

## Methodology
1. **Exploratory Data Analysis (EDA)**:
   - Checked distributions and skewness.
   - Visualized histograms and boxplots for key variables.
2. **Data Preprocessing**:
   - Log transformation applied to reduce right-skew in `Usage_kWh`.
3. **Modeling**:
   - Linear Regression with and without log-transformed target.
   - Random Forest Regression with hyperparameter tuning (`n_estimators`, `n_jobs=-1` for parallelization).
4. **Evaluation**:
   - Metrics: RMSE, MSE, R².
   - Residual analysis and distribution comparison.
5. **Visualization**:
   - Predicted vs actual plots, residual plots, log-transform effects.

## Results
- **Linear Regression (log-transformed target)**: Captured central tendency but underestimates high usage values.
- **Random Forest Regression**:
  - Captures nonlinearity and extreme values better.
  - RMSE significantly lower and distribution of predictions closely matches true data.
  - Handles skewed data without transformation.

## Key Features / Skills Demonstrated
- Python, pandas, numpy, matplotlib, scikit-learn.
- Handling skewed distributions and feature analysis.
- Model comparison and evaluation metrics.
- Residual analysis and visualization.
- Feature importance interpretation using Random Forest.

## Folder Structure
