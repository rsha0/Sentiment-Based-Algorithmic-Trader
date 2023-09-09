
# Sentiment Based Algorithmic Trading

This project selects a stocks from the S&P500 index and filters them by public sentiment towards them. Following this, 3 different trading strategies are tested against these stocks: breakout, long bias and momentum strategies. To visualise the returns, there is a function which can plot out line curves for each strategy. 

The strategy which provides the highest return along with the strategy which has the lowest risk are both returned to the user.


## API Used: Alpha Vantage 

#### Get sentiment

```python
import requests

# replace the "demo" apikey below with your own key from https://www.alphavantage.co/support/#api-key
url = 'https://www.alphavantage.co/query?function=NEWS_SENTIMENT&tickers=AAPL&apikey=demo'
r = requests.get(url)
data = r.json()

print(data)
```

#### For more Alpha Vantage API actions, click link below.

```html
  https://www.alphavantage.co/documentation/
```



## Authors

- [@RaymondShao](https://github.com/rsha0)


## Features

- Average stock sentiment function using Alpha Vantage API
- Sorting stocks by sentiment function
- Breakout Strategy Algorithm
- Long Bias Strategy Algorithm
- Momentum Strategy Algorithm
- Plots returns for each strategy
- Obtains strategy with the highest returns along with strategy that has the lowest risk



## 🛠 Skills
Python, Pandas, Matplotlib, Yfinance, Alpha Vantage API, Data Analysis


## Returns of Different Strategies Example

![](TradingAlgReturns.jpg)

## References
1. Kaabar S., 'A Simple Breakout Trading Strategy in Python', published October 3rd 2020, retrieved March 24th 2023: <https://towardsdatascience.com/a-simple-breakout-trading-strategy-in-python-eb043b868d8e>
2. NeuralNine, 'Algorithmic Trading Strategy in Python', published January 15th, retrieved March 25th 2023: <https://www.youtube.com/watch?v=dO0NM_SzWfI>
3. Peake C.F., 'Momentum Strategies (Digest Summary)', published August 1st 1997, retrieved March 24th 2023: <https://www.cfainstitute.org/en/research/cfa-digest/1997/08/momentum-strategies-digest-summary#:~:text=Abstract,after%20controlling%20for%20the%20other.>
4. PREQUIN,'Hedge Fund Strategies', publishing date unknown, retrieved March 25th 2023: <https://www.preqin.com/academy/lesson-3-hedge-funds/hedge-fund-strategies#:~:text=This%20strategy%20creates%20a%20hedge%20against%20market%20factors.&text=Long%2Dbias%20funds%2C%20on%20the,depending%20on%20its%20asset%20allocation.>
5. QuantProgram, 'Algorithmic Trading Python 2023 - FULL TUTORIAL Beginner, first uploaded January 25th 2022, retrieved March 24th 2023: <https://www.youtube.com/watch?v=GDMkkmkJigw&t=0s>

