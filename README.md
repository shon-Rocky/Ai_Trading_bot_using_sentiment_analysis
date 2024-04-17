# Trading Bot

This is a trading bot built using the Alpaca API for backtesting and live trading. The bot uses the FinBERT model for sentiment analysis on news related to the stock being traded.

## Getting Started

### Dependencies

* Python 3.10
* Alpaca API
* FinBERT
* LumiBot

### Installing

1. Clone the repository
```
git clone https://github.com/shon-Rocky/Ai_Trading_bot_using_sentiment_analysis.git
```
2. Navigate to the project directory:

```
cd Ai_Trading_bot_using_sentiment_analysis
```
3. Create a virtual environment
```
python3 -m venv venv
source venv/bin/activate
```
4. Install the dependencies
```
pip install -r requirements.txt
```
5. Create .env file in directory and set key
```
 API_KEY=your_api_key
 API_SECRET=your_api_secret
```

### Running

1. Run the backtesting
```
python main.py
```
2. Run the live trading
```
python main.py --live
```

## Backtesting example

### Back test Chart

![Screenshot (311)](https://github.com/shon-Rocky/GPT-Analyst/assets/140310009/e2d58db8-ebac-4f39-9106-d21f43337ed3)

### Strategy compared to SPY

![image](https://github.com/shon-Rocky/GPT-Analyst/assets/140310009/8c1e1346-6f64-49ad-b889-455580d28034)



## Sentiment Analysis

The sentiment analysis is done using the FinBERT model. The news related to the stock is fetched from the Alpaca API and then passed to the FinBERT model for sentiment analysis.

## Trading Strategy

The trading strategy is based on the sentiment analysis. If the sentiment is positive and the probability is high, the bot buys the stock. If the sentiment is negative and the probability is high, the bot sells the stock.

## Authors

* **Shonmon Rcokey** - *Initial work* - [Your GitHub](https://github.com/shon-Rocky)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Alpaca API for the backtesting and live trading
* FinBERT for the sentiment analysis
* LumiBot for the framework
