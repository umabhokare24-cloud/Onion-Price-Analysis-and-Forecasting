# Onion-Price-Analysis-and-Forecasting
Time Series Analysis and Forecasting of Onion Prices in Maharashtra using SARIMA and Holt-Winters Models (2013–2024)
# 🧅 Onion Price Analysis and Forecasting (2013–2024)

## 📊 Project Overview

This project focuses on analyzing and forecasting onion prices in Maharashtra using Time Series Analysis techniques. The study examines price volatility, seasonal patterns, and the impact of COVID-19 on onion prices and arrivals.

Using historical market data (2013–2024), predictive models such as SARIMA and Holt-Winters were applied to forecast future onion prices (2025–2026).

---

## 🎯 Objectives

- Analyze long-term trends and seasonal patterns in onion prices
- Study the impact of COVID-19 on prices and arrivals
- Perform statistical comparison using Welch’s t-test
- Build and evaluate SARIMA forecasting model
- Compare SARIMA with Holt-Winters model
- Forecast future onion prices (2025–2026)

---

## 📂 Dataset Information

- Source: https://agmarknet.gov.in
- Total Observations: 1,44,098
- Time Period: 2013–2024
- Region: Maharashtra, India
- Districts Covered: 25
- Markets Covered: 134

### Key Variables:
- District Name
- Market Name
- Variety
- Arrivals (Tonnes)
- Minimum Price (Rs/Quintal)
- Maximum Price (Rs/Quintal)
- Modal Price (Rs/Quintal)
- Reported Date

---

## 🔍 Exploratory Data Analysis (EDA)

Performed:
- Boxplots for price distributions
- Histograms for price concentration
- Scatter plots (Arrivals vs Price)
- Correlation heatmap
- Variety-wise and district-wise comparisons

Key Findings:
- Strong positive correlation between Min, Max, and Modal prices
- Slight negative relationship between arrivals and prices
- Presence of seasonal price spikes
- Right-skewed price distributions

---

## 🦠 COVID-19 Impact Analysis

Data was divided into:
- Pre-COVID: (2013 – March 23, 2020)
- During COVID: (March 23, 2020 – June 15, 2021)
- Post-COVID: (June 15, 2021 – 2024)

Statistical Method Used:
- Welch’s t-test (for unequal variances)

### Results:
- Prices increased significantly during COVID (p < 0.05)
- Prices remained elevated post-COVID
- Arrivals were more stable during and after COVID
- Pune district showed similar patterns with significant price shifts

---

## 📈 Time Series Modeling

### 1️⃣ SARIMA Model

Model Used:
SARIMA (2,1,0)(1,1,1)[12]

Tests Conducted:
- Augmented Dickey-Fuller (ADF) Test
- KPSS Test
- Box-Ljung Test

Results:
- Data showed strong seasonality
- Model captured cyclical patterns effectively
- Good alignment between actual and fitted values
- Forecast indicates slight price increase for 2025–2026

---

### 2️⃣ Holt-Winters Multiplicative Model

- Captured seasonality and trend
- Good short-term forecasting ability
- Residual autocorrelation present (Box-Ljung p < 0.05)

---

## 🏆 Model Comparison

| Model         | Performance |
|--------------|------------|
| SARIMA       | Better fit and handles complex seasonality |
| Holt-Winters | Good seasonal capture but residual autocorrelation present |

Conclusion:
SARIMA (2,1,0)(1,1,1) performed better overall.

---

## 🔮 Forecast (2025–2026)

- Seasonal patterns expected to continue
- Slight upward trend in modal prices
- Increasing uncertainty over longer horizon (widening confidence intervals)

---

## 🛠 Tools & Technologies Used

- R Programming
- forecast package
- tseries package
- ggplot2
- dplyr
- Time Series Analysis
- Statistical Hypothesis Testing

---


