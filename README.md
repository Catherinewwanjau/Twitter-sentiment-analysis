# Twitter Sentiment Analysis

# Introduction

In today's digital landscape, social media platforms like Twitter serve as a crucial space for customers to express their opinions about products and brands. This project focuses on analyzing tweets related to Apple and Google products to gauge public sentiment, identify trends, and extract actionable insights.

By leveraging Natural Language Processing (NLP) techniques, we process and classify tweets into sentiment categories (positive, negative, and neutral) to help brands enhance customer engagement and refine their strategies.

# Objectives

* Understanding Customer Sentiment: Analyze tweets to determine how consumers perceive Apple and Google products.
* Identifying Trends: Recognize sentiment patterns over time to inform marketing and product strategies.
* Developing a Sentiment Classification Model: Train models to categorize tweets accurately.
* Enhancing Decision-Making: Provide data-driven insights to improve customer satisfaction and brand loyalty.

# Dataset

The dataset used in this project consists of tweets mentioning Apple and Google products. It contains:
* tweet_text: The actual tweet content.
* emotion_in_tweet_is_directed_at: The brand or product mentioned.
* is_there_an_emotion_directed_at_a_brand_or_product: The sentiment associated with the tweet (Positive, Negative, Neutral).

# Data Preprocessing

* Checked for duplicates and missing values.
* Renamed columns for better readability.
* Imputed missing values with "unknown" for product mentions.
* Performed text cleaning (removing URLs, mentions, special characters, and stopwords).
* Tokenized and vectorized text using TF-IDF.

# Model Training and Evaluation
Machine Learning Models Used and Performance:

1. Logistic Regression
Accuracy : 0.6672
Precision:  0.6514
Recall: 0.4547
F1-Score: 0.4629

2. Random Forest Classifier
Accuracy : 0.6734
Precision:  0.6310
Recall: 0.4762
F1-Score: 0.4957

3. XGBoost Classifier
Accuracy : 0.6633
Precision:  0.6057
Recall: 0.4621
F1-Score: 0.4789

Best Performing Model: Random Forest achieved the highest accuracy and F1-score, making it the most robust choice for sentiment classification in this dataset.

# Hyperparameter Tuning

We performed hyperparameter tuning using GridSearchCV for all models, optimizing parameters like C for Logistic Regression, max_depth for Random Forest, and learning_rate for XGBoost.

# Key Insights and Recommendations

* Sentiment Distribution: The data suggests a balanced mix of positive and negative sentiments.
* Low Recall Across Models: Further optimization is needed to improve the identification of positive sentiments.
* Future Enhancements:
  1. Implement deep learning models (LSTMs, BERT) for better sentiment classification.
  2. Use advanced feature extraction methods like Word2Vec or GloVe.
  3. Incorporate real-time tweet analysis and sentiment tracking.

# Installation & Usage

1. Clone the repository:

2. Install dependencies:

pip install -r requirements.txt

3. Run the analysis:

python sentiment_analysis.py

# Conclusion

This project successfully developed sentiment classification models for analyzing consumer sentiment towards Apple and Google products. The insights can be leveraged for marketing, brand positioning, and customer engagement strategies.


