# Airline Passenger Satisfaction Prediction

## Project Overview

This project uses machine learning to predict airline passenger satisfaction based on passenger demographics, travel characteristics, and ratings of airline services.

The project focuses on data exploration, preprocessing, classification model development, and model evaluation using ROC-AUC.

## Objectives

- Explore passenger and flight-related data to identify patterns associated with satisfaction.
- Prepare numerical and categorical features for machine learning.
- Train and compare classification models.
- Evaluate model performance using holdout validation and stratified 5-fold cross-validation.
- Generate predictions for the Kaggle competition.

## Models Used

The following classification models were explored:

- **Logistic Regression** — baseline classification model.
- **XGBoost** — gradient-boosting model for tabular data.
- **CatBoost** — gradient-boosting model with support for categorical features.

## Model Evaluation

ROC-AUC (Area Under the Receiver Operating Characteristic Curve) was used as the primary evaluation metric.

| Evaluation | ROC-AUC |
|---|---:|
| CatBoost notebook — Kaggle public leaderboard | **0.95773** |
| 5-fold cross-validation notebook — Kaggle public leaderboard | 0.95635 |
| 5-fold cross-validation mean | 0.95714 |
| 5-fold cross-validation standard deviation | 0.00063 |

The cross-validation mean and standard deviation summarize performance across five validation folds. Kaggle public leaderboard scores are calculated on a separate subset of the competition test data.

## Project Structure

- `airline_satisfaction_catboost.ipynb` — Exploratory data analysis, preprocessing, model experiments, and CatBoost validation.
- `airline_satisfaction_5fold_cv.ipynb` — Model evaluation using stratified 5-fold cross-validation.

## Tools and Technologies

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- XGBoost
- CatBoost
- Jupyter Notebook

## Key Learnings

- Performing exploratory data analysis on a large tabular dataset.
- Preparing features for different classification algorithms.
- Comparing baseline and gradient-boosting models.
- Evaluating model performance using ROC-AUC.
- Using cross-validation to assess model stability.
- Generating probability-based predictions for a Kaggle competition.

## Future Improvements

- Further optimize model hyperparameters.
- Explore model ensembling and probability blending.
- Analyze feature importance and model errors.
- Evaluate additional feature-engineering strategies.

## Author

 Machine Learning and Data Analytics Enthusiast
