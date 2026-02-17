# Cloud Time Series Forecasting

## Overview

This project implements time-series forecasting of cloud resource utilization and billing cost using ARIMA and SARIMA models.

The objective is to predict:

- CPU Utilization
- Memory Utilization
- Cloud Cost

using historical daily data.

---

## Dataset

- Duration: 2 Years
- Observations: 2000 Daily Records
- Features:
  - Usage Start Date
  - CPU Utilization (%)
  - Memory Utilization (%)
  - Usage Quantity
  - Total Cost (INR)

---

## Methodology

1. Time-series indexing by date
2. Train/Test split (80-20)
3. Model implementation:
   - ARIMA (2,1,2)
   - SARIMA (2,1,2)(1,1,1,7)
4. Performance evaluation using:
   - R² Score
   - RMSE
   - MAE
   - MAPE

---

## Results

- SARIMA outperformed ARIMA in seasonal pattern detection.
- High Test R² achieved.
- Low RMSE and MAE values observed.
- Residual diagnostics indicate model stability.

---

## Future Work

- Real-time cloud monitoring integration
- Dashboard visualization
- Automated anomaly detection
- Cost optimization system
