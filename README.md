# housing-price-decision-analysis

## Problem Background
This project aims to predict housing prices in California and analyze
which factors most influence housing value, with the goal of supporting
pricing and investment decisions.

## Dataset
We use the California Housing dataset provided by scikit-learn, which
contains demographic and geographic features such as income, population,
and location.

## Feature Engineering
- SpacePerCapita: Average rooms divided by average occupancy
- Distance to San Francisco and Los Angeles

These features are designed to better capture living quality and
geographic influence on housing prices.

## Exploratory Data Analysis
We analyze feature distributions and correlations to understand
relationships between variables and housing prices.

## Modeling
A Random Forest Regressor is used to capture non-linear relationships
between features and housing prices.
Model performance is evaluated using RMSE and R².

## Results
The model achieves reasonable generalization performance on the test set.
Feature importance analysis shows that income level and geographic
location are key drivers of housing prices.

## Limitations
- Housing prices are capped in the dataset
- The model does not account for temporal market changes

## Practical Implications
This model can help real estate agents or investors prioritize key
factors when evaluating housing prices, rather than relying on intuition
alone.

## Feature Importance and Interpretation

Feature importance analysis from the Random Forest model shows that
median income (MedInc) is the most influential factor in housing price
prediction, accounting for more than 50% of the total importance.
This suggests that socioeconomic conditions dominate housing value
determination.

Average occupancy (AveOccup) is the second most important feature,
indicating that residential density plays a significant role in price
variation. Areas with higher occupancy levels tend to be associated
with lower housing prices.

Geographic features, including distance to San Francisco and Los Angeles
as well as latitude and longitude, collectively contribute a substantial
portion of the model's predictive power. This highlights the strong
impact of proximity to major economic centers on housing prices.

Structural attributes such as house age and room-related features show
relatively lower importance, suggesting that while they affect prices,
their influence is secondary compared to location and income factors.

It is important to note that feature importance reflects predictive
relevance rather than causal relationships.

## Limitations

This project has several limitations that should be considered when
interpreting the results.

First, the target variable in the California Housing dataset is capped
at an upper bound, which limits the model’s ability to accurately
predict high-end housing prices. As a result, predictions for expensive
properties may be systematically underestimated.

Second, the dataset represents a snapshot of housing conditions at a
specific time period. Temporal factors such as market cycles, interest
rates, and economic shocks are not included, which reduces the model’s
applicability to real-time or future price forecasting.

Third, feature importance in tree-based models reflects predictive
contribution rather than causal relationships. While income and
geographic factors appear highly influential, this does not imply that
changing these factors would directly cause housing prices to increase
or decrease.

Finally, some features may be correlated with each other, meaning that
their individual importance values should be interpreted cautiously.
Certain variables may appear less important because their information
is partially captured by other features.

Despite these limitations, the model remains useful as a decision
support tool for identifying key drivers of housing prices rather than
as a precise valuation system.
