## Introduction
This code trains and evaluates several machine learning models on labeled and unlabeled data. The labeled data consists of 8000 samples and the remaining samples are unlabeled.

## Data Preprocessing
The data is loaded from several numpy files and csv files. The features are preprocessed by filling NaN values with an empty string. The labeled and unlabeled data are separated, and the features and labels are extracted. The features are combined and three different datasets are created:

- Combined dataset
- Embeddings dataset
- TF-IDF dataset

## Model Training and Evaluation
The AutoGluon library is used to predict labels for the unlabeled data, and the confident samples and predictions are stored in dictionaries. Four machine learning models are used:

- KNN
- Logistic Regression
- SVM
- Random Forest

The models are trained and evaluated with and without self-training.

## Performance Metrics
The performance metrics used for evaluation are accuracy, precision, recall, and f1-score. The results are stored in a DataFrame and printed in a table sorted by accuracy in descending order.