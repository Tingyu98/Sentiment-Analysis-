# Sentiment-Analysis
DATA 5100 project

Member: Duong, Priyanka, Ting-Yu 


## Problem statement 

Our objective is to identify words in Yelp reviews that are indicative of an exceptionally liked restaurant business, and create a model that could accurately automate this process and adapt to new data inputs. In this process, Yelp reviews are transformed into numerical vectors using Natural Language Toolkit (NLTK)'s vectorization techniques, which convert the textual data into a format suitable for machine learning models. Logistic regression is then employed to analyze the sentiment expressed in the reviews. The model is trained on a labeled dataset, learning to predict whether a review conveys positive or negative sentiment based on the vectorized representation of the text. By combining NLTK's powerful text processing capabilities with logistic regression's ability to make binary sentiment predictions, we can gain valuable insights into the overall sentiment of Yelp reviews, enabling data-driven decisions or apply in other business applications. 

## Data sources 

The Kaggle folder contains 5 json files that display information about the business, check-in, review, tip and user. We will perform a minimal amount of cleaning, but preprocessing is necessary due to its size and to select relevant variables. Two datasets, business and review, are combined to create a comprehensive single dataset. 

Dataset link: https://www.kaggle.com/datasets/yelp-dataset/yelp-dataset 

## Analytical approach 

* Preprocessing (filtering, merging, text formatting) 
* Exploratory data analysis (EDA)
* Vectorization
* Model Training 
* Prediction and regression analysis
  
## Solution technologies 

* json
* pandas
* numpy
* matplotlib
* seaborn
* nltk
* sklearn
   

## Citations

https://www.kaggle.com/code/ambarish/a-very-extensive-data-analysis-of-yelp  

https://medium.com/analytics-vidhya/nlp-getting-started-with-sentiment-analysis-126fcd61cc4a 

https://medium.com/@skillcate/sentiment-analysis-project-with-traditional-ml-nlp-349185bf98dd 

F. Jemai, M. Hayouni and S. Baccar, "Sentiment Analysis Using Machine Learning Algorithms," 2021 International Wireless Communications and Mobile Computing (IWCMC), Harbin City, China, 2021, pp. 775-779, doi: 10.1109/IWCMC51323.2021.9498965.
