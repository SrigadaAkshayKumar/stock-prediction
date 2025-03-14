# Stock Analyzer

**Deployed in [Stock-Analysis-tool](https://github.com/SrigadaAkshayKumar/stock)**

## Overview
Stock price prediction is a tough problem in financial markets with big implications for investors, traders and financial analysts. Being able to predict future stock prices based on historical trends and market dynamics can lead to better investment strategies and risk management. Traditional statistical methods don’t capture the complex non-linear relationships in financial time-series data.

## Methodology
To tackle this challenge, this study uses a deep learning approach with Long Short-Term Memory (LSTM) networks, a type of recurrent neural network (RNN) designed for sequential data.

### Data Source
The dataset is dynamically fetched from Yahoo Finance (yfinance), focusing on historical closing prices of stocks. The data is preprocessed, normalized using MinMax scaling and structured into sequences to create a time-dependent learning pattern.

### Model Architecture
The LSTM model has multiple layers to capture long-term dependencies in the data, with dropout regularization to prevent overfitting. The model is trained with Adam optimizer and evaluated with Mean Squared Error (MSE) loss function to get accurate predictions.

### Performance Evaluation
The predicted stock prices are compared with actual values using visual plots. The results show that LSTMs can learn patterns in stock price movements and provide good forecasts.

## Future Enhancements
While this approach is promising, stock markets are influenced by many external factors like macroeconomic trends, investor sentiment and geopolitical events which are not captured by historical price data alone. Future enhancements can be:
- Integrating technical indicators, news sentiment analysis and macroeconomic indicators to improve prediction accuracy.
- Exploring advanced deep learning models like Transformer-based architectures, hybrid models and reinforcement learning for better performance in real-time stock forecasting.

## Applications
This study shows the potential of deep learning in financial market analysis and provides a framework for further development in:
- Algorithmic trading
- Portfolio optimization
- Automated investment strategies

The approach can be applied to multiple stocks, indices and asset classes making it a versatile tool for financial applications.

## References

- **Pandas ([**Documentation**](https://pandas.pydata.org/docs/user_guide/missing_data.html)) :** For Data Preprocessing, handling Missing Values
- **Matplotlib ([**Documentation**](https://matplotlib.org/stable/plot_types/basic/index.html)) :** For Data Visualization
- **Time Series Analysis ([**machinelearningmastery**](https://machinelearningmastery.com/time-series-prediction-with-deep-learning-in-python-with-keras/)) :** Understanding Time Series Prediction with Deep Learning
- **Understanding LSTM Model ([**machinelearningmastery**](https://machinelearningmastery.com/how-to-develop-lstm-models-for-time-series-forecasting/)):** How to Develop LSTM Models for Time Series Forecasting

## Installation
To set up the project, follow these steps:

```sh
# Clone the repository
git clone https://github.com/SrigadaAkshayKumar/stock-prediction.git
cd stock-prediction
# Run the application
python app.py
```
