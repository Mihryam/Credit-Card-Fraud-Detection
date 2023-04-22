# Credit-Card-Fraud-Detection

## Table of Contents
* [Introduction](#Introduction)
* [Problem Definition and Algorithm](#Problem Definition and Algorithm)
* [Simple Autoencoder](#Simple Autoencoder)
* [Deep Auto Encoder](#Deep Auto Encoder)
* [Logistic Regression](#Logistic Regression)
* [Conclusion](#Conclusion)

# Introduction

In today's fast-paced and digital world, credit card fraud is a growing concern for both consumers and financial institutions. Every year, millions of dollars are lost due to fraudulent credit card transactions. To combat this issue, machine learning algorithms can be utilized to identify and prevent fraudulent transactions. In this project, I will explore various machine learning algorithms that can be employed for credit card fraud detection. Through this project, I aim to create a robust and accurate model that can detect fraudulent transactions in real-time, and compare the differnt results from the model.

# Problem Definition and Algorithm
Credit card fraud detection is a fascinating problem due to its constantly evolving nature and high stakes. Innovative solutions using machine learning algorithms are needed to stay ahead of fraudsters and protect consumers and businesses in real-time. In this project , the data used was posed with high imbalance as the Normal transactions were more than the Fraudulent Transactions. I had to strategize a way to make the models learn what Normal transactions looked like and correctly classify the fraudulent transactions.
##
The data had 31 columns and 284807 rows, with just 492 of them being fraudulent and the rest Normal Transactions.
The algorithms used were Logistic Regresssion, K- Means, and Auto Encoders. I will be comparing different results of the models. A brief explanation of algorithms used can be seen below:

* Logistic Regression: Logistic Regression is a classification technique used in machine learning. It uses a logistic function to model the dependent variable. The dependent variable is dichotomous in nature, i.e. there could only be two possible classes (eg.: either the transaction is fraudulent or Normal.

* K-Means: K-means is an unsupervised classification algorithm, also called clusterization, that groups objects into k groups based on their characteristics. The grouping is done minimizing the sum of the distances between each object and the group or cluster centroid.

* Autoencoders: An autoencoder is a neural network model that can be used to learn a compressed representation of raw data. It takes as input large data size and reconstructs it.
