# Long-Term Fog Prediction (Hyperparameter tunning) 
This repository contains hyperparameter tunning for long term fog index prediction 

## Data
Data Source: https://mesonet.agron.iastate.edu/request/download.phtml

Parameters: Select Network - India ASOS

Select Station

Fix Start and End date

Get Data

## Initial Preprocessing
Data is taken for Lucknow and other cities after it initial preprocessing applied which includes - Normalisation, Resampling, Interpolation , stationarity and seasonality by the team members and cleaned data provided us for further hyperparameter tunning 

## Preprocessing 
Fog index,Fog Duration and Energy loss column get added and resampling occurs for 6 hr .

## Models
Many Machine learning regression models applied on the dataset but only handful of them - **Linear Regression, Gradient boosting, Adaboost, Random forest Regression and Ensemble technique** performs well so they are considered for base model.

During EDA one hidden point came in front that - **Fog Index Value Depends on its previous values**. 

By, considering this above point two Models were proposed - 
1) Model -1 : Having columns of previous fog index datasets .
2) Model -2 : Having column of previous day data for which we are predicting .

## Conclusion 
Till now Model -1 performs well ,so it can be included with the base model and further hyperparameter tunning will be performed on the Machine learning models. Also Model -2 need to be tested further.
