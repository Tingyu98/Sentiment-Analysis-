# Sentiment-Analysis

## Overview
This project applies **Natural Language Processing (NLP)** and **machine learning** techniques to analyze restaurant reviews from Yelp. By extracting a subset of reviews from the large-scale Yelp dataset, the study explores sentiment drivers and builds predictive models for automated classification of positive and negative sentiments. The analysis provides insights into customer experiences and service quality, supporting restaurants and platforms in enhancing customer satisfaction.

## Goal
* Identify words and phrases that drive positive or negative customer sentiment.
* Build machine learning models to predict sentiment from textual reviews.
* Automate sentiment classification for scalability and adaptability to new data.
* Provide actionable insights to help businesses improve service and customer experience.
* Dataset link: https://www.kaggle.com/datasets/yelp-dataset/yelp-dataset 

## Methodology

* **Data Sources** – Yelp Open Dataset (Kaggle), combining business and review JSON files into a comprehensive dataset (~6M reviews total, 150K selected for training/analysis). 
* **Data Preparation**
  * Filtering reviews for restaurants only.
  * Cleaning and preprocessing text (tokenization, lowercasing, stop-word removal, lemmatization).
  * Merging metadata (business category + review text).
* **Exploratory Data Analysis (EDA)**
  * Distribution of review ratings, business categories, and text length.
  * Visualization of word frequencies and sentiment-related terms.
  * Identification of class imbalance (positive vs negative reviews).
* **Feature Engineering** - TF-IDF vectorization using NLTK & scikit-learn.
* **Modeling**
  * Logistic Regression – Baseline model for binary sentiment prediction.
  * XGBoost – Gradient boosting classifier optimized via hyperparameter tuning.
* **Evaluation**
  * Performance measured using F1-score, accuracy, and precision-recall tradeoffs.
  * Feature importance analysis to identify key drivers of sentiment.
* **Tools & Libraries**
  * Python (pandas, numpy)
  * NLP: NLTK, scikit-learn
  * Visualization: matplotlib, seaborn
  * Modeling: XGBoost, Logistic Regression
  
## Results & Insights

* **Model Performance** –
  * Logistic Regression with TF-IDF achieved strong baseline results.
  * XGBoost with TF-IDF reached 94% F1-score, outperforming logistic regression.
* **Key Drivers of Negative Sentiment** – Terms such as “time” and “order” were strongly associated with poor customer experiences (e.g., long wait times, incorrect orders).
* **Scalability** – The trained models generalize well and adapt to new incoming review data, demonstrating robustness for real-world deployment.

## Application / Recommendation
* **Business Use Cases**
  * Restaurants can monitor real-time sentiment to identify service pain points.
  * Platforms like Yelp can automate review flagging and sentiment summaries.

* **Recommendations**
  * Focus on reducing service delays and order issues, as these terms drive negative sentiment.
  * Integrate sentiment dashboards for managers to act on insights proactively.
 
## Future Work
  * Expand feature set by integrating word embeddings (Word2Vec, BERT) for richer semantic understanding.
  * Extend to multi-class sentiment classification (very positive → very negative).
  * Deploy as a real-time application (API or dashboard) for automated monitoring.

## Citations

https://www.kaggle.com/code/ambarish/a-very-extensive-data-analysis-of-yelp  

https://medium.com/analytics-vidhya/nlp-getting-started-with-sentiment-analysis-126fcd61cc4a 

https://medium.com/@skillcate/sentiment-analysis-project-with-traditional-ml-nlp-349185bf98dd 

F. Jemai, M. Hayouni and S. Baccar, "Sentiment Analysis Using Machine Learning Algorithms," 2021 International Wireless Communications and Mobile Computing (IWCMC), Harbin City, China, 2021, pp. 775-779, doi: 10.1109/IWCMC51323.2021.9498965.
