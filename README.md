# Objective

This project involves analysis for an online game store, which sells video games worldwide. The goal is to analyze user and expert reviews, game genres, platforms (such as Xbox or PlayStation), and historical sales data to identify patterns that determine whether a game will be successful or not. This analysis will help in identifying promising projects and planning advertising campaigns.

In this project I test the following hypotheses:

1. Average user ratings for Xbox One and PC platforms are the same.
2. The average user ratings for the Action and Sports genres are different.

# Data

- Name
- Platform
- Year_of_Release (Year of release)
- Genre (Genre)
- NA_sales (North American sales in millions of US dollars)
- EU_sales (European sales in millions of U.S. dollars)
- JP_sales (Japan sales in millions of U.S. dollars)
- Other_sales (sales in other countries in million US dollars)
- Critic_Score (maximum of 100)
- User_Score (maximum of 10)
- Rating (ESRB)

# Library

Pandas, numpy, seaborn, scipy, matplotlib


# Conclusions

* This study described the DataFrame data and made corrections to the data type and duplicate elimination. The data was refined and a new variable, "all_sales," was created, which is the sum of sales in all regions.

* Graph visualizations were performed for console and game sales, and it was found that action games are the top sellers in all regions except Japan, where RPGs are more popular. We also compared user ratings with reviewer ratings, and found that sales were most correlated with reviewer ratings.

* For the first hypothesis, not being able to reject the null hypothesis, we can conclude that there is not enough statistical evidence to claim that the average user ratings for the Xbox One and PC platforms are different.

* As for the second hypothesis, by rejecting the null hypothesis, we can conclude that there is sufficient statistical evidence to claim that the average user ratings for the Action and Sports genres are different. It is important to note that this does not necessarily imply that one genre is better or worse than the other, but simply that there is a significant difference in the average user ratings for both genres.
