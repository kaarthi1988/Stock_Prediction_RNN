# FB Stock Prices Analysis with RNN

## Project Overview

This project focuses on analyzing Facebook (Meta) stock price data using a Recurrent Neural Network (RNN). The goal is to predict future stock prices based on historical data. The project leverages Python libraries such as Pandas for data handling, Matplotlib for visualization, and TensorFlow/Keras for building and training the RNN model.

## Prerequisites

The following libraries are required to run this project:

- **Pandas**: For reading and manipulating the stock price dataset.
- **NumPy**: For numerical computations.
- **Matplotlib**: For plotting and visualizing the stock prices.
- **TensorFlow/Keras**: To build and train the RNN model.

## Data

The dataset used in this project, `FB-stock-prices.csv`, contains historical stock price data for Facebook. The columns typically include:
- `Date`: The trading date.
- `Price`: The price at which the stock closed on the trading day.

The dataset is processed to fit the requirements of a time series model, with appropriate scaling and reshaping before being passed into the RNN.

## Recurrent Neural Network (RNN)

### Model Architecture

A Recurrent Neural Network (RNN) is employed to capture the temporal patterns in stock price data. RNNs are specifically suited for sequential data such as time series. In this project, the RNN is structured as follows:
- **SimpleRNN Layer**: Captures sequential dependencies in the data.
- **Dense Layer**: A fully connected layer that produces the final output, which is the predicted stock price.

The model is trained to minimize the mean squared error (MSE) between the predicted stock prices and the actual prices.

### Training

The model is trained on the scaled stock price data over multiple epochs. During training, the model learns the underlying patterns in the data that it can use to predict future stock prices.

## Results and Visualization

After training, the model's predictions are compared with the actual stock prices. The results are visualized using Matplotlib to provide a clear comparison between predicted and actual prices over time. This allows for an assessment of the model's performance and its ability to capture trends in stock price movement.

## Conclusion

This project demonstrates the use of an RNN for time series prediction, specifically applied to Facebook stock price data. With further tuning, the model's accuracy can be improved by experimenting with more advanced architectures like LSTMs or GRUs and adjusting hyperparameters. Additionally, more features such as volume or external market indicators can be incorporated to enhance the model's predictive power.
