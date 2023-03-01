# NCAAB Data Analysis Project

Sports analytics is an emerging data science field that is gaining public exposure. Leagues like the National Football League (NFL) are routinely including [NextGen Stats](https://nextgenstats.nfl.com/) during their broadcasts, which include advanced statistics like expected completion percentage. The National Collegiate Athletic Association Basketball (NCAAB) has a plethora of data that can also be analyzed using similar analytical techniques to make both conclusions about previous seasons and predictions about future seasons. 

In these notebooks, I will use the 2021 season from an NCAAB [dataset](https://www.kaggle.com/datasets/andrewsundberg/college-basketball-dataset) to build build multiple models:

1) A linear regression model using several team statistical measures that I believe will capture a team's winning percentage (wins / total games) during the season. I will extend this model to previous seasons to see how well it can generalize across years. 
2) A decision tree classifier that will use the same team statistics as above to predict whether or not a team made the NCAA March Madness tournament in 2021. 

## Contents
1) Loading data and libraries
2) Exploratory Data Analysis and Pre-processing
3) Model Training
4) Model Testing
5) Model predictions for other seasons
6) Final Summary

## Summary of Findings and Future Directions
Linear regression:
Overall, the six predictors I selected (Adjusted Offensive Efficiency, Adjusted Defensive Efficiency, Effective Field Goal Percentage Shot, Effective Field Goal Percentage Allowed, Two-Point Shooting Percentage, and Two-Point Shooting Percentage Allowed) did a relatively good job of predicting a team's winning percentage from both the 2021 and 2020 seasons. 

There is certainly more optimization I can do to account for multicollinearity and improve the predictive value of the model. I would like to continue to work with this data set and test other machine learning techniques, which I will add to this repo as I perform them. 

Decision Tree:
The decision tree did a fairly good job of predicting which teams would make the 68-team March Madness tournament, both within the 2021 test data, and across the untrained 2019 season data. 

There is some concern here for the imbalance of outcomes (only 68 teams make the tournament and 200+ do not), so this may not be the most sensitive model to make such a classification. Again, I will pursue other models, and perhaps methods for dealing with such an imbalance of outcomes.
