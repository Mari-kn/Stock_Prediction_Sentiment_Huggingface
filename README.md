Nvidia Stock and Sentiment Analysis
This project analyzes Nvidia's stock performance in relation to social media sentiment and news sentiment. Using data from Yahoo Finance, Twitter, and news sources, it visualizes stock trends alongside sentiment scores derived from tweets and news articles. The analysis leverages the transformers library for sentiment scoring and plotly for interactive financial visualizations.

This project conducts an analysis of Nvidia's stock (NVDA) by collecting stock price history and merging it with sentiment data from Twitter and financial news. It uses:

Yahoo Finance to retrieve stock data.
transformers library with cardiffnlp/twitter-roberta-base-sentiment-latest model for sentiment analysis.
Plotly to visualize the stock price with overlaid sentiment trends.

Requirements
Install the following dependencies before running the code:

pip install transformers yfinance snscrape pandas numpy matplotlib plotly tqdm


Clone the repository:

git clone https://github.com/your-username/your-repo.git
cd your-repo

How to Run the Code
Run the Jupyter notebook or Python script provided, following the order of steps:

Load and Process Stock Data.
Clean and Prepare Social Media and News Sentiment Data.
Run Sentiment Analysis and Prepare Sentiment Scores.
Generate Visualizations for stock prices and sentiment scores.

# Sentiment analysis on a sample text
sentiment_task("I do not like playing football, but sometimes I enjoy watching football matches")

# Load Nvidia stock data and visualize with sentiment scores
nvda = yf.Ticker("NVDA")
nvda_hist = nvda.history(period="max")
nvda_hist["Open"].plot(figsize=(15,5), title="Nvidia Stock Price")

