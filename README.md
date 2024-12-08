# Time Series Data Analysis of Tesla and Google Stock Prices

This repository contains the time series analysis of **Tesla (TSLA)** and **Google (GOOGL)** stock prices over the period of **December 1, 2023, to December 1, 2024**. The data was sourced from [Yahoo Finance](https://finance.yahoo.com/) using Python and analyzed to determine the most effective time series model for each stock. Finally, the results of different time series models are compared to identify their strengths and weaknesses.

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Data Collection](#data-collection)
3. [Analysis Techniques](#analysis-techniques)
4. [Model Comparison](#model-comparison)
5. [Results](#results)
6. [Installation](#installation)
7. [Usage](#usage)
8. [Contributing](#contributing)
9. [License](#license)

---

## Project Overview

The goal of this project is to:
1. Analyze the historical stock prices of Tesla and Google over one year.
2. Apply various time series analysis techniques to identify trends, seasonality, and other patterns.
3. Evaluate the performance of different time series forecasting models.
4. Compare the models and recommend the best forecasting technique for Tesla and Google.

---

## Data Collection

The stock price data for Tesla (TSLA) and Google (GOOGL) was collected using the **Yahoo Finance API** with the Python library `yfinance`. The data includes:
- Date
- Open price
- High price
- Low price
- Close price
- Volume

### Example of Data Structure
| Date       | Open   | High   | Low    | Close  | Volume     |
|------------|--------|--------|--------|--------|------------|
| 2023-12-01 | 200.00 | 205.50 | 198.50 | 203.00 | 30,000,000 |
| 2023-12-02 | 203.00 | 207.00 | 202.00 | 206.50 | 32,000,000 |

---

## Analysis Techniques

### Exploratory Data Analysis (EDA)
- Time series decomposition into **trend**, **seasonality**, and **residuals**.
- Visualization of stock price trends and moving averages.

### Statistical Models
1. **ARIMA (Auto-Regressive Integrated Moving Average)**
2. **SARIMA (Seasonal ARIMA)**
3. **Holt-Winters Exponential Smoothing**

### Machine Learning Models
1. **Random Forest Regressor**
2. **Gradient Boosting**
3. **Long Short-Term Memory (LSTM) Neural Networks**

### Performance Metrics
- **Mean Absolute Error (MAE)**
- **Mean Squared Error (MSE)**
- **Root Mean Squared Error (RMSE)**

---

## Model Comparison

The results of the models were evaluated and compared for both Tesla and Google stock price predictions.

| Model                     | Tesla (MAE) | Google (MAE) | Tesla (RMSE) | Google (RMSE) |
|---------------------------|-------------|--------------|--------------|---------------|
| ARIMA                     | 3.45        | 2.98         | 4.32         | 3.87          |
| SARIMA                    | 3.22        | 2.75         | 4.10         | 3.65          |
| Holt-Winters              | 3.56        | 3.10         | 4.50         | 4.05          |
| Random Forest Regressor   | 2.95        | 2.50         | 3.88         | 3.50          |
| Gradient Boosting         | 2.80        | 2.35         | 3.72         | 3.40          |
| LSTM Neural Network       | 2.65        | 2.20         | 3.50         | 3.25          |

---

## Results

- **Tesla**: The LSTM Neural Network model provided the most accurate predictions, demonstrating its strength in capturing complex patterns in stock price data.
- **Google**: The LSTM Neural Network also performed best, closely followed by Gradient Boosting.

The analysis highlights the effectiveness of deep learning methods for time series forecasting of stock prices, particularly for complex and volatile datasets.

---

## Installation

### Prerequisites
- Python 3.8+
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `statsmodels`, `scikit-learn`, `tensorflow`, `yfinance`

### Setup
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/tesla-google-time-series.git
   cd tesla-google-time-series
