# 🦠 COVID-19 Forecasting Using ARIMA Time Series Analysis

This repository features a statistical approach to predicting pandemic trends. Using the ARIMA (AutoRegressive Integrated Moving Average) model, this project analyzes historical COVID-19 confirmed cases to forecast future spread, providing a data-driven perspective on public health trends.

---

## 📊 Project Overview

Time series forecasting is a powerful tool for understanding infectious disease patterns. This project implements the ARIMA framework to handle non-stationary data and generate short-term predictions for **Confirmed** COVID-19 cases.

### Key Objectives
- Perform exploratory data analysis (EDA) on time-series pandemic data  
- Test for data stationarity and apply differencing  
- Identify optimal $(p, d, q)$ parameters using ACF and PACF plots  
- Forecast future cases and evaluate accuracy against test data  

---

## 🛠️ The ARIMA Model

The model used in this analysis is **ARIMA(2, 2, 3)**, which consists of:

- **AutoRegression (p = 2):**  
  Uses the relationship between an observation and a number of lagged observations  

- **Integrated (d = 2):**  
  Applies differencing to make the time series stationary  

- **Moving Average (q = 3):**  
  Models the dependency between an observation and residual errors from lagged forecasts  

---

## 📈 Performance Metrics

The model’s effectiveness was evaluated using standard error metrics:

| Metric | Value |
|------|-------|
| MSE (Mean Squared Error) | 524,039.62 |
| RMSE (Root Mean Squared Error) | 723.91 |
| MAE (Mean Absolute Error) | 486.08 |
