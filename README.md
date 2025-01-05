# Predicting Stock Prices Using LSTM and Linear Regression Models

## Project Summary

This project aims to develop predictive models for IT companies’ stock prices using historical data. We employed three distinct approaches: Long Short-Term Memory (LSTM) networks, a type of recurrent neural network well-suited for time series forecasting, LSTM using technical indicators in place of the traditional Open, High, Low, Volume features, and Linear Regression, a traditional statistical method. The objective is to evaluate and compare the performance of these models in predicting future stock prices, leveraging historical features such as open, high, low prices, volume, and adjusted close prices in two of the models and technical indicators like RSI (Relative Strength Index), EMA (Exponential Moving Average), SMA (Simple Moving Average), and MACD (Moving Average Convergence Divergence).

## Project Description

### 1. Introduction

Stock price prediction is a challenging but important task in financial analytics. Accurate predictions can assist investors in making informed decisions. In this project, we focus on exploring how different modelling techniques can forecast stock prices.

### 2. Data Collection and Preparation

- **Data Source**: Datasets were downloaded using the `yfinance` module in Python.
- **Preprocessing**: The dataset is cleaned and organized to include relevant features for the prediction tasks. For Linear Regression, data is prepared by creating lagged target variables. For LSTM, data is scaled and shaped appropriately for time series forecasting.

### 3. Model Development

- **Linear Regression**:
  - **Feature Engineering**: Used features like 'Open', 'High', 'Low', and 'Volume' to predict the next day’s 'Adj Close' price.
  - **Training and Testing**: The data is split into training and testing sets, with the model trained on historical data and evaluated on unseen test data.

- **Long Short-Term Memory (LSTM)**:
  - **Data Preparation**: Data is scaled and reshaped into sequences to fit the LSTM model’s requirements.
  - **More features**: Additional technical indicators like RSI, MACD, SMA, and EMA are used for one of the models.
  - **Model Training**: An LSTM model is built and trained using the prepared sequences, optimizing it for accurate forecasting.

### 4. Evaluation and Comparison

- **Performance Metrics**: Both models are evaluated using Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE) to assess their prediction accuracy.
- **Visualization**: Graphs comparing actual stock prices with predictions from both models are plotted to visualize performance.

### 5. Results

- **Linear Regression**: The Linear Regression model provides a baseline for comparison with LSTM. Its performance is evaluated using MAE and RMSE metrics.
- **LSTM Model**: The LSTM model is expected to capture complex patterns in the time series data and potentially outperform the Linear Regression model.

### 6. Conclusion

This project demonstrates how different forecasting techniques can be applied to stock price prediction. The comparison between Linear Regression and LSTM models provides insights into their effectiveness and suitability for financial time series forecasting.


## Dependencies

- numpy
- pandas
- scikit-learn
- tensorflow
- yfinance
- matplotlib
