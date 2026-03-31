Global GDP Growth Forecasting 📈
A machine learning and time-series analysis project to forecast the Gross Domestic Product (GDP) and GDP per Capita of over 260 countries and regional aggregates. This project compares traditional regression techniques with modern time-series models like ARIMA and Facebook Prophet.

🚀 Project Overview
Predicting economic growth is a complex task influenced by numerous global factors. This project implements a robust data science pipeline to:

Merge and Clean Data: Consolidate global GDP and population datasets.

Feature Engineering: Calculate GDP per Capita and perform inflation adjustments using Consumer Price Index (CPI) data.

Predictive Modeling: Compare the accuracy of four different modeling approaches for short-term and long-term forecasting.

Visualization: Generate interactive and static visualizations to track economic trends across decades.

🛠️ Tech Stack
Language: Python

Time-Series Models: Prophet (Meta), statsmodels (ARIMA)

Machine Learning: scikit-learn (Linear & Polynomial Regression)

Data Manipulation: Pandas, NumPy

Visualization: Plotly (Interactive), Seaborn, Matplotlib

📊 Models Explored
The project evaluates the following models to determine the best fit for macroeconomic data:

Linear Regression: Baseline model for identifying general growth trends.

Polynomial Regression: Captures non-linear economic cycles and acceleration.

ARIMA (AutoRegressive Integrated Moving Average): A statistical model specifically designed for time-series forecasting.

Prophet: A robust forecasting tool developed by Meta that handles seasonality and outliers effectively.

📉 Key Features & Workflow
Global Scope: Analyzes data for 262 entities, including individual nations and regional groups like OECD, Sub-Saharan Africa, and the European Union.

Data Integrity: Includes comprehensive checks for missing values and duplicates to ensure model reliability.

Performance Metrics: Models are evaluated using MAE (Mean Absolute Error), RMSE (Root Mean Squared Error), and MAPE (Mean Absolute Percentage Error).

Interactive Dashboards: Utilizes Plotly for dynamic charts that allow users to explore specific country data.
