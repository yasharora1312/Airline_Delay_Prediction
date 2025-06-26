# ✈️ Flight Delay Analysis & Prediction

A comprehensive project on analyzing and predicting airline delays using data-driven techniques, including exploratory data analysis, feature engineering, classification, and regression modeling.

> 📘 Built as part of a social/business analytics project  
> 📅 Author: **Yash Arora** | 📄 Report: `Report(YashArora).pdf`

---

## 🚀 Project Objective

To explore flight delay data, identify core delay drivers, and build predictive models that forecast:
- Whether a flight will be delayed (Classification)
- Expected delay duration in minutes (Regression)

---

## 🧰 Tech Stack

- **Language:** Python
- **Tools:** Jupyter Notebook, Pandas, NumPy, Matplotlib, Seaborn, Plotly
- **ML Models:** Random Forest, Linear Regression, XGBoost
- **Other:** SMOTE for balancing, Scikit-learn metrics

---

## 📊 Key Project Highlights

### 🔍 Exploratory Data Analysis (EDA)
- Tracked **monthly delay trends**
- Identified **top delay-prone airlines and airports**
- Analyzed **seasonal trends** in delays
- Conducted **root cause analysis** for:
  - Carrier delays
  - Weather-related delays
  - NAS (Air Traffic) issues
  - Late aircraft
  - Security delays

### 📈 Advanced Delay Insights
- Built **correlation heatmaps** to understand feature relationships
- Analyzed **delay rate distributions**
- Computed summary statistics (mean, median, std dev, etc.)

---

## 🏗 Feature Engineering

| Feature | Description |
|--------|-------------|
| `delay_rate` | Proportion of delayed flights |
| `avg_delay` | Average delay in minutes |
| `carrier_prop`, `weather_prop` | Delay shares by cause |
| `carrier_his`, `airport_his` | Historical reliability |
| `is_delayed` | Classification target |
| `target_delay` | Regression target |

Categorical variables like `carrier` and `airport` were encoded.

---

## 🤖 Modeling Approaches

### ✅ **Classification (Will it be delayed?)**
- **Model:** Random Forest
- **Class imbalance handled using:** SMOTE
- **Metrics Used:** Accuracy, Precision, Recall, F1-score

### 🔁 **Regression (How long will it be delayed?)**
- **Model 1:** Linear Regression
  - MAE: 7.20 min
  - MSE: 236.01
- **Model 2:** XGBoost Regressor
  - MAE: 67.65 min
  - RMSE: 91.80 min
  - R² Score: 0.71

---

## 📌 Business Recommendations

1. **Improve controllable delays** (carrier and late aircraft) by managing turnaround time and scheduling buffers.
2. **Optimize network planning** based on seasonal delay patterns.
3. **Target underperforming carriers and airports** for improvement initiatives.
4. **Enhance customer communication** with real-time delay alerts.
5. **Allocate resources dynamically** during peak travel seasons or at high-delay airports.

---
