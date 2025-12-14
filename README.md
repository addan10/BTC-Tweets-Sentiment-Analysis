📈 Crypto Tweet Sentiment Analysis (Bullish vs Bearish)

This project explores how cryptocurrency market sentiment is reflected through Twitter (X) posts by classifying tweets as Bullish or Bearish using Natural Language Processing (NLP) techniques.

The motivation behind this work is to analyze how influential tweets can shape market perception and potentially impact crypto price movements.

🔍 Project Overview

Social media plays a critical role in the cryptocurrency ecosystem. Traders and investors often react instantly to tweets posted by influential figures or communities.
This project builds an end-to-end NLP pipeline that:

Cleans and preprocesses crypto-related tweets

Converts text into numerical representations

Trains multiple NLP models for sentiment classification

Predicts sentiment of unseen tweets in real time

The system demonstrates a comparison between classical NLP pipelines and neural sequence models.

📊 Dataset

The dataset used in this project consists of Bitcoin-related tweets labeled with sentiment information.

🔗 Dataset Link:
https://huggingface.co/datasets/ckandemir/bitcoin_tweets_sentiment_kaggle

After preprocessing, the dataset is converted into a binary classification task:

Bullish → Positive sentiment

Bearish → Negative sentiment

Neutral tweets are excluded to maintain clarity and balance.

🧠 Models Implemented
Classical NLP Models

Bag-of-Words + Logistic Regression

TF-IDF + Linear SVM

Word2Vec (Averaged) + Logistic Regression

Neural NLP Model

Simple Recurrent Neural Network (RNN) with pretrained embeddings

Each model is evaluated using:

Accuracy

Precision

Recall

F1-Score

Confusion Matrix

🔬 Key Insights

TF-IDF with linear classifiers performs strongly on short, noisy text like tweets.

Dense embeddings capture semantic meaning but may lose word order when averaged.

Sequence-aware models (RNNs) help with negation and context but require more computation.

Increased model complexity does not always guarantee better performance.
