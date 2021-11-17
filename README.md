# Time Series Analysis ARIMA

This is our implementation on ARIMA time series analysis. 

This project is to analyze the stock price. Apple(APPL) historical data is collected from Yahoo Finance. From the historical data, we were utilizing ARIMA to do time series analysis and predict the upcoming stock price. 

This model is great as an addition to our deciding factor but shouldn’t be our main factor because there are many other variables that affect stock prices. One data that is important to predict stock prices is the P/E ratio. This model is great because autoARIMA decides for us which p,d,q values are the best for our model and it uses historical data to give us insight on how the data would be in the future. This is only one of the factors that should be considered in stock analysis as there are many other factors besides historical data that would affect the analysis of stock’s market price and what is the best option to exercise in stocks.

Also, it is recommended to run on jupyter notebook. With jupyter lab, there ARIMA model is updated, thus it will no longer work with the older versions. 

## Table of Content
* [Features](https://github.com/byu5/time_series_analysis_ARIMA/blob/main/README.md#features)
* [Get Started](https://github.com/byu5/time_series_analysis_ARIMA/blob/main/README.md#get-started)
* [Background](https://github.com/byu5/time_series_analysis_ARIMA/blob/main/README.md#background)
* [Contributors](https://github.com/byu5/time_series_analysis_ARIMA/blob/main/README.md#contributors)

## Features
The data analysis will provide:
- Time series data into testing and training sets
- Standardized residual
- Histogram plus estimated density 
- Normal Q-Q 
- Correlogram
- MSE, MAE, RMSE, and MAPE


## Get Started
+ We would require libraries called pmdarima. This is used for .autoarima. The model that we use is a function called auto_arima.
+ _pip install pmdarima_


## Background
+ AR (Autoregressive)
The AR algorithm determines the linear regression of (Present fitted values) vs. (Past fitted values).
+ MA (Moving Average)
The linear regression of the (Present value of residuals) vs. MA is discovered by MA (Past value of residuals).
We employ a mixture of the two (ARIMA).

+ ADF (Augmented Dickey-Fuller) Test
One of the most widely used statistical tests is the Dickey-Fuller test. It can be used to determine whether or not a series has a unit root, and thus whether or not the series is stationary. This test’s null and alternate hypotheses are:
Null Hypothesis: The series has a unit root (value of a =1)
Alternate Hypothesis: The series has no unit root.

The auto_arima function returns a fitted ARIMA model after determining the most optimal parameters for an ARIMA model. This function is based on the forecast::auto. Arima R function, which is widely used.

## Contributors
- Weijia Wang
- Barry Yu
- Giani Kurniawan
