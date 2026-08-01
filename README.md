# Revenue Time Series Forecasting

## Overview

This project develops a time series forecasting model to predict future daily revenue using historical revenue data. The analysis follows the complete forecasting workflow, including data preparation, stationarity testing, ARIMA model selection, model evaluation, and future revenue forecasting.

---

## Business Problem

Organizations rely on accurate revenue forecasts for budgeting, inventory planning, and strategic decision-making. This project evaluates whether historical daily revenue can be used to reliably forecast future revenue trends.

---

## Tools Used

- Python
- Pandas
- NumPy
- Matplotlib
- Statsmodels
- pmdarima
- Scikit-learn
- Jupyter Notebook

---

## Project Workflow

- Import and explore the dataset
- Convert the data into a time series
- Visualize revenue trends
- Test stationarity using the Augmented Dickey-Fuller (ADF) test
- Apply first-order differencing
- Analyze ACF and PACF plots
- Compare multiple ARIMA models
- Select the optimal model using AIC
- Evaluate forecasting performance using a train/test split
- Generate a 147-day revenue forecast

---

## Model Selection

Three ARIMA models were evaluated:

- ARIMA(1,1,2)
- ARIMA(1,1,1)
- ARIMA(1,1,0)

ARIMA(1,1,0) was selected because it produced the lowest Akaike Information Criterion (AIC) while maintaining a simpler model structure.

---

## Model Evaluation

Evaluation metrics included:

- RMSE
- MAE
- MSE

The model was trained using an 80/20 chronological train-test split and evaluated on unseen revenue data.

---

## Key Findings

- The original revenue series was non-stationary.
- First-order differencing successfully stabilized the data.
- Revenue exhibited an upward trend with recurring seasonal behavior.
- ARIMA(1,1,0) provided the best balance between accuracy and model simplicity.
- The final forecast projected relatively stable future revenue while confidence intervals widened over time.

---

## Forecast Preview

*(Insert your final forecast visualization here.)*
