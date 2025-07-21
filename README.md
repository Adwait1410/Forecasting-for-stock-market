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

```
📁 Time-Series-Forecasting/
├── final.ipynb       # Main Jupyter notebook with full implementation
├── README.md         # Project documentation
```

---

## 🧰 Technologies Used

| Tool/Library         | Purpose |
|----------------------|---------|
| Python               | Core programming language |
| Pandas, NumPy        | Data manipulation and numerical operations |
| Matplotlib, Seaborn  | Data visualization |
| Scikit-learn         | Feature scaling, preprocessing, and evaluation |
| TensorFlow / Keras   | Deep learning (LSTM implementation) |
| Statsmodels          | Statistical models (ARIMA, SARIMA, SARIMAX) |
| Prophet              | Time series forecasting library by Facebook |

---

## ⚙️ How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/time-series-forecasting.git
cd time-series-forecasting
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

> If `requirements.txt` is not available, install manually:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn tensorflow keras statsmodels prophet
```

### 3. Run the Notebook

```bash
jupyter notebook final.ipynb
```

---

## 📊 Evaluation Metrics

- **MAE (Mean Absolute Error)**
- **MSE (Mean Squared Error)**
- **RMSE (Root Mean Squared Error)**
- **R² Score (Coefficient of Determination)**

Used to evaluate model prediction accuracy.

---

## 📌 Notes

- Dataset must include a time-based column (e.g., `Date`).
- For Prophet: use `ds` for date and `y` for target value.
- LSTM input must be reshaped to 3D format: `(samples, timesteps, features)`.
- SARIMA and SARIMAX require careful seasonal parameter tuning.

---

## 📚 References

- [Facebook Prophet Documentation](https://facebook.github.io/prophet/)
- [Statsmodels Documentation](https://www.statsmodels.org/)
- [Keras Time Series Example](https://keras.io/examples/timeseries/)
- [Scikit-learn Metrics](https://scikit-learn.org/stable/modules/model_evaluation.html)
- [IQR and Z-Score for Outlier Detection](https://towardsdatascience.com)

---


---

