# Long-Term Fog Prediction (Hyperparameter tunning) 
This repository contains hyperparameter tunning for long term fog index prediction 

## Data
Data Source: https://mesonet.agron.iastate.edu/request/download.phtml

Parameters: Select Network - India ASOS

Select Station

Fix Start and End date

Get Data

## Initial Preprocessing
Data is taken for Lucknow city and others , applied initial preprocessing includes - Normalisation, Resampling, Interpolation , stationarity and seasonality by the team members and cleaned data provided us to do further hyperparameter tunning 

## Preprocessing 
Fog index, Duration and Energy loss column added , also data is resampled of 6 hour for long term fog prediction.

## Models
Machine learning regression models applied but only handful of them - Linear Regression, Gradient boosting, Adaboost, Random forest Regression and Ensemble technique performs well so these models are get considered as a base model.

During EDA one hidden point came in front that - ** Fog Index Value Depends on its previous values **. 

So, two Models proposed till now- 
1) Model -1 : Having columns of previous fog index dataset .
2) Model -2 : Having column of previous day data for which we are predicting .

## Conclusion 
Till now Model -1 performs well ,so it can be included with the base model and further hyperparameter tunning will be performed on the Machine learning models. And Model -2 need to be tested.
