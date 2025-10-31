# 🌦️ Toronto Climate Trends: Time Series Forecasting (1937–2025)

## 📘 Project Overview  
This project explores **Toronto’s historical climate data** from **November 1937 to July 2025** using **time series analysis and forecasting**. It aims to uncover long-term changes in **temperature, precipitation, snowfall, and wind** — offering data-driven insights for **climate planning and sustainability**.

---

## 🧭 Objectives  
- Analyze nearly 90 years of weather records for Toronto.  
- Identify **trends, seasonality, and anomalies** in the data.  
- Build and evaluate multiple forecasting models.  
- Forecast future temperature patterns and support **environmental preparedness**.

---

## 🔍 Methodology  
1. **Data Preparation** – Loaded and cleaned daily weather data (`weatherstats_toronto_daily.csv`), converted to a time-indexed format.  
2. **Exploratory Data Analysis** – Visualized long-term temperature and precipitation trends, identified missing values and seasonal fluctuations.  
3. **Stationarity Testing** – Used the **Augmented Dickey-Fuller (ADF) Test**, confirming the data is **stationary** (p-value < 0.05).  
4. **Decomposition** – Extracted **trend**, **seasonal**, and **residual** components for interpretability.  
5. **Model Building** – Implemented ARIMA/SARIMA models with tuned parameters, and compared with ML/DL approaches (Random Forest, LSTM).  
6. **Validation & Forecasting** – Evaluated model accuracy and generated forecasts for future years.

---

## 📊 Results  
- ✅ **ADF Test:** Series confirmed stationary (ADF = -5.11, p = 0.0000134).  
- ✅ **Model Fit Summary:**  
  - AIC = 4229.68, BIC = 4264.22 → strong and valid fit.  
  - Significant coefficients: AR(1,2), MA(1), Seasonal MA(12).  
  - Residuals show **no autocorrelation or heteroskedasticity**.  
- ✅ **Validation Metrics:**  
  - **MSE:** 3.18  
  - **RMSE:** 1.78 °C  
  - **MAE:** 1.39 °C  
  → Average forecast deviation under 2 °C, showing strong predictive accuracy.

---

## 🧠 Conclusion  
The ARIMA-based forecasting model performs robustly, capturing both **seasonal and long-term temperature patterns**.  
Residuals behave well with **low forecast error**, making it suitable for practical climate forecasting.  
Overall, the analysis reveals **gradual warming trends** in Toronto and seasonal fluctuations consistent with global climate change.  
Deep learning models (LSTM/GRU) show promise for even longer-term, non-linear forecasting.

---

## 🧰 Tools & Libraries  
`Python`, `Pandas`, `NumPy`, `Matplotlib`, `Seaborn`, `Statsmodels`, `Scikit-learn`, `TensorFlow`
