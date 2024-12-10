# **Business Forecasting Final Exam**

## **Introduction**
This repository contains the final exam submission for the Business Forecasting course. The analysis focuses on forecasting time series data using multiple statistical models and evaluating their performance. The dataset is includes monthly car sales data from 2019 to 2024.

---

## **Contents**
- **Dataset Overview**
  - Monthly sales data from 2019 to 2024.
  - Variables include: `Date`, `Sales Units`.

- **Objectives**
  - Analyze the time series for trends, seasonality, and stationarity.
  - Apply various forecasting techniques.
  - Evaluate and compare forecasting models for accuracy and reliability.

- **Forecasting Methods**
  - **Naive Method**
  - **Simple Moving Average**
  - **Simple Exponential Smoothing**
  - **Holt-Winters Additive**
  - **ARIMA`

---

## **Key Steps**
1. **Exploratory Data Analysis**
   - Time series plots to visualize trends and seasonality.
   - Decomposition of the time series into trend, seasonal, and remainder components.

2. **Model Evaluation**
   - Accuracy metrics: `ME`, `RMSE`, `MAE`, `MPE`, `MAPE`, `MASE`, `ACF1`.
   - Residual analysis for each model:
     - Residual time series plot.
     - Histogram of residuals.
     - ACF of residuals.

3. **Forecasting**
   - Short-term (1 year) and long-term (2 years) forecasts.
   - Confidence intervals for predictions.
   - Comparison of forecasted values across models.

4. **Model Selection**
   - Based on accuracy metrics and residual diagnostics, **Holt-Winters Additive** is the best model for this dataset.

---

## **Results**
- **Best Model**: Holt-Winters Additive.
  - Lowest RMSE, MAE, and MAPE.
  - Effectively captures trend and seasonality.

- **Future Predictions**
  - The time series is expected to show stabilization with seasonal fluctuations over the next two years.

- **Comparison**
  - Holt-Winters Additive outperforms all other models.
  - ARIMA serves as a strong alternative with comparable accuracy.

---

## **Conclusion**
- **Holt-Winters Additive** is the recommended model for accurate and reliable forecasting of the sales data.
- The value of the time series is expected to stabilize with seasonal variations.

---

## **Files**
- **`BF_Final_Exam.Rmd`**: R Markdown file with the complete analysis.
- **`TOTALSA.csv`**: Dataset used for the analysis.
- **`README.md`**: Documentation for the project.

---

## **How to Run**
1. Open the `BF_Final_Exam.Rmd` file in RStudio.
2. Install the required libraries (`forecast`, `ggplot2`, etc.).
3. Run the code chunks step by step to reproduce the analysis and plots.

---

## **Acknowledgments**
- This project was completed as part of the Business Forecasting course.
- Special thanks to the instructor for guidance throughout the course.

---

Feel free to explore the repository and provide feedback!
