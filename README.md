# TSLA-LSTM-Forecast
Predict Tesla’s stock price using a deep learning model, specifically the LSTM – Long Short-Term Memory neural network.

#  TSLA Stock Price Prediction Using LSTM

This project uses a Long Short-Term Memory (LSTM) neural network to predict the future stock prices of **Tesla Inc. (TSLA)** based on historical data. It demonstrates how deep learning can be applied to time-series data for financial forecasting.

# Project Overview

- Objective: Predict future TSLA stock prices using historical closing prices.
- Approach: Use LSTM, a type of Recurrent Neural Network (RNN), suited for sequential/time-series data.
- Tools Used: Python, TensorFlow/Keras, yfinance, matplotlib, scikit-learn

# Technologies & Libraries

- `Python`
- `TensorFlow` / `Keras`
- `NumPy` / `Pandas`
- `Matplotlib`
- `yfinance` (for fetching TSLA data)
- `MinMaxScaler` from `sklearn.preprocessing`

# Dataset

- Downloaded using the `yfinance` library.
- Stock: Tesla (TSLA)
- Data Range: From the start of Tesla’s historical stock data up to `2024-12-31`
- Focused column: `Close` price

# Steps Involved

# 1. Data Collection
- Used `yfinance.download()` to fetch full TSLA stock history.

# 2. Data Preprocessing
- Extracted `Close` prices
- Scaled values between 0 and 1 using `MinMaxScaler`
- Created sequences of 60 days to predict the 61st day

# 3. LSTM Model Building
- Two LSTM layers with dropout
- Dense output layer for regression
- Optimized with `Adam`
- Trained over 10 epochs

# 4. Prediction & Visualization
- Predicted prices on test data
- Converted scaled predictions back to real values
- Plotted actual vs predicted prices for evaluation

# Output Visualization
![image](https://github.com/user-attachments/assets/bcf4208b-5423-4d90-af7a-5a58e551f562)

The line graph shows how closely the model’s predictions follow the actual price trends of Tesla stock.

# Learnings

- Applied time-series forecasting with LSTM
- Learned how to process financial data using Python
- Practiced key machine learning concepts: scaling, sequence creation, model training & evaluation
