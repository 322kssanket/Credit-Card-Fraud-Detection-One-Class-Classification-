# Credit-Card-Fraud-Detection-One-Class-Classification-
One-Class Classification Project
Overview
This project focuses on the implementation and analysis of three one-class classification algorithms. One-class classification (OCC) is used to classify data points based on a single class observed during training. During inference, the model identifies whether a new point belongs to the known class or is an outlier.

Problem Statement
Credit card companies must identify fraudulent transactions to protect customers from unauthorized purchases. The dataset used for this project contains credit card transactions made by European cardholders over two days in September 2013. Out of 284,807 transactions, only 492 were fraudulent, making the dataset highly imbalanced. The dataset includes 30 features: 28 of which are principal components (V1-V28) from a PCA transformation, while 'Time' and 'Amount' remain unchanged. The response variable, 'Class', indicates whether a transaction is fraudulent (1) or legitimate (0). Due to the imbalance, we use the Area Under the Precision-Recall Curve (AUPRC) as the primary evaluation metric.

Algorithms Implemented
Isolation Forest:
An anomaly detection algorithm that isolates observations by randomly selecting features and splitting the data.
DBSCAN (Density-Based Spatial Clustering of Applications with Noise):
A clustering algorithm that finds dense regions in data space and separates noise points.
One-Class SVM (Support Vector Machines):
This algorithm learns a decision boundary that encompasses the majority of the data from the target class and treats any data point outside the boundary as an anomaly.
Datasets Used Credit Card Fraud Detection from Kaggle (https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud).

Getting Started
Prerequisites
Python 3.x
Required Libraries: scikit-learn, numpy, matplotlib, pandas
