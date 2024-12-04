# **Stock Price Prediction Using Machine Learning Models**

This project explores predicting stock prices using historical data and technical indicators, leveraging machine learning models for enhanced accuracy. It includes a comprehensive model evaluation (`ML FOR PREDICTIVE ANALYSIS.ipynb`) and an interactive user interface (`ProjectDemo.ipynb`) to predict stock prices.

---

## **Project Overview**

### **Files**
1. **`ML FOR PREDICTIVE ANALYSIS.ipynb`**:
   - A research-driven notebook where different machine learning models were implemented and evaluated to determine the most effective approach for stock price prediction.
   - Models compared: 
     - Linear Regression
     - Random Forest Regressor
     - Support Vector Regressor (SVR)

2. **`ProjectDemo.ipynb`**:
   - An interactive notebook that allows users to predict next-day stock prices or a specific future date based on historical data.
   - Implements the best-performing model (Random Forest Regressor) and provides an easy-to-use interface with widgets.

---

## **Data Collection**
- **Source**: Yahoo Finance (`yfinance` library)
- **Stock**: Apple Inc. (`AAPL`)
- **Timeframe**: January 2022 to January 2023
- **Technical Indicators**:
  - Simple Moving Average (SMA)
  - Exponential Moving Average (EMA)
  - Relative Strength Index (RSI)
  - Volatility
- **Target Variable**: Next-day closing price.

---

## **Models Implemented**
- **Linear Regression**: A simple baseline model for predicting stock prices.
- **Random Forest Regressor**: An ensemble learning model that aggregates predictions from multiple decision trees.
- **Support Vector Regressor (SVR)**: A regression model optimized for non-linear relationships.

---

## **Evaluation Metrics**
To evaluate model performance, the following metrics were used:
- **MAE (Mean Absolute Error)**: Measures average prediction error.
- **MSE (Mean Squared Error)**: Penalizes larger errors.
- **R² Score**: Indicates the proportion of variance captured by the model.

---

## **Results**
| **Model**               | **MAE** | **MSE**  | **R² Score** |
|--------------------------|---------|----------|--------------|
| Linear Regression        | 2.99    | 12.54    | 0.88         |
| Random Forest Regressor  | 2.63    | 12.18    | 0.88         |
| Support Vector Regressor | 5.81    | 52.11    | 0.50         |

The **Random Forest Regressor** performed the best, accurately capturing variance in the stock data, while SVR struggled due to overfitting or insufficient feature engineering.

---

## **Interactive Prediction Features**
The `ProjectDemo.ipynb` notebook offers the following capabilities:
1. **Dynamic Ticker Selection**: Enter any valid stock ticker (e.g., `AAPL`, `GOOGL`).
2. **Historical Data Range**: Select start and end dates for data collection.
3. **Future Prediction**:
   - Predict the **next day’s price**.
   - Predict the price for a **specific future date**.
4. **Model Flexibility**:
   - Allows users to choose between multiple models for predictions.
5. **Visualization**:
   - Interactive plots for historical trends and model predictions.

---
