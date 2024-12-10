# **Business Forecasting Final Exam**

This repository contains the R code and analysis conducted for the **Business Forecasting Final Exam**. The exam focuses on analyzing and forecasting car sales data using various time series techniques.

---

## **Dataset**
- **Name**: `TOTALSA.csv`
- **Description**: Monthly car sales data in the United States from 2019 to 2024.
- **Columns**:
  1. **Date**: Monthly time periods.
  2. **Sales Units**: Number of cars sold (in millions).

---

## **Analysis Steps**
1. **Data Preprocessing**:
   - Converted `Date` column to a proper date format.
   - Created a time series object for analysis (`sales_ts_window`).

2. **Exploratory Data Analysis**:
   - Visualized time series trends and seasonal patterns.
   - Analyzed summary statistics, seasonal indices, and distributions.

3. **Modeling Techniques**:
   - **Naïve Forecasting**:
     - Baseline model using the last observed value for forecasts.
     - Pros: Simple to implement.
     - Cons: Does not account for trends or seasonality.
   - **Moving Averages**:
     - Used to smooth short-term fluctuations.
     - Highlighted overall trends with different order settings.
   - **Simple Exponential Smoothing (SES)**:
     - Captures the level of the time series using a smoothing parameter.
     - Provides a stable forecast for stationary data.

4. **Residual Analysis**:
   - Evaluated residuals for randomness and patterns.
   - Checked autocorrelation using ACF plots to validate model fit.

5. **Forecasting**:
   - Forecasted sales for the next 12 months using SES and compared it with Naïve forecasts.
   - Generated prediction intervals to account for uncertainty.

---

## **Key Insights**
1. **Seasonality**:
   - The dataset exhibits significant seasonal variations, as revealed by decomposition and seasonal indices.

2. **Best Forecasting Model**:
   - Simple Exponential Smoothing (SES) performed well with:
     - **MAPE**: 4.20% (small percentage error).
     - Residuals: Random with minimal autocorrelation.

3. **Predictions**:
   - The SES forecast stabilizes at **16.13933 (million units)** for the next year, with increasing prediction uncertainty.

4. **Limitations**:
   - Naïve and SES models do not capture trends or seasonality effectively.
   - Advanced models like ARIMA or Holt-Winters are recommended for further improvement.

---

## **How to Run the Code**
1. Clone this repository:
   ```bash
   git clone <repository-url>
