# 📈 Time Series Forecasting with LSTM, ARIMA, SARIMA, SARIMAX & Prophet

This project provides a full pipeline for time series forecasting using deep learning and statistical models. It includes data preprocessing, feature engineering, outlier detection, model training, evaluation, and comparison.

---

## 📘 Table of Contents

- [Project Overview](#project-overview)
- [Key Concepts Covered](#key-concepts-covered)
- [Project Structure](#project-structure)
- [Technologies Used](#technologies-used)
- [How to Run](#how-to-run)
- [Evaluation Metrics](#evaluation-metrics)
- [Notes](#notes)
- [References](#references)
- [Contact](#contact)

---

## 📌 Project Overview

In this project (`final.ipynb`), we forecast time series data (like stock prices or sales) using:

- LSTM (Keras/TensorFlow)
- ARIMA
- SARIMA
- SARIMAX
- Prophet

Preprocessing includes handling outliers, missing data, normalization, encoding, feature extraction, and reshaping data for model compatibility.

---

## ✅ Key Concepts Covered

### 🧼 Data Analysis

| Command | Description |
|--------|-------------|
| `df.info()` | Summary of data types and missing values |
| `df.describe()` | Statistical summary |
| `df.isna().sum()` | Count of missing values |

### 📅 Time Series Basics
- **Time Series**: Sequence of observations indexed by time
- **Instance**: Single row of observation
- **Schema**: Structure of dataset (columns, types)

### 📊 Feature Engineering
- Extracting: `day`, `month`, `year`, `dayofweek`
- Lag features
- Rolling statistics

### 🔍 Outlier Detection
- **IQR Method**: Detect values outside Q1−1.5×IQR or Q3+1.5×IQR
- **Z-Score**: Values with Z > 3 or < −3

### ⚖️ Normalization
- **MinMaxScaler**
- **StandardScaler**
- **Z-Score Normalization**

### 🔠 Encoding
- Label Encoding
- One-Hot Encoding

---

## 📁 Project Structure

