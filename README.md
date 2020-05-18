# COVID19_TimeSeries_Comparison
Brief comparison of Time Series methods to predict daily confirmed cases of Coronavirus

My personal goal in this notebook was to learn about Time Series and use it to help forecasting the possible evolution of the Coronavirus outbreak.
This is not intended to be a comprehensive study, but more a beginner's introduction to apply time series.

The methods compared are classical time series like Autoregressive Integrated Moving Average (ARIMA)  and Holt-Winters Exponential Smoothing, machine learning  methods like several types of Long Short Term Memory (LSTM) networks, and Facebook Prophet as well.

ARIMA requires data sets to be stationary, and most data related to the Coronavirus outbreak has shown an exponential growth, though it has started to reduce the slope in the trend in some places.
This exercise demonstrates a comparison between different models using root mean squared error to measure the model performance after using Walk-forward validation testing.

The dataset used is corona-virus-report\covid_19_clean_complete.csv from https://www.kaggle.com.

Before getting into the forecast analysis, there are some visual comparisons between countries in features like "Confirmed" (accumulated number of confirmed cases), "New_Confirmed" (daily number of confirmed cases), "Deaths" (accumulated number of deaths), "New_Deaths" (daily number of deaths), "Recovered" (accumulated number of recovered cases), "New_ Recovered" (daily number of recovered cases), "Active" (difference between the number of confirmed cases and the number of deaths and recovered cases).
The last feature is CFR (Case fatality rate) which is the ratio between deaths to confirmed cases. 

Important references:

- Italy space time & spreading of Covid19
https://www.kaggle.com/lumierebatalong/italy-space-time-spreading-of-covid19

- How to Grid Search Triple Exponential Smoothing for Time Series Forecasting in Python
https://machinelearningmastery.com/how-to-grid-search-triple-exponential-smoothing-for-time-series-forecasting-in-python/

- How to Develop LSTM Models for Time Series Forecasting
https://machinelearningmastery.com/how-to-develop-lstm-models-for-time-series-forecasting/

- How To Backtest Machine Learning Models for Time Series Forecasting
https://machinelearningmastery.com/backtest-machine-learning-models-time-series-forecasting/

- Time Series Forecast Case Study with Python: Monthly Armed Robberies in Boston
https://machinelearningmastery.com/time-series-forecast-case-study-python-monthly-armed-robberies-boston/
