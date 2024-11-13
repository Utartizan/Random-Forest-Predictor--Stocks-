# Stock Price Prediction App
Welcome to the Stock Price Prediction App! This app allows users to select a stock from the top 100 companies within the S&P 500 and predict future prices based on historical data.

# Features
Stock Selection: Choose a stock symbol (e.g., AAPL, AMZN, BLK) from a dropdown menu.

Date Range: Set the date range for analysis, with a default range from January 1, 2022, to the current date.

Training Data Percentage: Adjust the training data percentage (40-90%) for model training, with suggested ranges based on stock volatility and time span.

Prediction Output: Generate predictions for the next 30 days, with historical prices in red, predicted prices in cyan, and future predictions in blue.

# Methodology

The app leverages a Random Forest model, trained on historical stock prices up to 30 days before the selected end date, to provide time-series predictions.

Training Data: Uses historical stock prices.

Testing Data: Last 30 days of the selected date range.

Forecasting: Provides a 30-day forecast.

# Interpretation of Results

Plot: Displays historical and predicted stock prices. Actual prices are shown in blue, while predicted prices are in red.
Metrics:

Mean Absolute Error (MAE): Indicates the average error between predicted and actual prices.

Root Mean Squared Error (RMSE): Measures the average of squared differences between predicted and actual prices.

R-Squared: Shows the goodness of fit, representing the model's accuracy.

# Acknowledgments
This app was developed using the following R packages: shiny, quantmod, forecast, caret, and ggplot2. Special thanks to my professor, Artur Semeyutin, and the resources below:

R Script Markdown Cookbook by Yihui Xie, Christophe Dervieux, Emily Riederer

Introduction to Machine Learning with R by Laurent Gatto

Quantmod Package for R

ShinyWidgets Documentation

All stock price data is sourced from Yahoo Finance using the quantmod package.
