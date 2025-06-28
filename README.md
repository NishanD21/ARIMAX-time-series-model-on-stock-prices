# ARIMAX time series model on stock prices

This repository contains a time series forecasting project using the ARIMAX (AutoRegressive Integrated Moving Average with Exogenous Variables) model to predict stock prices. The model leverages both historical stock price data and relevant external indicators to enhance forecast accuracy.

## 🔍 Key Features:
Data preprocessing and visualization of stock trends.
Stationarity checks and differencing.
Model selection using Auto Arima and AIC/BIC.
Integration of exogenous variables to capture external influence.
Forecasting and performance evaluation using RMSE and MAPE.
Plots comparing actual vs predicted stock prices.

## Dataset :

| Feature                     | Description                                                                                                                                                                                                                                                       |
| --------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **stock**                   | Identifier or name of the stock/security being analyzed. Useful if the dataset contains data for multiple stocks.                                                                                                                                                 |
| **Open**                    | The price at which the stock opened trading on a given day. Reflects investor sentiment at the market open.                                                                                                                                                       |
| **High**                    | The highest price at which the stock traded during the day. Indicates the day’s peak value.                                                                                                                                                                       |
| **Low**                     | The lowest price at which the stock traded during the day. Represents the minimum value seen during the trading session.                                                                                                                                          |
| **Close**                   | The final price of the stock at the end of the trading day. Often used as the primary target variable for forecasting.                                                                                                                                            |
| **holiday**                 | A binary flag indicating whether the date is a market holiday (`1`) or a regular trading day (`0`). May be used to account for missing or irregular data points in the time series.                                                                               |
| **unpredictability\_score** | A custom numeric score representing how volatile or uncertain the stock's behavior was on a given day. Could be derived from external factors, news sentiment, or intra-day volatility. Useful as an exogenous variable to model complex behavior in forecasting. |
