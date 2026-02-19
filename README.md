# Flight Delay Prediction Using Logistic Regression, SES, and SARIMA

This project analyzes and predicts flight delays in the United States using classification and time series forecasting approaches. The study applies Logistic Regression for delay classification and SES (Single Exponential Smoothing) and SARIMA for short-term and long-term forecasting.

## Dataset

* Source: U.S. Bureau of Transportation Statistics (BTS)
* Period: January 2022 – February 2025
* Features include carrier delay, weather delay, NAS delay, security delay, late aircraft delay, and arrival delay
* Time series case study focused on Hartsfield–Jackson Atlanta International Airport (ATL)

## Methodology

CRISP-DM framework:

* Business Understanding
* Data Understanding
* Data Preparation
* Modeling
* Evaluation
* Deployment

## 1. Classification Model – Logistic Regression

Goal: Classify whether a flight is delayed (>15 minutes) or not.

Data preparation:

* Feature selection
* One-hot encoding
* Feature scaling
* 80:20 train-test split

Performance:

* Accuracy: 81%
* Precision: 83%
* Recall: 90%
* F1-score: 86%

Key predictors:

* Late arriving aircraft
* Carrier delay

The model effectively detects delayed flights and minimizes misclassification.

## 2. Time Series Forecasting

### Short-Term Forecast (1 Month) – SES

* MSE: 47,044.64
* MAPE: 8.6% (Very Good Forecast)

SES performs best for short-term prediction.

### Long-Term Forecast (6 Months) – SARIMA

* MSE: 44,303,781.25
* MAPE: 19.50% (Good Forecast)

SARIMA performs better for longer forecasting horizons due to its ability to capture seasonality and trend patterns.

## Key Insights

* Flight delays show strong seasonal patterns, peaking during summer (especially July).
* Late aircraft and carrier-related issues are the dominant contributors to delays.
* SES is highly accurate for short-term forecasting.
* SARIMA is more stable for long-term predictions.

## Conclusion

* Logistic Regression provides reliable delay classification.
* SES is optimal for short-term forecasting.
* SARIMA is more suitable for long-term seasonal forecasting.

This project demonstrates how combining classification and time series models can support data-driven decision-making in airline operations and delay mitigation strategies.
