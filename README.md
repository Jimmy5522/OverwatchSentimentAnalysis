# OverwatchSentimentAnalysis

This project scrapes twitter for tweets regarding the popular game Overwatch.
It scrapes for general tweets concerning the game.
It also scrapes tweets related to all 32 playable characters in the game.

The project puts the tweets through processing and sentiment analysis to find out what the most liked
and least liked characters currently are, according to twitter.

Required packages:
  pandas
  tweepy
  nltk
  textblob
  matplotlib
 
Additional requirements:
  This project requires a twitter developer account with elevated access.
  The user must enter the 5 keys related to their account in order for the tiwtter scraper to work.
    
    Keys required:
    app_api_key
    app_api_key_secret
    access_token
    access_token_secret
    bearer_token
  
  These variables can be found at the top of main_overwatch_twitter.ipynb
  
The project will take a while gathering the data, as the project needs to sleep after each query.
This is because tweepy will deny a query if the project makes too many requests in a short amount of time.

Tweets scraped will always be the most recent in the query, so the intended use for this program is to
get a current yield of twitter's opinion.
