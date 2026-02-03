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
