# stock_price_prediction

* Run data compiler to get csv files for the data, then run the investor guide notebook in order to recreate the results

### Using Technical Analysis to Create Algorithmic Trading Signals

Create buy and sell signals based on multiple technical indicators. 4 prominent indicators were utilized measuring varying attributes of stock price movement.

* Kaufman Adaptive Moving Average: price trend indicator with signals made using crossover strategies

* Relative Strength Index (RSI): Measure of price momentum with signals made based on the RSI reaching certain thresholds

* On-Balance Volume: Stock volume indicator with signals based on whether there is more buy or sell volume

* Average True Range (ATR): Volatility indicator with signals based on whether price deviates away from previous volatility levels

Using the yearly returns and volatility of stocks, clustering can be implemented to group equities based on these characteristics. We can also use this to see how other metadata relating to the company groupings can be used ot find patterns in company performance.

Using LSTM recurrent neural networks, stock price direction can be accurately predicted with a moving window of 60 days. The LSTM model takes every 60 days of data to predict the value for the next day. This allows it to accurately gauge trend movements for a larger period of time, thus making it more accurate as compared to traditional time series methods such as (S)ARIMA. Trading strategies can then be analyzed on predicted data and compared to the actual results to see if performance is close to reality.

Final backtesting is then done on Quantopian to see potential returns and sharpe ratio of an investment over a 2 year period with a low base capital of $5000 to account for survivorship bias.

