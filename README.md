# Kaggle House Price Competition

This repo is to share some models and techniques I use in the competition such as LGBM regressor and XGB regressor. I start with a simple model and improve it with feature engineering and parameters optimization.

## File Organization

In the project/workspace folder we should have: the models notebooks/python_files (like lgbm1.ipynb) and the 'input' folder (where the dataset should be - just unzip the files there).

## LGBM_1

This model is simple. It uses some data visualization to make sense of the problem, simple feature engineering to handle categorical features and missing values and almost no model optimization. The most cost-efficent thing done here is a log transformation on the target, that makes the model way better.

## LGBM_1 future improvements

The next step is to detect and remove outliers. By the data analysis we can see that they can have a great impact on the results. Other changes could be better feature engineering, creating meaningful features by combination/transformation or using one-hot-encoding.

## Stacking_1

In this model was made stacking lgbm regressor, lasso, linear regressor and xgboost regressor, using as meta-model the linear regressor from sklearn. I made almost no changes from LGBM_1 file and this approach improved a lot the results. The improvements of the section above are still valid.
