# Sentitick

Sentitick project focuses on analyzing financial news articles to extract and summarize key information, as well as to evaluate sentiment related to specific stock tickers. It utilizes natural language processing (NLP) techniques and leverages large language models to create concise summaries of the articles and then generate sentiment-based recommendations.

## Features

- **Article Summarization**: Generate summaries of financial news articles.
- **Sentiment Analysis**: Evaluate sentiment and generate financial recommendations.
- **Performance Analysis**: Compare sentiment-based recommendations with stock performance.

## Usage
Setup Environment: Create a .env file and add your API keys for accessing financial data and language models.
Retrieve Articles: Use the provided functions to fetch and process financial news articles.
Analyze Sentiment: Generate summaries and analyze sentiment to get financial recommendations.
Evaluate Performance: Compare the recommendations with stock performance over specified periods.

## Example usage

# Fetch and process articles
articles = get_news_articles(q='AAPL', from_date='2024-06-30', to_date='2024-07-07')
articles = process_articles(articles, ticker='AAPL')

# Analyze sentiment
recommendations = analyze_article_sentiment(articles, used_field='content')

# Calculate performance
performance = calculate_performance('AAPL', '2024-07-07', '2024-07-14')

## Disclaimer
Note: This project is for educational purposes only and should NOT be used as a financial tool or for making trading decisions. The sentiment analysis and performance metrics provided are not intended as financial advice. Always conduct your own research or consult with a financial advisor before making any financial decisions.