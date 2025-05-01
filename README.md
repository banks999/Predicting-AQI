# Air Quality Index (AQI) Prediction for Mumbai

Predicts Mumbai’s Air Quality Index (AQI) using polynomial regression on air quality data (2015–2020) from Kaggle. The model leverages pollutant levels (PM2.5, PM10, NO2, CO, O3) and seasonal effects, with statistical diagnostics and visualizations to validate performance. Built with Python, it supports environmental monitoring and public health strategies.

## Project Overview
This project develops a predictive model for Mumbai’s AQI, a critical metric for air quality affecting public health and urban planning. Using daily air quality data from the [Kaggle Air Quality Data in India dataset](https://www.kaggle.com/datasets/rohanrao/air-quality-data-in-india), it employs polynomial regression to forecast AQI based on key pollutants and seasonal patterns.

- **Objective**: Predict AQI in Mumbai to inform air quality management and policy.
- **Dataset**: Daily air quality measurements (2015–2020) for Indian cities, filtered for Mumbai.
- **Features**: PM2.5, PM10, NO2, CO, O3, their polynomial terms (degree=2), and month dummies for seasonality.
- **Methodology**:
  - Polynomial regression to capture non-linear relationships.
  - Statistical diagnostics: Variance Inflation Factor (VIF) for multicollinearity, Durbin-Watson for independence, Breusch-Pagan for homoscedasticity, and Jarque-Bera for normality.
  - Visualizations: Correlation heatmap, residual plots, Q-Q plot, and actual vs. predicted AQI over time.
- **Technologies**: Python, pandas, NumPy, scikit-learn, statsmodels, Matplotlib, Seaborn.

## Key Results
- **Model Performance**: Accurately predicts AQI, outperforming a baseline (mean AQI) with low prediction error.
- **Insights**:
  - PM2.5 and PM10 are strongly correlated with AQI, highlighting their role as key predictors.
  - Residual diagnostics confirm the model captures most patterns, with minor deviations in normality.
- **Visualizations**: Plots reveal pollutant impacts and model fit, saved in the `plots/` directory.
- **Applications**: Supports air quality monitoring, public health policies, and urban planning initiatives.

## Requirements
- Python 3.8+
- Libraries:
  ```bash
  pip install pandas numpy matplotlib seaborn scikit-learn statsmodels
