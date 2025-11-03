# Share-Price-Forecasting-Using-Facebook-Prophet
Forecasting future values of a time series using Facebook Prophet, capturing trends, seasonality, and holidays, with evaluation via MAPE, MAE, and RMSE.
# Time Series Forecasting with Facebook Prophet

## Project Overview
This project demonstrates time series forecasting using **Facebook Prophet**, enabling prediction of future values by capturing trends, seasonality, and holiday effects. It provides a complete workflow from data preprocessing to model evaluation.

## Dataset
- Historical daily data
- Preprocessing includes:
  - Converting date column to `datetime`
  - Handling missing values
  - Optional outlier removal
- Sample dataset preview:

| ds         | y    |
|------------|------|
| 2025-01-01 | 100  |
| 2025-01-02 | 120  |
| 2025-01-03 | 115  |

## Methodology
1. **Data Splitting**: Train/test split based on a cutoff date.
2. **Modeling with Prophet**:
   - Trend and seasonality modeling
   - Custom seasonalities (e.g., monthly)
   - Holiday effects (optional)
   - Hyperparameters tuning (`changepoint_prior_scale`, `seasonality_mode`, `fourier_order`)
3. **Forecasting**: Using `make_future_dataframe()` for future predictions.
4. **Evaluation Metrics**:
   - MAPE (Mean Absolute Percentage Error)
   - MAE (Mean Absolute Error)
   - RMSE (Root Mean Squared Error)
5. **Visualization**:
   - Forecast vs actuals
   - Trend and seasonal components

