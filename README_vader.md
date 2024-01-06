
# Guardian Articles Sentiment Analysis Model

## Introduction
This repository contains the code and model for sentiment analysis on Guardian articles related to the COVID-19 pandemic inquiry.

## Model
The final sentiment analysis model is based on VADER sentiment intensity analysis.

### How to Use the Pickled Model
1. Install the required libraries: `pip install pandas nltk`
2. Load the pickled VADER analyzer in your Python script or notebook:
    ```python
    import pickle
    from nltk.sentiment import SentimentIntensityAnalyzer

    with open('final_model_vader.pkl', 'rb') as model_file:
        vader_analyzer = pickle.load(model_file)
    ```
3. Use the loaded VADER analyzer to analyze text sentiment:
    ```python
    text = "Your sample text here."
    sentiment_score = vader_analyzer.polarity_scores(text)
    print("Sentiment Score:", sentiment_score['compound'])
    ```
Feel free to contact the author for any questions or clarifications.
