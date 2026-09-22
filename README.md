# Stock Market Prediction using LSTM

A time-series forecasting project that uses a Long Short-Term Memory (LSTM) neural network to predict stock closing prices from historical market data.

## Project Overview

This project demonstrates a complete machine-learning workflow for stock-price time-series forecasting:

1. Load historical stock-price data.
2. Select the closing-price series.
3. Normalize the data using MinMaxScaler.
4. Create sequential time-window samples.
5. Train an LSTM model.
6. Predict prices on unseen test data.
7. Convert predictions back to the original price scale.
8. Evaluate the model using RMSE.
9. Visualize actual versus predicted closing prices.

## Model

The model uses an LSTM network because LSTMs are designed to learn patterns from sequential/time-series data.

Typical architecture used in the notebook:

- LSTM layer
- Dropout layer
- LSTM layer
- Dropout layer
- Dense output layer

## Dataset

The notebook downloads historical market data using `yfinance`. The example uses Alphabet (Google) stock data and the closing-price column.

The dataset is downloaded when the notebook is executed, so a separate CSV dataset does not have to be uploaded to GitHub.

## Evaluation

The notebook calculates Root Mean Squared Error (RMSE) on the test set.

A previously reported project result was an RMSE of approximately **$4.50** on the test data. The exact value can vary when the data period, library versions, or model settings change, so the notebook's executed result should be used as the final experimental result.

## Technologies Used

- Python
- Jupyter Notebook
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- TensorFlow
- Keras
- yfinance

## Files

- `Stock_Market_Prediction_LSTM.ipynb` — complete implementation
- `requirements.txt` — Python dependencies
- `README.md` — project documentation

## How to Run

1. Install Python 3.10 or 3.11.
2. Install the dependencies:

```bash
pip install -r requirements.txt
```

3. Open the notebook:

```bash
jupyter notebook Stock_Market_Prediction_LSTM.ipynb
```

4. Run the cells from top to bottom.

Internet access is required because the notebook downloads historical market data through `yfinance`.

## Notes

This project is for educational and portfolio purposes. Stock-price predictions are experimental forecasts and should not be treated as financial advice.
