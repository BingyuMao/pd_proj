# Predicting Parkinson’s Disease for Patients Using Voice Recording 

## Introduction

This is the code repository for PH 1976 (Fundamentals of Data Analytics and Predictions) course project in Spring 2022.

## Abstract

In this project, we aim to find an accurate machine-learning model that can predict Parkinson's disease (PD) using the extracted features from the voice recordings of patients. We did data management in three steps before modeling. Firstly, all explanatory variables except categorical ones are scaled to the range 0 to 1 to avoid any measurement error due to unequal scales. Then we performed data upsampling by Synthetic Minority Oversampling Technique (SMOTE) since the binary outcomes are unbalanced. After this step, the sample size is extended from 252 to 408 and the labels become balanced. Next, in order to evaluate the model performance, we split the dataset into 70% training and 30% validation sets. For the modeling part, we conducted five machine learning algorithms including Logistic Regression (LR), k-Nearest Neighbors (k-NN), Random Forest (RF), Support Vector Machine (SVM), and Light Gradient Boosting Machine (LGBM) together with three deep learning methods including Neural Network (NN), Gated Recurrent Unit (GRU), and Long-short Term Memory (LSTM) on the training sets using cross-validation. Then, we calculated the accuracy, sensitivity, and specificity of the validation set. We noticed that the number of variables is larger than the sample size, so we also performed Principal Component Analysis (PCA) for dimension reduction and tested it on the same models. Among all the models tested, we find that LSTM gives the highest accuracy (0.9339) on the validation set.
