# E-commerce Revenue Forecasting using ARIMA

Time series analysis and 14-day revenue forecasting on e-commerce sales data using ARIMA modelling.

## Overview

This project applies ARIMA-based time series modelling to daily e-commerce revenue data to forecast the next 14 days of sales. It covers the full pipeline from stationarity testing to model selection and final forecast with confidence intervals.

## Tools Used

- Python — pandas, numpy, matplotlib, seaborn, statsmodels
- Models — AR(1), MA(1), ARMA(1,1), ARIMA
- Statistical Tests — ADF Test, Yule-Walker Estimation, Ljung-Box Test, ACF/PACF Analysis
- Data — E-commerce order dataset (daily revenue aggregated from transaction records)

## Files

| File | Description |
|---|---|
| `TSA_ASSIGNMENT.ipynb` | Full notebook — EDA, stationarity tests, model comparison, forecast |
| `final ecommerce.xlsx` | E-commerce transaction dataset |

## How to Run

```bash
pip install pandas numpy matplotlib seaborn statsmodels openpyxl
jupyter notebook TSA_ASSIGNMENT.ipynb
```

## Methodology

Raw Transaction Data → Daily Revenue Aggregation → ADF Stationarity Test → Differencing → Yule-Walker Estimation → AR(1) vs MA(1) vs ARMA(1,1) Comparison (AIC/BIC) → Final ARIMA Model → Ljung-Box Residual Validation → 14-Day Forecast with 95% Confidence Intervals

## Key Steps

- Aggregated transaction-level data into a continuous daily revenue time series
- Applied ADF test to check stationarity; used first-order differencing where needed
- Compared AR, MA, and ARMA models using AIC and BIC criteria
- Validated final model with Ljung-Box test (residuals confirmed as white noise)
- Forecasted next 14 days of revenue with confidence intervals

## Author

Hasini Gogula 
Christ University 
