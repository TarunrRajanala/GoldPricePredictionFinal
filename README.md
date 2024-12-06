# ECE 460J Final Project
## Gold Price Prediction
### Outline
Model to Predict Adjusted Closing price of Gold

**Feature Engineering**
Ideally this is what will separate our model from others’ so we need unique features
****Lagged Features****:
  Add lagged versions of the gold price and VIX (e.g., 1-day or 7-day lag).
  Include rolling averages (e.g., 7-day moving average of gold price).
****Derived Features****:
  Calculate volatility metrics: rolling standard deviation of gold prices.
  Create interaction terms: e.g., VIX × Interest Rates.
  Come up with a few more engineering features (using Oil, Currency, etc)
****Temporal Features****:
  Extract features like day of the week, month, quarter, or year.
****Select Relevant Features: Start with a few derived features and expand as needed.****
****Experiment: Test different combinations of derived features to identify the most predictive.****
****Evaluate: Use feature importance metrics (e.g., SHAP or feature coefficients) to identify the most impactful features.****

**Select Models**
****Baseline Model:****
  Start with a simple baseline (predicting the previous day’s price or mean).
****Machine Learning Models:****
  Linear Regression or Ridge/Lasso Regression for interpretability.
  Tree-based models like Random Forest, Gradient Boosting (e.g., XGBoost, LightGBM).
****Advanced Models:****
  Time-series models like ARIMA.
  Neural networks (e.g., LSTMs, GRUs, or Transformer models) for capturing sequential dependencies.
****Train -  normalize/standardize features, tune hyperparameters****
****Evaluate -RMSE, MAE****
****Combine Models - ensemble learning, weighted averages.****



Features

Gold ETF
SP = S&P 500 Index
DJ = Dow Jones Index
EG = Eldorado Gold Corporation (EGO)
EU = EUR USD Exchange rate
OF = Brent Crude oil Futures
OS = Crude Oil WTI USD
SF = Silver Futures
USB = US Bond Rate data
PLT = Platinum Price
PLD = Palladium price
RHO = Rhodium Prices
USDI = US dollar Index Price
GDX = Gold Miners ETF
USO = Oil ETF USO

