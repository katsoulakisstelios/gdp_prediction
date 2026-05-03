# 📈 Global GDP & GDP per Capita Forecasting using Machine Learning

This project applies multiple **machine learning regression and time-series models** to forecast the GDP and GDP per Capita of over 260 countries and regional aggregates. The goal is to compare traditional regression techniques with modern time-series approaches, evaluate them using appropriate metrics, and identify the best-performing model for macroeconomic forecasting.

---

## 📊 Dataset Overview

* **Total entities covered:** 262 (individual nations + regional groups)
* **Regional aggregates include:** OECD, Sub-Saharan Africa, European Union, and more
* **Target variables:** GDP (USD) and GDP per Capita (USD)
* **Time span:** Multi-decade historical economic data
* **Source datasets:** Global GDP dataset + Population dataset (merged)

The dataset contains annual economic indicators such as total GDP output and population figures, from which GDP per Capita is engineered as a derived feature.

---

## ⚙️ Project Workflow

1. **Data Merging & Cleaning**

   * Consolidated global GDP and population datasets into a unified DataFrame
   * Handled missing values and duplicate records
   * Ensured data integrity across all 262 entities

2. **Feature Engineering**

   * Calculated GDP per Capita as a derived feature from GDP and population data
   * Structured time-series data for compatibility with all model types

3. **Exploratory Data Analysis (EDA)**

   * Inspected dataset structure and data types
   * Visualized GDP trends across countries and decades
   * Identified economic patterns, outliers, and regional disparities
   * Generated interactive dashboards for country-level exploration

4. **Model Training**
   Four models were trained and evaluated across different forecasting horizons:

   * **Linear Regression** — baseline model for identifying general growth trends
   * **Polynomial Regression** — captures non-linear economic cycles and acceleration
   * **ARIMA** (AutoRegressive Integrated Moving Average) — statistical time-series model designed for sequential forecasting
   * **Prophet** (Meta/Facebook) — robust forecasting tool handling seasonality and economic outliers

5. **Model Evaluation**
   Performance was evaluated using:

   * MAE (Mean Absolute Error)
   * RMSE (Root Mean Squared Error)
   * MAPE (Mean Absolute Percentage Error)

6. **Visualization**

   * Static charts using Matplotlib and Seaborn for trend analysis
   * Interactive dashboards using Plotly for dynamic, country-level exploration

---

## 🏆 Results

### Models Compared

| Model | Strengths |
|---|---|
| Linear Regression | Simple baseline; captures overall growth direction |
| Polynomial Regression | Better fit for non-linear economic cycles |
| ARIMA | Strong at short-term time-series forecasting |
| Prophet | Handles seasonality, holidays, and structural breaks effectively |

### Key Evaluation Metrics
* **MAE** — measures average absolute prediction error
* **RMSE** — penalises larger prediction errors more heavily
* **MAPE** — expresses error as a percentage of actual values for comparability across countries

---

## 📈 Key Insights

* No single model outperforms all others across every country and time horizon.
* **ARIMA** performs well for stable economies with consistent historical trends.
* **Prophet** is more robust in the presence of economic shocks and irregular patterns.
* **Polynomial Regression** captures acceleration phases in fast-growing economies better than a linear baseline.
* MAPE is the most informative metric for cross-country comparisons given the vast difference in GDP scale.

---

## 🌍 Practical Applications

* Support policymakers and economists in anticipating future economic output
* Enable cross-country and cross-regional GDP comparisons over time
* Serve as a foundation for more advanced macroeconomic modelling pipelines
* Can be extended into a web tool for real-time GDP forecasting and scenario planning

---

## 🔮 Future Improvements

* Incorporate additional macroeconomic features (inflation, trade balance, unemployment rate)
* Extend forecasting horizon to 10–20 years with uncertainty intervals
* Deploy as an interactive web application with country-level prediction on demand
* Include explainability tools (e.g. SHAP) for regression models
* Experiment with deep learning approaches such as LSTM for long-term time-series forecasting

---

## 📌 Final Remarks

This project demonstrates how a combination of classical machine learning and time-series models can be applied to real-world macroeconomic data. By evaluating multiple approaches and comparing their performance across a diverse set of countries and regions, the project highlights the importance of model selection and domain context in economic forecasting.

---

## 🚀 Technologies Used

* Python
* NumPy, Pandas
* Scikit-learn (Linear & Polynomial Regression)
* statsmodels (ARIMA)
* Prophet (Meta/Facebook)
* Plotly (Interactive Visualisation)
* Matplotlib / Seaborn
* Google Colab
