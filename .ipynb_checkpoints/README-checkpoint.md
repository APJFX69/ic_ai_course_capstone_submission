# A client sentiment recommendation expert module for CRM

## PROJECT OVERVIEW

WE are building a model that classifies product description provided by clients into classes depending on the positivity of the review. Based on that the model recommends an action (prioritisation for the respective sales person to reach ou to client).

## DATA
The project is using data from two sources - both available via Kaggle platform that are then merged to create a synthetic data used to train model. The details of the each data sources is provided under 

[View the Data Sheet](./data_sheet.md)

## MODEL 

WE are using ensemble model that has few inputs: sentiment model to for pre-processing and than an ensemble of GradientBoost and RnadomForest 

A model card is provided as a part of the project: [View the Model Card](./model_card.md)

## HYPERPARAMETER OPTIMSATION

Given fairly small data set for the training no hyperparameter optimisation was done.

## RESULTS
Here is the resulting classification tree for the Random Forest:
![RF Treet](rf_tree.svg)

Here is the resulting classification tree for the Gradient Boost Forest:
![GB Tree](gb_tree.svg)

The meta model is finished by a logistic regression being used as final estimator result in the following weights

### Meta-model weights (higher -> more influence):
Intercept: 1.026676149653994
rf_proba    0.228467
gb_proba   -0.999474


