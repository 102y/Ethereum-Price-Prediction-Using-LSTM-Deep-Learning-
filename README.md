# Ethereum-Price-Prediction-Using-LSTM-Deep-Learning-
Project Overview
This project aims to predict Ethereum's price for the next hour based on historical data using a Long Short-Term Memory (LSTM) model. LSTM is a type of Recurrent Neural Network (RNN) that is particularly effective for time-series forecasting tasks, especially in volatile markets like cryptocurrency.

The project utilizes historical Ethereum data, including features such as open, high, low, close prices, and volume, to train a model that can predict future prices with a focus on hourly forecasts.

Data Source
The dataset used for training the model is taken from Kaggle's "Ethereum Historical Dataset." This dataset includes the following columns:

Unix Timestamp
Date
Symbol (ETH)
Open Price
High Price
Low Price
Close Price
Volume
The dataset is preprocessed to ensure that only the Close price is used as the feature for the model's predictions.

Project Goals
The main goals of this project are:

Accurate Prediction: Predict Ethereum prices for the next hour with high accuracy by training on historical data.
Efficient Model: Develop a model that balances prediction speed with accuracy.
Deep Learning Application: Utilize advanced deep learning techniques like LSTM to capture the time-dependent trends in cryptocurrency prices.
Model Architecture
The model is built using Keras and TensorFlow.
It includes two LSTM layers with 50 units each, followed by Dropout layers to prevent overfitting.
The model is trained for 100 epochs with a batch size of 32.
The optimizer used is Adam, and the loss function is mean squared error (MSE).
Features of the Code
Preprocessing: Data scaling using MinMaxScaler and transformation into time-series sequences.
LSTM Model: A robust deep learning model to capture the complex patterns in Ethereum price movements.
Next Hour Prediction: After training, the model predicts Ethereum's price for the upcoming hour.
Visualization: A graph comparing actual and predicted prices is plotted for visual analysis.
How to Run the Project
Clone this repository:
git clone https://github.com/your-username/ethereum-price-prediction.git
Install the required libraries:

pip install -r requirements.txt
Download the dataset from Kaggle or another source and place it in the project folder.

Modify the path_to_your_file.csv in the code to the location of your dataset.

Run the script:python ethereum_price_prediction.py
View the prediction for the next hour and the graph showing actual vs predicted prices.

Example Output
Predicted price for the next hour: 1800.45 USD
Results
The model provides reasonable predictions based on the training data, but the results may vary depending on the market's volatility and the dataset's quality.

Future Improvements
Incorporate Additional Features: Adding technical indicators such as moving averages or relative strength index (RSI) to enhance prediction accuracy.
