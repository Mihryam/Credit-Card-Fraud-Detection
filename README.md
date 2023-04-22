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


# Simple Auto Encoder
In this algorithm 20,000 normal transaction data was used in training with 400 fraudulent data transaction. I had to choos this because I wanted to teach the auto encoder what normal data looks like. If i take more abnormal data than the normal data, the auto encoder will learn that the fraudulent data is normal and wouldn't give us the results that we want.
29 Columns were encoded into 12 features using the encoder. Finally the decoder expanded the 12 features back to our original features being 29.
An accuracy score of 66% was gotten, with roc score of 80% using batch size of 32 and 20 epochs

# Deep Auto Encoder
Model was trained on normal transactions because I wanted it to detect any abnormality on new transactions presented to it. The Fraudulent Class was included in the test data. Training was done with 100 epochs and a batch size of 32 samples. 20% tst size was used with 18 fraud cases and 3170 normal cases. The model had an acuracy of 98.1% correctly classifying 17 out of the 18 fraud cases and 3113 out of 3170 normal cases.

# Logistic Regression (Vanilla)
The term "vanilla" generally refers to a basic or standard approach without any additional features or modifications. In the context of machine learning, vanilla logistic regression is a straightforward algorithm that can be used for binary classification problems. Although there are other approaches such as smote , etc, i will be working with only this approach.
Using 35% of the data as test size with 168 fraud cases in it, the model correctly classified 129 of them and incorrectly classified 39 of them. It gave us a 99% accuracy score.

# Conclusion
In summary, our models did well in classifying the frauduletn transactions correctly, but the logistic regression model had the highest accuracy of 99%. But I would highly recommend the use of the results from the deep auto encoders as it will perform better in real time detection than the Logistic regression model. There are other algorithms out there to be used for th detection of frauds, plase do well to check them out
