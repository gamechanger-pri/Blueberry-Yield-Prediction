# Blueberry Yield Prediction

## About Project

This project employs a Machine Learning model to predict the yield of Blueberries given the temperature condition, pollinator density in that area, and some features of its clone.


## Dataset

[Prediction of Wild Blueberry Yield](https://www.kaggle.com/competitions/playground-series-s3e14/data "Prediction of Wild Blueberry Yield")

## Algorithm/Technology

* Numpy
* Pandas
* Seaborn
* XGBoost
* LightGBM
* CatGBM
* RandomizedSearchCV
* Optuna

## Model

* This model aims to improve prediction accuracy through practical **feature engineering and feature selection** techniques. The primary approach involves building an **ensemble model** that combines the predictions of three base models: 

	1\. LightGBM Regressor</br>
	2\. XGBoost Regressor</br>
	3\. CatBoost Regressor

* The ensemble model is designed to leverage the strengths of each base model, resulting in more accurate and robust predictions. To achieve this, specific base classifiers are **fine-tuned using RandomSearchCV**, a powerful optimization technique.

* Additionally, the project utilizes **optuna** to assign appropriate weights to the trained models within the ensemble. This further enhances the overall performance and ensures that each base model contributes optimally to the final predictions.

## Results

* The ensemble model achieved a five-fold **cross-validation MAE of 342.02**.

## References

* https://www.kaggle.com/code/jamjomjim/randomforest-comments-appreciated/notebook
* https://www.kaggle.com/code/tetsutani/ps3e14-eda-various-models-ensemble-baseline/notebook
* https://www.geeksforgeeks.org/xgboost-for-regression/
* https://www.kaggle.com/code/akioonodera/ps-3-14-lgbm-reg#2.-Import-data
* https://www.kaggle.com/code/mnokno/wild-blueberry-yield-prediction-eda/notebook

