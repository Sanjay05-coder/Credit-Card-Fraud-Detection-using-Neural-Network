Credit Card Fraud Detection (Binary Classification)
Project Overview

This project implements a binary classification model to detect whether a credit card transaction is fraudulent or non-fraudulent using a Neural Network.
The dataset consists of numerical features that were scaled and fed into a neural network trained using Binary Cross Entropy loss.

 Dataset

Features: V1 to V28 (PCA-transformed features)

Amount: Transaction amount

Class:

0 → Not Fraud

1 → Fraud

Data Preprocessing

Removed irrelevant columns (if any)

Handled missing values

Applied Min-Max Scaling to normalize all feature values between 0 and 1

Split data into training and testing datasets

 Model Architecture

Input Layer: Scaled feature vector

Hidden Layer:

1 hidden layer

Activation function: ReLU

Output Layer:

1 neuron

Activation function: Sigmoid (binary classification)

 Model Training

Loss Function: Binary Cross Entropy

Optimizer: Adam

Epochs: 30

The model learns to classify transactions by minimizing prediction error during training.

 Model Evaluation

Evaluated using a confusion matrix

Observed metrics:

True Positives

True Negatives

False Positives

False Negatives

 Model Accuracy

Achieved Accuracy: 0.9991 (99.91%)

This high accuracy indicates the model’s strong ability to distinguish between fraudulent and non-fraudulent transactions.

 Prediction on New Data

A new sample transaction dataset was created

The data was scaled using the same Min-Max Scaler

The trained model predicted the class:

1 → Fraud

0 → Not Fraud

This confirms whether a new transaction is suspicious.

 Results

Successfully predicts fraud and non-fraud transactions

Achieved 99.91% accuracy

Demonstrates the effectiveness of neural networks in fraud detection tasks
