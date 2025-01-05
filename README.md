# Stock Price Predictor

Predicting Stock Prices Using LSTM and Linear Regression Models
Project Summary
This project aims to develop predictive models for IT companies’ stock prices using historical data. We employed three distinct approaches:

LSTM (Long Short-Term Memory): A type of recurrent neural network well-suited for time series forecasting.
LSTM with Technical Indicators: Using features like RSI (Relative Strength Index), EMA (Exponential Moving Average), SMA (Simple Moving Average), and MACD (Moving Average Convergence Divergence).
Linear Regression: A traditional statistical method for forecasting.
The objective is to evaluate and compare the performance of these models in predicting future stock prices.

Table of Contents
Introduction
Data Collection and Preparation
Model Development
Linear Regression
Long Short-Term Memory (LSTM)
Evaluation and Comparison
Results
Conclusion
Dependencies


1. Introduction
Stock price prediction is a challenging but important task in financial analytics. Accurate predictions can help investors make informed decisions. This project explores the effectiveness of different modeling techniques for forecasting stock prices.

2. Data Collection and Preparation
Data Source: Stock price data was collected using the yfinance module in Python.
Preprocessing:
Linear Regression: Lagged target variables were created for prediction.
LSTM: Data was scaled and reshaped for time series forecasting.

3. Model Development
a)Linear Regression
Feature Engineering: Features such as 'Open', 'High', 'Low', and 'Volume' were used to predict the next day's 'Adjusted Close' price.
Training and Testing: Data was split into training and testing sets. The model was trained on historical data and evaluated on unseen test data.
b)Long Short-Term Memory (LSTM)
Data Preparation: Data was scaled and reshaped into sequences suitable for LSTM models.
Feature Selection: Additional technical indicators (RSI, MACD, SMA, EMA) were included in one of the LSTM models for richer feature representation.
Model Training: LSTM models were trained and optimized for accurate forecasting.

4. Evaluation and Comparison
Metrics: Models were evaluated using:
Mean Absolute Error (MAE)
Root Mean Squared Error (RMSE)
Visualization: Actual stock prices were compared with model predictions through visualizations.

5. Results
Linear Regression: Served as a baseline model, evaluated using MAE and RMSE.
LSTM Model: Expected to capture complex patterns in time series data, potentially outperforming Linear Regression.

6. Conclusion
This project demonstrates the application of different forecasting techniques for stock price prediction. The comparison highlights the strengths and weaknesses of Linear Regression and LSTM models, providing insights into their suitability for financial time series forecasting.

7. Dependencies
numpy
pandas
scikit-learn
tensorflow
yfinance
matplotlib
