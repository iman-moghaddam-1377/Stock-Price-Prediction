# 📈 Stock Price Prediction using Transformer Models

![Python](https://img.shields.io/badge/python-3.8+-blue.svg)
![PyTorch](https://img.shields.io/badge/PyTorch-2.0+-EE4C2C.svg)
![HuggingFace](https://img.shields.io/badge/%F0%9F%A4%97-Transformers-yellow)


## 📋 Project Overview
The goal of this task is to forecast stock values over various time intervals using a provided dataset of company stock prices. While transformer models like **BERT** are traditionally used for Natural Language Processing, this project adapts them for financial time-series forecasting.

---

## 🛠️ Implementation Steps

### A) Feature Engineering & Preprocessing
Before training, the data is preprocessed and normalized. In addition to raw price data, we incorporate technical financial indicators to enhance model performance:
*   **MACD** (Moving Average Convergence Divergence)
*   **RSI** (Relative Strength Index)

### B) BERT Model Adaptation
We adapt a pre-trained **BERT** model to receive stock data and predict future values.
*   **Input Windows**: The model is tested using historical data from the past **3, 7, 15, 30, and 90 days**.
*   **Prediction Horizons**: We evaluate the model's ability to predict the stock value for:
    *   The next day.
    *   The next **7 days**.
    *   The next **30 days**.
*   **Evaluation Metric**: Model performance is measured using **MSE** (Mean Squared Error).

### C) Comparative Analysis
To determine the most effective architecture, the experimental setup is repeated and compared across different models:
*   **RoBERTa** (A robustly optimized BERT approach)
*   **LSTM** (Long Short-Term Memory networks)

---

## 📊 Results & Performance
The results section includes a comparison of MSE across different look-back windows and prediction horizons for each model.

---



