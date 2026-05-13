# TweetSense

TweetSense compares two sentiment-classification methods for noisy Twitter text:

1. Traditional ML: preprocessing, TF-IDF, and classic classifiers.
2. Hugging Face classification: fine-tuned Twitter RoBERTa.

## Setup

```bash
pip install -r requirements.txt
```

The notebook is configured to read the dataset from:

- `C:\Users\nwf15\OneDrive\Desktop\NLP_Project\twitter_training.csv`
- `C:\Users\nwf15\OneDrive\Desktop\NLP_Project\twitter_validation.csv`

Dataset: https://www.kaggle.com/datasets/jp797498e/twitter-entity-sentiment-analysis

The Hugging Face section fine-tunes `cardiffnlp/twitter-roberta-base`. The first run may download the model; after that it runs locally from the Hugging Face cache.

## Main Notebook

Open and run:

- `TweetSense_Sentiment_Comparison.ipynb`

The notebook saves the best traditional TF-IDF model package to:

- `models/tweetsense_tfidf_model.joblib`
