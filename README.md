# contextual_multiarmed_bandits
First Price Auctions Bid Optimization with Contextual Multiarmed Bandits (Vowpal Wabbit)

Title: First Price Auctions Bid Optimization with Contextual Multiarmed Bandits (Vowpal Wabbit)

We use MultiArmedBandits to find the best bidding strategy for real estate bidding. The project involves several stages:
0 - back engineer home sales dataset based on tax roll data
1 - engineer additional features based on property, geospatial, and time-series fields and use RandomForests to select the best features.
2 - use probabilistic regression models NGBoost, Quantile Gradient Boosted Decision Trees, and Quantile Random Forests to predict future median home prices and confidence intervals. We train on past data and iteratively predict home prices for the coming four weeks to prevent any data leaks.
3 - We use Wowpal Vabbit to set up multi-armed bandits' online training, which uses future predictions to find the optimal bidding strategy over 16,000 experiments. 

We show that MABs select different strategies depending on the accuracy of the probabilistic models.
