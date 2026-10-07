# Bank Customer Churn Prediction using ANN

## Project Overview

This project focuses on predicting whether a bank customer is likely to leave the bank using an Artificial Neural Network (ANN).

The project demonstrates an end-to-end deep learning workflow, including data preprocessing, categorical encoding, feature scaling, train-test splitting, neural network development, model training, and binary classification.

---

## Problem Statement

Customer churn is an important problem for banks because losing existing customers can negatively affect business revenue.

The objective of this project is to build a machine learning/deep learning model that can predict whether a customer is likely to leave the bank based on customer-related features.

The target variable is:

- `Exited = 0` → Customer stayed with the bank
- `Exited = 1` → Customer left the bank

---

## Dataset

The project uses a bank customer churn dataset containing customer demographic, financial, and account-related information.

### Important Features

- CreditScore
- Geography
- Gender
- Age
- Tenure
- Balance
- NumOfProducts
- HasCrCard
- IsActiveMember
- EstimatedSalary

### Target Variable

- `Exited`

The target is a binary classification variable representing customer churn.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- TensorFlow
- Keras
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Machine Learning Workflow

The project follows these major steps:

1. Import required libraries
2. Load the dataset
3. Inspect the dataset
4. Check data types and missing values
5. Check duplicate records
6. Perform data preprocessing
7. Encode categorical variables
8. Apply one-hot encoding
9. Select relevant features
10. Split data into training and testing sets
11. Apply feature scaling using `StandardScaler`
12. Build an Artificial Neural Network
13. Compile the neural network
14. Train the model
15. Generate predictions
16. Evaluate the model

---

## Data Preprocessing

### Categorical Encoding

Categorical features such as `Gender` and `Geography` are converted into numerical representations so that they can be used by the neural network.

One-hot encoding is applied to categorical variables where required.

### Feature Scaling

`StandardScaler` from Scikit-learn is used to scale numerical features.

Feature scaling helps the neural network train more effectively by bringing numerical features to a comparable scale.

---

## Artificial Neural Network

The project uses an Artificial Neural Network implemented using TensorFlow and Keras.

The network consists of:

- Input layer
- Hidden layers
- Output layer

### Activation Functions

The hidden layers use the **ReLU (Rectified Linear Unit)** activation function.

The output layer uses the **Sigmoid** activation function because the project performs binary classification.

Conceptually:

```text
Input Features
      ↓
Input Layer
      ↓
Hidden Layer
(ReLU)
      ↓
Hidden Layer
(ReLU)
      ↓
Output Layer
(Sigmoid)
      ↓
Churn Prediction
0 = Stayed
1 = Exited
