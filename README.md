# Steam Game Review Sentiment Analysis

### Introduction / Motivation
Steam is a video game digital distribution service for PC platform. The products on Steam are rated by players in the form of comments or reviews. These reviews can be a good indicator for other players how good the product is. In this case, those reviews can be used to do sentiment analysis using machine learning. Sentiment analysis can be useful to monitor product sentiment from player feedback.

### About the Data
This project used 'Steam Reviews' dataset that was downloaded from [Kaggle](https://www.kaggle.com/datasets/andrewmvd/steam-reviews).
'Steam Reviews' dataset has about 6.4 million rows and 6 columns (`app_id`, `app_name`, `review_text`, `review_score`, `review_votes`). Of the 6 features, only `review_text` and `review_score` features are used. Also 'Steam Reviews' dataset is an unbalanced dataset.

### Goal
Goal of this project is to create model that can classify positive sentiment (positive review) and negative sentiment (negative review) base d on dataset that already mentioned above. There will be a performance comparison between 3 model: **Logistic Regression, Multinomial Naive Bayes and Random Forest Classifier**. The 3 models will then be evaluated using **F1-Score and ROC-AUC score**.

## Conclusion / Result

Through this project, all 3 model was able to be fitted where Logistic Regression model produces highest F1-Score and ROC-AUC around 0.8 and 0.77, respectively. Multinomial Naive Bayes had the lowest F1-Score of 0.49 and ROC-AUC of 0.52 while Random Forest model had F1-Score of 0.63 and ROC-AUC of 0.60. The result of the three model are presented below in the form of a table:

|Model|F1-Score|ROC-AUC|
|---|---|---|
|Logistic Regression|**0.8003524874981843**|**0.7682825262448604**|
|Multinomial Naive Bayes|0.488701288813998|0.5182127762195058|
|Random Forest|0.6270504131555521|0.6009745157160985|

---
### You can check model [here](https://nbviewer.org/github/Layrin14/Steam-Game-Reviews-Sentiment-Analysis/blob/master/Steam%20Game%20Review%20Sentiment%20Analysis.ipynb)

