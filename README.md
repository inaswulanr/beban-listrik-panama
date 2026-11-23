# ⚡ ChronosLab — Time Series Model Intelligence Center

![ChronosLab Banner](assets/banner.png)

**ChronosLab** is an interactive time series analytics dashboard built with **Python and Streamlit**. It provides a unified workspace for exploring time series data, generating forecasts, and evaluating model performance through a combination of modern AI-based forecasting and classical statistical methods.

At its core, ChronosLab uses **Amazon Chronos-Bolt** to investigate how pretrained time series foundation models perform against traditional forecasting approaches. The application features a clean, light-themed interface designed to make model evaluation and forecasting results easier to explore and interpret.

## ✨ Features

### 1. Overview & Exploratory Data Analysis
Get a quick overview of the dataset through key statistics and interactive visualizations.

- Summary statistics and key performance indicators (KPIs).
- Historical time series visualization.
- 30-day moving average to highlight underlying trends.
- Seasonal pattern exploration through hour-of-day and day-of-week heatmaps.

### 2. Model Benchmarking
Compare AI-based forecasting models with classical statistical approaches using a consistent evaluation framework.

The benchmark includes:

- Chronos-Bolt Zero-Shot
- Chronos-Bolt Fine-Tuned
- Seasonal Naive
- Holt-Winters
- Harmonic Regression

Model performance is evaluated using **MAE, RMSE, and MAPE** across three forecasting horizons:

- 24 hours
- 168 hours
- 720 hours

An interactive leaderboard makes it easier to identify how each model performs under different forecasting scenarios.

### 3. Forecast Explorer
Explore forecasting results through interactive visualizations that compare actual observations with model predictions.

- Actual vs. predicted time series plots.
- Probabilistic prediction intervals (P10–P90).
- Forecast exploration across different prediction horizons.
- CSV export for further analysis.

### 4. Residual Diagnostics
Go beyond accuracy metrics and examine how well each model captures the underlying patterns in the data.

Available diagnostic visualizations include:

- Residuals over time.
- Residual distribution histogram.
- Actual vs. predicted scatter plot.
- Hourly error profiles.

These diagnostics help identify systematic forecasting errors and potential patterns that may not be visible from aggregate evaluation metrics alone.

## 📁 Repository Structure

```text
ChronosLab/
│
├── assets/
│   └── banner.png
│
├── README.md
├── app.py
└── requirements.txt
```

## 🛠️ Tech Stack

- **Python** — Core programming language.
- **Streamlit** — Interactive web application framework.
- **Amazon Chronos-Bolt** — Pretrained time series forecasting model.
- **Pandas & NumPy** — Data manipulation and numerical computation.
- **Plotly** — Interactive data visualization.
- **Scikit-learn / Statistical Libraries** — Model evaluation and statistical analysis.

## 🎯 Project Goal

ChronosLab aims to provide a practical environment for understanding and evaluating time series foundation models alongside established statistical forecasting methods.

Rather than focusing solely on prediction accuracy, the project also emphasizes exploratory analysis, forecast uncertainty, and residual diagnostics to support a more comprehensive assessment of forecasting performance.