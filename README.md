# Capstone2

Many theorize that one of the reasons America is struggling with Covid-19 is due to an active anti-science movement. It is difficult to quantify the impact this movement has had on American health, but with NLP we can at least get a better understanding of its ideas. And where better to find an exhaustive supply of extreme views than Twitter? This project demonstrates EDA of pro and anti-mask tweets using Python, KMeans clustering, PCA, and Bayesian Classification.

## The Data

Over 14,000 tweets were scraped that date from 3/1/2020 to 8/21/2020. Each tweet had the hashtag #wearamask or #nomask, which served as proxy labels for the tweet. #wearamask tweets were labeled pro, and #nomask were labeled anti. 

These tweets are included in the tweets_primary directory. The directory also includes a timeline that compares tweets about mask-wearing to US daily Covid-19 cases. 


![Timeline](https://raw.githubusercontent.com/brendanquinn612/Capstone2/master/timeline.png)

## Topic Labeling

Each stance was divided into four topics using KMeans clustering. 

![pos_cluster](https://raw.githubusercontent.com/brendanquinn612/Capstone2/master/c.png)

![neg_cluster](https://raw.githubusercontent.com/brendanquinn612/Capstone2/master/c2.png)

## Tweet Prediction

Naive Bayes Classifiers were used to predict if a given tween was pro or anti-mask. It acheived 86% accuracy over a baseline of 66%.

![Word_clouds](https://raw.githubusercontent.com/brendanquinn612/Masks-on-Twitter/master/clouds.png)
