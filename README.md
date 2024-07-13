# LSTM Stock Price Prediction

This project implements a Long Short-Term Memory (LSTM) neural network to predict stock prices, specifically for Apple Inc. (AAPL) stock. The model uses historical stock data to forecast future prices.

## Project Overview

The project consists of the following main steps:

1. Data downloading and preprocessing
2. LSTM model creation and training
3. Stock price prediction and evaluation

## Requirements

- Python 3.x
- Libraries: yfinance, pandas, numpy, sklearn, tensorflow, matplotlib

You can install the required libraries using pip:

```
pip install yfinance pandas numpy scikit-learn tensorflow matplotlib
```

## Usage

1. **Data Download and Preprocessing**:
   - The script downloads AAPL stock data from Yahoo Finance for the period 2014-2024.
   - It calculates moving averages (MA5, MA10, MA20, MA50) and normalizes the data.

2. **Creating the Dataset**:
   - The data is transformed into a format suitable for LSTM, using a rolling window approach.

3. **Model Creation and Training**:
   - A 3-layer LSTM model is created and trained on the prepared dataset.
   - The model uses early stopping to prevent overfitting.

4. **Prediction and Evaluation**:
   - The model makes predictions on both training and testing data.
   - Evaluation metrics (MSE, RMSE, MAPE) are calculated and displayed.
   - Actual vs Predicted prices are plotted for visual comparison.

## Results

The model's performance is evaluated using the following metrics:

- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- Mean Absolute Percentage Error (MAPE)

Plots are generated to visualize the actual vs predicted stock prices for both training and testing data.

## Limitations and Future Work

- The model's predictions are based on historical data and may not account for unexpected market events.
- Future improvements could include incorporating sentiment analysis or other relevant financial indicators.
- The model's performance could potentially be improved by fine-tuning hyperparameters or trying different architectures.

## License

This project is open-source and available under the MIT License.

## Contribution

Contributions, issues, and feature requests are welcome. Feel free to check [issues page](https://github.com/yourusername/lstm-stock-prediction/issues) if you want to contribute.

## Disclaimer

This project is for educational purposes only. It should not be used for actual trading decisions. Always consult with a qualified financial advisor before making investment decisions.
