# 📊 US Home Price Prediction using Economic Indicators

This project explores the impact of key economic indicators on US home prices using machine learning models like Linear Regression and Random Forest. The dataset spans from 2005 to 2025 and is based on publicly available sources like the S&P/Case-Shiller Home Price Index.

---

## 🧠 Objective

To build predictive models that estimate home prices using key economic variables such as:

- 🏦 Disposable Personal Income (DSPIC96)
- 💸 Mortgage Rate
- 📈 Unemployment Rate (UNRATE)
- 🛒 Consumer Price Index (CPIAUCNS)
- 💰 Federal Funds Rate (FEDFUNDS)

---

## 📂 Dataset Description

| Column Name     | Description |
|-----------------|-------------|
| `observation_date` | Date of the observation (monthly frequency) |
| `CSUSHPISA`     | Target variable – Home Price Index |
| `DSPIC96`       | Real Disposable Personal Income |
| `Mortgage Rate` | 30-Year Fixed Mortgage Rate |
| `UNRATE`        | Unemployment Rate |
| `CPIAUCNS`      | Consumer Price Index |
| `FEDFUNDS`      | Effective Federal Funds Rate |

---

## 🧹 Preprocessing Steps

1. **Drop missing values** to clean the dataset.
2. **Standardize features** using `StandardScaler` to normalize scales.
3. **Train-Test Split** (80-20), without shuffling to retain time-series nature.

---

## 📊 Exploratory Data Analysis (EDA)

- Time series plots for each feature.
- Correlation matrix to check feature relationships.
- Observed trends and seasonal patterns in `CSUSHPISA`.

---

## 🏗️ Model Training

Two models were trained:
- **Linear Regression**
- **Random Forest Regressor**

Both were evaluated on:
- R² Score (Explained Variance)
- MAE (Mean Absolute Error)
- MSE (Mean Squared Error)

---

## 🧪 Evaluation Metrics

| Metric      | Linear Regression | Random Forest |
|-------------|-------------------|---------------|
| R² Score    | 0.9987            | 0.9986        |
| MAE         | 1.53              | 1.65          |
| MSE         | 4.42              | 4.95          |

✅ Both models performed exceptionally well, with Linear Regression slightly ahead in this case.

---

## 📈 Visualization

- **Bar Chart** showing last 12 months of actual vs predicted values.
- Simple and intuitive visuals make it easy for beginners to interpret results.

---

## 📝 Conclusion

- Economic indicators like income, interest rates, and inflation play a major role in home pricing trends.
- The models demonstrate strong predictive power, especially with clean and consistent historical data.

---

## 🚀 Future Work

- Introduce lag features or rolling statistics.
- Use time-series forecasting models like ARIMA or LSTM.
- Deploy as a simple API using FastAPI or Flask.

---

## 👨‍💻 Author

Built by Prathamesh Shete
📧 Email: prathameshshete616@gmail.com  
💼 Role: Data Research / Machine Learning Enthusiast

---

## 📌 Requirements

- Python 3.8+
- pandas, scikit-learn, matplotlib

Install dependencies:
```bash
pip install -r requirements.txt
