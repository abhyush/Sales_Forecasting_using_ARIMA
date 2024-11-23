# Time Series Forecasting with ARIMA and Seasonal ARIMA

This project demonstrates the process of building ARIMA and Seasonal ARIMA models for time series forecasting. Using a dataset of Perrin Freres' monthly champagne sales, the project covers key steps including data cleaning, visualization, testing for stationarity, and model construction for forecasting future sales.

---

## 📖 Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Methodology](#methodology)
- [Results](#results)
- [References](#references)

---

## 🌟 Overview
The project involves:
1. Cleaning and preprocessing time series data.
2. Testing for stationarity and making the data stationary using differencing.
3. Using AutoCorrelation Function (ACF) and Partial AutoCorrelation Function (PACF) plots to identify model parameters.
4. Building ARIMA and Seasonal ARIMA models to forecast future values.

---

## ✨ Features
- **Data Cleaning**: Prepares the dataset for time series modeling.
- **Stationarity Testing**: Utilizes the Augmented Dickey-Fuller test.
- **ACF and PACF Analysis**: Determines model parameters.
- **ARIMA Model**: Builds a non-seasonal model for time series data.
- **Seasonal ARIMA Model**: Incorporates seasonality in the forecasting process.
- **Future Predictions**: Generates forecasts for future periods.

---

## 🛠 Requirements
- Python 3.x
- pandas
- numpy
- matplotlib
- statsmodels

---

## 🧠 Methodology
### Step 1: Data Cleaning
- Rename columns for clarity.
- Remove unnecessary rows.
- Convert the date column to a datetime format and set it as the index.

### Step 2: Visualize the Data
- Plot the time series data to observe trends and seasonality.

### Step 3: Test for Stationarity
- Use the Augmented Dickey-Fuller (ADF) test to check for stationarity.
- Apply differencing to make the data stationary.

### Step 4: Analyze ACF and PACF
- Plot ACF and PACF charts to determine the ARIMA parameters:
  - `p`: Number of autoregressive terms.
  - `d`: Number of differences.
  - `q`: Number of moving average terms.

### Step 5: Build ARIMA and Seasonal ARIMA Models
- Use the `statsmodels` library to fit ARIMA and SARIMA models.
- Evaluate the model using statistical summaries and diagnostic plots.

### Step 6: Forecast Future Values
- Generate forecasts using the fitted models.
- Extend the time series with future dates and visualize the predictions.

---

## 📊 Results
### Key Findings
- The seasonal differencing successfully made the data stationary (ADF test statistic: -7.63, p-value: 2.06e-11).
- The ARIMA(1,1,1) model effectively captured the non-seasonal components of the time series.
- The SARIMA(1,1,1)(1,1,1,12) model provided accurate seasonal forecasts.

### Visualizations
- Time series plot with actual and forecasted values.
- ACF and PACF plots for parameter selection.

---

## 🔍 References
- [Statsmodels Documentation](https://www.statsmodels.org/)
- [ARIMA Overview](https://otexts.com/fpp2/arima.html)
- [Augmented Dickey-Fuller Test](https://en.wikipedia.org/wiki/Augmented_Dickey%E2%80%93Fuller_test)
