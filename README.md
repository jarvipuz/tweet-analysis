# tweet-analysis
COMP8240 Applications of Data Science: Twitter Data Analysis

## Overall Goal
Tweets from two users were collected and analyzed following the analysis conducted on Donald Trump's tweets: [Text analysis of Trump's tweets confirms he writes only the (angrier) Android half](http://varianceexplained.org/r/trump-tweets/). For this project, US politician Alexandria Ocasio-Cortez ([@AOC](https://twitter.com/AOC)) and celebrity Kim Kardashian ([@KimKardashian](https://twitter.com/KimKardashian)) were used as examples but the code can be used with any (public) Twitter profiles.

## Data
400 tweets were collected from 2 different Twitter users, 200 from each.  The users were selected such that it is expected that there are some noticeable differences in their tweets.

## Packages Used
* pandas
* numpy
* matplotlib
* seaborn
* re
* collections
* json
* datetime
* tweepy
* nltk
* sklearn

## Method
1.	Used pandas to plot the posting times of the tweets for the two users that aims to distinguish them.
2.	Used pandas to construct a bar chart of the proportions of tweets for each of the two users that contain pictures or links.
3.	Used pandas to construct a histogram of the number of hashtags in tweets for each of the two users.
4.	Calculated the log odds ratio (see Donald Trump's tweet analysis for example) for each word used in the set of tweets, and listed the 20 words most strongly associated with each of the two users. The tweets were processed such that stopwords and mentions were removed.
5.	Used the nltk vader module to calculate the sentiment of each tweet, and then for each of the two users, calculate the average 'compound' sentiment for all their tweets.
