⚡ Electricity Production Forecasting Using SARIMA
Overview
This project builds a robust time series forecasting model for predicting monthly U.S. electricity and gas utility production. The workflow covers data preparation, exploratory analysis, seasonality detection, model development, evaluation, and future forecasting using a Seasonal ARIMA (SARIMA) approach.

Business Objective
Accurate electricity demand forecasting supports:

Energy production planning
Resource allocation
Grid management
Demand forecasting
Capacity optimization
Dataset
Source: U.S. Electric & Gas Utility Production Index

Dataset Characteristics
Monthly frequency
Date range: January 1985 – January 2018
Observations: 397
Target Variable: Production Index
Project Workflow
1. Data Preparation
Renamed columns for consistency
Converted dates to datetime format
Set date column as time-series index
Verified data completeness
2. Data Quality Assessment
Missing value analysis
Gap detection
Interpolation demonstration
Outlier detection using IQR
3. Exploratory Data Analysis
Trend visualization
Seasonal pattern analysis
Monthly production comparison
Time series decomposition
4. Stationarity Testing
Augmented Dickey-Fuller (ADF) Test
5. Baseline Models
Naïve Forecast
Seasonal Naïve Forecast
6. Advanced Forecasting Model
SARIMA (1,1,1)(1,1,1,12)
7. Model Evaluation
Performance metrics:

MAE (Mean Absolute Error)
RMSE (Root Mean Squared Error)
MAPE (Mean Absolute Percentage Error)
8. Future Forecasting
12-month production forecast
95% Confidence Intervals
Results
Model	MAE	RMSE	MAPE
Naïve	15.24	17.64	15.75%
Seasonal Naïve	4.19	6.22	3.92%
SARIMA	3.17	2.07	3.00%
Best Model
✅ SARIMA(1,1,1)(1,1,1,12)

The SARIMA model outperformed baseline approaches and effectively captured both trend and seasonal patterns.

Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Statsmodels
Scikit-learn
Repository Structure
