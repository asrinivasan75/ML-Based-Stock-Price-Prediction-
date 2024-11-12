# Stock Price Prediction Using Machine Learning Models

This project aims to predict the next-day closing prices of stocks based on historical data and technical indicators, using machine learning models. It used Python library yfinance for data collection and sklearn for model training and evaluation.

## Project Overview

In this project, I implemented and compared three machine learning models: Linear Regression, Random Forest Regressor, and Support Vector Regressor (SVR), to see which is best suited for predicting next-day prices.

### Data Collection

- **Source**: Yahoo Finance
- **Stock**: Apple Inc. (AAPL)
- **Period**: January 2022 to January 2023

### Features and Target
- **Technical Indicators**: Simple Moving Average (SMA), Exponential Moving Average (EMA), Relative Strength Index (RSI), and Volatility.
- **Target Variable**: Next-day closing price.

### Models Implemented
1. **Linear Regression**
2. **Random Forest Regressor**
3. **Support Vector Regressor (SVR)**

### Evaluation Metrics
- **MAE** (Mean Absolute Error)
- **MSE** (Mean Squared Error)
- **R² Score** (Coefficient of Determination)

## Results

| Model                     | MAE       | MSE       | R² Score |
|---------------------------|-----------|-----------|----------|
| Linear Regression         | 2.99      | 12.54     | 0.88     |
| Random Forest Regressor   | 2.63      | 12.18     | 0.88     |
| Support Vector Regressor  | 5.81      | 52.11     | 0.50     |

The **Random Forest Regressor** performed best, capturing more variance in the stock data, while SVR struggled with accuracy on this dataset.

## Conclusion

Random Forest is recommended for stock price prediction in this setup, as it balances both interpretability and performance. Future exploration could involve trying other models, like Gradient Boosting or neural networks, for potentially improved accuracy.
