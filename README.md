# Netflix Stock Prediction Using LSTM

## Project Overview


This project predicts the future stock price of Netflix (NFLX) using Long Short-Term Memory (LSTM), a type of Recurrent Neural Network (RNN). The stock prices are predicted based on historical data from the dataset NFLX.csv.

We chose LSTM because it is specifically designed to handle sequential data (like time series), making it perfect for stock price prediction. The model looks at the past 60 days of stock prices to make future prediction

## Project Goals

- Predict future Netflix stock prices using the LSTM model.
- Use Exploratory Data Analysis (EDA) to understand the data.
- Visualize the predictions against real stock prices.
- Analyze the price movement (up or down) with a confusion matrix.

## Why LSTM?

Stock prices change over time, and LSTM can "remember" patterns in these changes because it uses past information to predict future values. This makes it ideal for time series forecasting, where each data point is influenced by its previous points

## Dataset
The dataset used is NFLX.csv, which includes Netflix stock price data. The main column we focus on is the Close price (the final price a stock is traded at during a market session).
###  Dataset Features:
- Date: The date of the stock price.
- Close: The stock's closing price for each day.

## Model Explanation
- LSTM Model: The model uses 2 LSTM layers with 50 units each, followed by dropout layers to prevent overfitting. A final Dense layer predicts the stock price.
- Loss Function: The model uses Mean Squared Error (MSE) as the loss function, which measures how well the model predicts the actual stock price.
- Training: The model trains on 80% of the data, while 20% is used for testing

##  Accuracy
While LSTM performs well in stock prediction, the accuracy can vary depending on market volatility and other factors. In real-world scenarios, the accuracy typically hovers around 60-80%, which is acceptable for stock prediction tasks. Our goal is to minimize prediction error and achieve an accuracy of over 70%.

The model can be improved by adjusting hyperparameters or using additional features (like trading volume, news sentiment, etc.), but even with basic data, the model can provide good short-term predictions.

## How the Project Helps in Real Life
This project provides an insight into how machine learning models like LSTM can assist traders and investors:

Investment Decisions: Traders can use predictions to decide whether to buy or sell stocks.
- Trend Analysis: The model helps in spotting potential upward or downward trends.
- Financial Planning: Investors can use stock price predictions for long-term investment strategies.
By predicting future stock prices, this project helps reduce investment risks and improve decision-making.


## Contributing
- Feel free to open issues or submit pull requests if you find any bugs or have suggestions for improvements.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Author
Developed by [MD Rashidul Islam](https://github.com/mrirashid/)

