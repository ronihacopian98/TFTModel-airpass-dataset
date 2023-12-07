# TFT Model for Darts AirPassengers Dataset

## Overview

This project involves training a Temporal Fusion Transformer (TFT) model using the Darts library to 
forecast future air passenger counts based on historical data.

##Here are some key features and concepts related to the TFT model in Darts:

- Model Architecture:

The TFT model leverages a transformer-based architecture, similar to models used in natural language processing tasks.
It utilizes self-attention mechanisms to capture temporal dependencies in the time series data.

- Input and Output:

The model takes as input a historical time series and any additional features or covariates that might influence the forecast.
The output is a forecasted time series for future time steps.

- Quantile Regression:

TFT supports quantile regression, allowing you to generate prediction intervals along with point forecasts.
You can specify different quantiles to obtain a range of predictions.

- Training Process:

Training involves minimizing a combination of mean absolute error (MAE) and quantile loss functions.
The model learns to predict not just the expected value but also the uncertainty in the predictions.

- Hyperparameters:

Hyperparameters of the TFT model include input_chunk_length, output_chunk_length, hidden_size, lstm_layers, num_attention_heads, dropout, and the number of training epochs.

- Usage in Darts:

To use the TFT model in Darts, you typically create an instance of the TFTModel class and then train it using the fit method.
After training, you can make predictions using the predict method.

## Dataset

The AirPassengers dataset is used for training and evaluation. It includes the monthly total number of airline passengers from 1949 to 1960.

To find more information about the AirPassengersDataset in Darts, you can refer to the official Darts documentation. 

Here's how you can explore it:

#### Darts Documentation:

- Visit the official Darts documentation on GitHub: Darts Documentation.
- Look for sections related to datasets or provided datasets.

####GitHub Repository:

- Explore the Darts GitHub repository: Darts GitHub Repository.
- Check for any specific documentation or code related to datasets, especially - the AirPassengers dataset.


## Prerequisites

- Python 3.6 and later versions.
- Darts library.

## Installation

!pip install Darts

## Model Configuration
Input Chunk Length: 20
Output Chunk Length: 10
Hidden Size: 100
LSTM Layers: 1
Num Attention Heads: 4
Dropout: 0.1
Number of Epochs: 200


## License
This project is licensed under the MIT License
