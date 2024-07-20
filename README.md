# Forecasting_Models
A forecasting model is a statistical tool designed to predict future trends and outcomes based on historical data. It involves analyzing past patterns and trends to make informed predictions about future events, sales, demand, or inventory levels.


# ARIMA, SARIMA, SARIMAX - Time Series Forecasting

This project involves the implementation and analysis of ARIMA, SARIMA, and SARIMAX models for time series forecasting. The dataset used is the Drug Sales dataset.

## Project Overview

The aim of this project is to:
1. Understand and implement ARIMA models for time series forecasting.
2. Extend ARIMA models to seasonal data using SARIMA.
3. Incorporate exogenous variables into the SARIMA model using SARIMAX.

## Dataset

The dataset used in this project is stored in a file named `dataset.txt`. It contains the monthly sales data of a drug.

## Steps and Methodology

### 1. ARIMA Model for Time Series Forecasting
ARIMA (AutoRegressive Integrated Moving Average) is a forecasting algorithm based on past values of the time series. ARIMA models are specified by three order parameters: (p, d, q).
- `p`: order of the AR term.
- `d`: order of differencing.
- `q`: order of the MA term.

#### Steps:
- **Checking for Stationarity:** Using the Augmented Dickey-Fuller (ADF) test to check if the time series is stationary.
- **Differencing:** If the series is not stationary, apply differencing.
- **Determining AR and MA Terms:** Using PACF and ACF plots to determine the values of `p` and `q`.
- **Model Training:** Building the ARIMA model with the determined parameters.

### 2. SARIMA Model for Seasonal Time Series Forecasting
SARIMA (Seasonal ARIMA) extends ARIMA to capture seasonality in the data.

#### Steps:
- **Seasonal Differencing:** Applying seasonal differencing to remove seasonal effects.
- **Determining Seasonal AR and MA Terms:** Using seasonal PACF and ACF plots to determine the seasonal parameters (P, D, Q, m).
- **Model Training:** Building the SARIMA model with the seasonal parameters.

### 3. SARIMAX Model with Exogenous Variables
SARIMAX (Seasonal ARIMA with eXogenous variables) incorporates external predictors into the model.

#### Steps:
- **Creating Exogenous Variables:** Computing seasonal indices or other relevant predictors.
- **Model Training:** Building the SARIMAX model using the exogenous variables.

