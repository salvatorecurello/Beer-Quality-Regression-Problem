# Beer-Quality-Regression-Problem
Extracting information from each beer reviews in order to predict the quality score of a specific beer.

## Overview

This project involves building a regression model to predict beer quality scores based on a dataset of beer reviews. The goal is to accurately predict beer quality ratings on a scale of 1 to 5 for a test set of 30,000 reviews, after training models on a dataset of 70,000 reviews.

The dataset contains 13 features including numerical features like alcohol content, and categorical features like beer style, review text, etc. The target variable is the "review/overall" score.

## Approach

The main steps taken in this project:

- Data exploration and visualization to understand distributions and correlations
- Preprocessing of different data types
  - normalization for numerical
  - one-hot encoding for categorical
  - TF-IDF vectorization for text
- Testing different regression algorithms
  - Ridge
  - Lasso
  - Random Forest
  - LightGBM
- Hyperparameter tuning using grid search and 5-fold cross-validation
- Evaluation using $R^2$ metric

## Results

- Ridge regression achieved the best performance with $R^2$ score of 0.716 on public test set
- LightGBM and Random Forest also performed reasonably well
- The feature engineering and preprocessing were important to get good results

## Future Work

Some ideas to further improve performance:

- Try other feature extraction methods like Word2Vec for text
- Additional hyperparameter tuning
- Experiment with neural network models like MLPRegressor


