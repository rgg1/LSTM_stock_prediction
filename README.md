# Stock Price Prediction Using LSTM

This notebook illustrates a machine learning model using a Long Short-Term Memory (LSTM) network to predict the stock prices of a specific company. The example provided here is for Amazon (AMZN), but you can use any company's stock by setting the appropriate ticker.

## Overview

The model takes historical stock price data, including Open, High, Low, and Close prices, and utilizes an LSTM network to predict future stock prices. The data is sourced using the yfinance library, and the LSTM model is implemented using PyTorch.

## Dependencies

The following libraries are required to run the notebook:

- PyTorch
- yfinance
- torch-summary
- matplotlib
- scikit-learn

You can install these dependencies using the following commands:

`!pip install torch`
`!pip install torch-summary`
`!pip install yfinance`
`!pip install matplotlib`
`!pip install scikit-learn`

## How to Use

1. Initialization: Define the stock ticker and the starting date for the data.
2. Data Visualization: The notebook includes comprehensive data visualization techniques that allow you to understand various stock attributes over time. Plots are provided on a daily, weekly, and monthly frequency, as well as moving averages.
3. Data Preparation: The notebook preprocesses the data using MinMaxScaler, normalizing the Open, High, Low, and Close features, and transforms the data into sequences for time series prediction.
4. Model Architecture: An LSTM network is employed to capture the sequential pattern in the data. The network includes 64 hidden units and a fully connected layer to output the predicted values for the Open, High, Low, and Close features.
5. Training and Evaluation: The model is trained using Adam optimization and Mean Squared Error loss function. Training, validation, and test datasets are defined, and the training process includes saving the best model based on validation loss.
6. Prediction: The notebook illustrates how to use the trained model to make predictions on the test set and to forecast the next 10 days' stock prices.

## Results

The notebook includes a plot that visualizes the actual vs. predicted stock prices on the test set, providing a clear comparison of the model's performance.

## Customization

You can customize the model by changing the stock ticker, altering the LSTM architecture, modifying the sequence length, or adjusting the number of epochs.

## Conclusion

This LSTM-based stock price prediction model provides a robust framework to understand and forecast stock market trends. By leveraging PyTorch and state-of-the-art time series modeling techniques, you can adapt this model for various stocks and financial market analysis.

## Disclaimer

This model is intended for educational and research purposes only and should not be used for making actual investment decisions.
