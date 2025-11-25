
# Advanced Time Series Forecasting With State Space Models and Optimization

This project implements an advanced state-space forecasting model using a linear Gaussian framework, estimated through both EM and maximum likelihood optimization, with benchmarking against SARIMAX. It supports trend, seasonal harmonics, regressors, and full Kalman filtering for forecasting.
This project implements an advanced state-space forecasting model using a linear Gaussian framework, estimated through both EM and maximum likelihood optimization, with benchmarking against SARIMAX. It supports trend, seasonal harmonics, regressors, and full Kalman filtering for forecasting.



Benchmark Pipeline
Running the file directly performs:
1.	Synthetic data generation
2.	Train/test split
3.	EM estimation & forecasting
4.	MLE estimation & forecasting
5.	SARIMAX baseline
6.	Automatic evaluation (RMSE, MAE, MAPE)
7.	Final report



Project Structure
   ssm_em_forecast.py

   Forecast Metrics
Built-in metrics:
•	RMSE
•	MAE
•	MAPE

Synthetic Data Generator
The file includes a flexible generator producing:
•	Weekly + yearly seasonality
•	Piecewise linear trend
•	Optional regressor with campaign shocks
•	Additive Gaussian noise
Perfect for benchmarking SSMs






          

## Features

 Model Components
•	Local Linear Trend
State vector includes level + slope.
•	Multiple Seasonalities
Weekly and yearly seasonalities implemented using harmonic rotation matrices.
•	Regressors / Exogenous Variables
Fully supported in the observation equation.
•	Diagonal Q + scalar R
Estimated either with EM or direct MLE.



## Installation


```
    Installation
pip install numpy scipy pandas statsmodels
## Acknowledgements

 -Kalman filtering concepts from Durbin & Koopman

Seasonal harmonic state-space structures inspired by Hyndman et al.

