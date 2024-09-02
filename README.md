# Time-Series

Description: This repository contains the Time Series Analysis project that I completed for a graduate PSTAT course at UCSB in 2024.

Abstract: 
This project focuses on analyzing and forecasting the average electricity price per kilowatt-hour in U.S. cities using two advanced time series models: the Seasonal Autoregressive Integrated Moving Average (SARIMA) Model and the State Space Model. The Data folder contains a csv dataset that spans from January 2000 to December 2020, which includes 252 data points collected from 75 urban areas. It is divide it into two parts: a training set (240 data points) and a testing set (12 data points). The data was gathered by the Bureau of Labor Statistics through mail questionnaires administered by the Department of Energy. The dataset is available via the Federal Reserve Bank of St. Louis. The Code folder contains all the R code that analyze the data and predicts. 

Methodology
1. SARIMA Model
Purpose: Capture and forecast data exhibiting regular seasonal patterns, trends, and autocorrelations.
Parameters: Tuned using ACF and PACF plots, with model selection based on criteria like AIC, AICc, and BIC.
Outcome: The SARIMA model provided accurate forecasts within the 95% confidence interval for the next 12 months.
2. State Space Model
Purpose: Decompose the time series into unobserved components (trend and seasonal) and provide real-time estimates using Kalman Filtering and Smoothing.
Parameters: Estimated using Maximum Likelihood Estimation (MLE).
Outcome: The State Space Model offered more accurate predictions and better alignment with actual values compared to the SARIMA model.

Results
1. SARIMA Model
Successfully removed seasonality and trend, resulting in a stationary time series.
Provided forecasts with minimal deviation from actual values, all within the 95% confidence intervals.
2. State Space Model
Decomposed the observed data into trend and seasonal components effectively.
Produced forecasts that closely matched actual values, demonstrating higher prediction accuracy than the SARIMA model.
