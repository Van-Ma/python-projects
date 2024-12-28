# Cryptocurrency Trading and Prediction Prototype

This is a simple prototype project that explores the world of cryptocurrencies and basic machine learning. The project allows users to:
- View the current price of a selected cryptocurrency.
- Predict the future price of a cryptocurrency using a linear regression model.
- Simulate cryptocurrency trading with a fictional balance.

### Features
1. **Find Current Cryptocurrency Price**: Fetches the current price of a cryptocurrency (such as Bitcoin, Ethereum) from the CoinGecko API.
2. **Predict Cryptocurrency Price**: Uses a linear regression model to predict the price of a cryptocurrency based on historical price data from the past `n` days.
3. **Simulate Cryptocurrency Trading**: Allows users to buy or sell a cryptocurrency with a simulated balance.

### How It Works

- **API Integration**: The project uses the CoinGecko API to fetch real-time cryptocurrency data (prices and historical prices).
- **Linear Regression**: A simple linear regression model is used to predict future cryptocurrency prices based on historical price data. The model trains on the past `n` days of data and predicts the price for the next 5 days.
- **Trading Simulation**: Users can simulate buying or selling cryptocurrencies by entering an amount and checking if they have enough balance to execute the trade.

### Why Linear Regression is Used
The linear regression model is used here as a **basic implementation** to practice machine learning. It is a **simple model** that assumes a linear relationship between past prices and future prices, making it easy to understand and implement for beginner projects.

### Limitations of Using Linear Regression for Crypto Predictions
While the linear regression model is a fun and straightforward way to start learning about machine learning, it **should not** be used for real-world cryptocurrency predictions due to the following reasons:

- **High Volatility**: Cryptocurrencies are known for their **extreme volatility**, meaning that price changes can be highly unpredictable and influenced by various factors such as market sentiment, news, and regulatory changes.
- **Non-Linear Patterns**: The relationship between historical prices and future prices is **non-linear** in most cases. Linear regression assumes a linear relationship, which does not capture the complex behavior of crypto markets.
- **External Factors**: Price fluctuations in the crypto market are influenced by various external factors, such as government regulations, market manipulation, technological advancements, and social media trends, none of which are accounted for in this simple model.
- **Model Accuracy**: Due to these complexities, the linear regression model may provide **inaccurate predictions** when applied to real-world data, especially for highly volatile assets like cryptocurrencies.

### Purpose of This Project
This project is a **fun and educational experiment** that introduces the basics of cryptocurrency exploration and machine learning. It's designed to practice **simple machine learning** and familiarize users with basic concepts of cryptocurrency data analysis and trading simulations. It is not intended for actual trading or financial decision-making.

### Requirements

To run this project, you need the following Python packages:
- `requests`: For fetching data from the CoinGecko API.
- `numpy`: For numerical operations.
- `sklearn`: For implementing the linear regression model.
- `matplotlib`: For plotting data and predictions.

You can install the required packages using:
```bash
pip install requests numpy scikit-learn matplotlib
