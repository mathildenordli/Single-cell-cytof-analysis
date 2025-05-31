# Master thesis
This repository contains code used for Mathilde Pytte Nordli’s master thesis. Since the data involves sensitive health information, some files, such as those used for preprocessing the train, validation and test datasets are not included. 

The patient IDs used in the dataset are not real, but randomly generated. This was done to prevent the same patient from appearing in multiple splits. For example, if a patient's data before treatment was included in the training set, their post-treatment data was not included in the validation or test sets. This was to avoid the model learning to recognize individuals instead of general patterns.

## Preprocessing folder

This folder includes the preprocessing steps used to prepare the data. It includes:
* Conversion from fcs to csv files using fcsparser

## Decision trees folder

This folder contains all the code related to the decision tree models used in the thesis. It includes:
* The initial run of a decision tree using default settings
* Binary decision trees for classification between two groups at a time
* The process of selecting and evaluating the final, simplified decision tree

## DeepSet folder

This folder contains all the code related to the Deep Sets models used in the thesis. It includes:
* The initial run of Deep Sets models
* Simpler Deep Sets models with fewer parameters

## Clustering folder
Includes:
* K-means clustering followed by classification using decision trees or Lasso logistic regression

