# Sales time-series forecasting

Forecast monthly vehicle sales using exponential smoothing with a fixed window and an expanding window.

## Data

`cs_11.csv` is US monthly total vehicle sales from 1976 to 2022 (thousands of units), sourced in the notebook from the U.S. Bureau of Economic Analysis series [TOTALNSA](https://fred.stlouisfed.org/series/TOTALNSA) via the Federal Reserve Bank of St. Louis (FRED). Columns are `date` and `sales`.

## Method

`Time_series_analysis.ipynb` explores the series, then builds exponential smoothing forecasts under a fixed window and an expanding window. It also explores feature selection with RFECV and an expanding window. Forecasts are evaluated with MAPE, MAE, and other absolute-error summaries.

## Findings

From the comparison table in the notebook, expanding-window exponential smoothing had a lower MAPE (7.38) and MAE (85.0) than the fixed-window model (MAPE 8.69, MAE 101.8). These figures are from the committed notebook outputs.

## How to run

```bash
jupyter notebook Time_series_analysis.ipynb
```
