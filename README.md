# 🚗 Traffic Volume Forecasting in Gorey (Time Series Analysis)

This project develops a predictive model to **forecast vehicle traffic volume** in the town of **Gorey (Wexford County, Ireland)**, using **time series analysis** and **machine learning techniques**.  
The objective is to anticipate traffic intensity every 15 minutes to support **urban transport planning and congestion management**.

---

## 🎯 Objective

- Analyze and model a **real-world time series** of vehicle flow.  
- Compare **classical statistical models** (ARIMA, SARIMA, SARIMAX, Prophet) with **machine learning methods** (Random Forest, Ridge, Decision Tree).  
- Evaluate model performance using **walk-forward validation** and metrics like **MAE, RMSE, and MAPE**.  
- Identify **patterns of seasonality and daily periodicity** in urban traffic.

---

## 🧩 Dataset

**Source:** [Wexford County Council – data.gov.ie](https://data.gov.ie/)  
**Dataset:** *Gorey Road and Pedestrian Traffic in County Wexford*  
**Format:** Excel (`.xlsx`)

The dataset contains vehicle counts in both **Eastbound** and **Westbound** directions on Gorey Main Street, aggregated every 15 minutes.

---

## ⚙️ Methodology

1. **Data preprocessing and exploration**: handling missing data, visualization of daily and weekly patterns.  
2. **Modeling**:
   - Baselines: Naïve, SNaïve, AR Ridge.  
   - Statistical models: ARIMA, SARIMA, SARIMAX, Prophet.  
   - Machine learning: Random Forest, Ridge Regression, Decision Tree.  
3. **Validation**: walk-forward strategy to prevent data leakage.  
4. **Metrics**: MAE, RMSE, MAPE.  

---

## 📈 Results

| Model | Description | Performance Highlights |
|-------|--------------|------------------------|
| **SNaïve** | Simple seasonal baseline | Captures daily seasonality |
| **SARIMA** | Statistical model with 24h periodicity | High accuracy, interpretable |
| **Random Forest** | Non-linear ML model | Best overall MAE ≈ 56.4 |
| **Ridge Regression** | Linear ML model | Stable, interpretable |
| **Prophet** | Additive model | Balanced performance |

**Key findings:**
- The series exhibits **strong daily seasonality** (24h pattern).  
- **Random Forest** achieved the best predictive accuracy.  
- **SARIMAX** provided the highest interpretability and temporal stability.  
- Combining classical and ML models improved both precision and robustness.  

---

## 🧰 Tech Stack

- Python 3  
- Pandas, NumPy, Matplotlib, Seaborn  
- Statsmodels (ARIMA, SARIMAX)  
- Scikit-learn  
- Prophet  

