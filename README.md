Using Twitter Data to Create a Stock Portfolio
-

Intuition:
-Interaction with posts on Twitter related to stocks may indicate trends related to the growth of that stock
-Large interaction can indicate negative trends as well (effects are not as strong)
-We want to find a way to rank stocks based on their monthly engagement levels and buy the top X amount 
-Choosing more should lessen the effects of cases where a stock has high engagement but is negatively trending

Data
-For data, we have the daily amount of likes, comments, impressions, etc, of tweets including hashtags of just under 100 of the most liquid stocks 
-We tested a variety of combinations between these predictor variables to determine what the best proxy for sentiment analysis was

Building Portfolio

DNN Implementation
-A DNN was created with 4 predictors of twitter data to predict the closing stock price of each day.
-Using keras
-In progress: The stocks with highest predicted increase from previous closing day will be valued higher in portfolio
