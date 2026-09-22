# Stock Market Prediction using LSTM

A deep learning project that uses a Long Short-Term Memory (LSTM) neural network for stock-market time-series forecasting.

## Project Overview

This project uses historical stock closing-price data to build an LSTM-based forecasting model. The workflow includes data preprocessing, normalization, sequence creation, model training, prediction, and evaluation.

## Objective

- Work with historical stock-market data
- Prepare closing-price data for time-series modelling
- Build an LSTM neural network
- Predict stock closing prices for the test period
- Evaluate predictions using RMSE
- Visualize actual and predicted prices

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- TensorFlow / Keras
- yfinance
- Jupyter Notebook

## Model

The project uses an LSTM neural network with:

- LSTM layers
- Dropout layers
- Dense layers
- Adam optimizer
- Mean Squared Error loss

The model uses the previous 60 trading days as the input sequence for predicting the next closing price.

## Workflow

1. Load historical stock data
2. Select closing prices
3. Normalize the data using Min-Max scaling
4. Create 60-day time-series sequences
5. Split the data into training and testing sets
6. Train the LSTM model
7. Generate predictions
8. Convert predictions back to the original price scale
9. Calculate RMSE
10. Plot actual versus predicted closing prices

## Evaluation

Root Mean Squared Error (RMSE) is used to evaluate the model's prediction error on the test data.

The notebook calculates the RMSE when it is executed.

## Project Structure

```text
Stock-Market-Prediction-LSTM/
│
├── Stock_Market_Prediction_LSTM.ipynb
├── requirements.txt
└── README.md
```

## How to Run

Install the required packages:

```bash
pip install -r requirements.txt
```

Then open:

```text
Stock_Market_Prediction_LSTM.ipynb
```

and run the notebook cells sequentially.

## Note

This project is intended for machine-learning and time-series forecasting practice. Stock-market predictions are uncertain and should not be treated as financial advice.

## Author

**Sinchana**
