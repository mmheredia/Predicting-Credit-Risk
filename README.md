# Predicting-Credit-Risk

This project consisted of creating supervised machine learning models to predict whether a loan from LendingClub will become high risk or not.

## Background

[LendingClub](https://www.lendingclub.com/) is a peer-to-peer lending services company that allows individual investors to partially fund personal loans as well as buy and sell notes backing the loans on a secondary market. LendingClub offers their previous data through an API.

Data from 2019 & 2020 is used in this project to create machine learning models (Logistic Regression and Random Forest Classifier) to predict the credit risk of loans from the first quarter of 2020.

## Description

The Resources folder contains two CSV files of data that was used to train and test the models and a Generator folder which contains the notebook that was used to download data from LendingClub and output the two CSVs.

The two CSVs were undersampled to give an even number of high and lowrisk loans. In the original dataset, only 2.2% of loans are categorized as high risk. To get a truly accurate model, special techniques need to be used on imbalanced data. Undersampling is one of those techniques. Oversampling and SMOTE (Synthetic Minority Over-sampling Technique) are other techniques that are also used.

Preprocessing took place before creating and comparing models that consisted of coverting categorical data to numerical data and filling in nmissing data. A second step included during preprocessing included scaling the data.

## Overall Considerations

Once preprocessing took place, the models were trained and tested within the Credit Risk Evaluator notebook and the Logistics Regression Model proved to outperform the Random Forest Classifier model.