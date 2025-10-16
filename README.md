# 🌸 Iris Flower Prediction Web App

A machine learning project that predicts the species of an Iris flower using K-Nearest Neighbors (KNN), deployed as a Flask web application.

## 🔹 About Iris Flowers

The Iris flower is a popular flower used in machine learning datasets because it has clear differences between species while being easy to measure.

Species in the dataset:

Iris-setosa – Small flowers with short petals, usually bright white or violet.

Iris-versicolor – Medium-sized flowers with colorful petals, often blue or purple.

Iris-virginica – Large flowers with long petals, typically violet-blue.

## Features measured in the dataset:

Sepal Length (cm)

Sepal Width (cm)

Petal Length (cm)

Petal Width (cm)

These measurements allow a machine learning model to distinguish between the three species accurately.

# 🔹 Machine Learning Concepts
## 1. Supervised Learning

This project uses supervised learning, where:

The algorithm learns from labeled data (features + target labels).

Features: Sepal length, Sepal width, Petal length, Petal width

Target: Species (Iris-setosa, Iris-versicolor, Iris-virginica)

The model learns patterns in the data and predicts the species for new, unseen flowers.

## 2. K-Nearest Neighbors (KNN) Algorithm

KNN is a simple but powerful algorithm for classification:

## How it works:

For a new flower, KNN finds the K nearest neighbors in the training dataset.

It calculates the distance (Euclidean or other metrics) between the new flower and all training points.

Predicts the species based on the majority class among the K neighbors.

## Key points:

Non-parametric: KNN does not assume any data distribution.

Lazy learning: KNN stores training data and computes predictions at runtime.

Hyperparameters: K (number of neighbors) and distance metric can be tuned for best performance.

## Advantages:

Simple and intuitive.

Works well on small datasets with clear patterns.

## Limitations:

Can be slow for large datasets.

Sensitive to irrelevant features and feature scaling.

## 3. Model Training

Trained on the classic Iris dataset (150 samples, 4 features).

Used GridSearchCV to optimize hyperparameters (n_neighbors, weights, algorithm).

Model saved using pickle (predictor.pickle) for deployment in Flask.

# 🔹 Web Application

Built using Flask (Python).

Users can input:

Sepal Length (cm)

Sepal Width (cm)

Petal Length (cm)

Petal Width (cm)

Model predicts and displays the species of the Iris flower instantly.

# 🔹 Example Inputs and Outputs
| Sepal Length | Sepal Width | Petal Length | Petal Width | Predicted Species |
| ------------ | ----------- | ------------ | ----------- | ----------------- |
| 5.1          | 3.5         | 1.4          | 0.2         | Iris-setosa       |
| 6.0          | 2.9         | 4.5          | 1.5         | Iris-versicolor   |
| 6.3          | 3.3         | 6.0          | 2.5         | Iris-virginica    |

# 🔹 Technologies Used

Python

scikit-learn (machine learning)

NumPy & Pandas (data handling)

Flask (web deployment)

HTML/CSS (frontend) 



# 🔹 Why an Iris Flower Prediction Model is Important

## Educational Purpose

-The Iris dataset is a classic dataset in machine learning.
-It helps beginners learn supervised learning, classification algorithms, and model deployment.

## Understanding Machine Learning Concepts

-It demonstrates feature-based classification.
-Shows how algorithms like KNN use patterns in data to make predictions.

## Foundation for Real-world Applications

-Predicting species based on measurements is a real-world classification problem.
-Similar methods are used in:
    -Agriculture (identifying plant or crop species)
    -Biology research (species classification)
    -Environmental monitoring (tracking plant diversity)

# 🔹 How This Model Can Be Used

## Botanical Research

Quickly identify the species of an Iris flower from measurements.

Useful for researchers to label flowers accurately without manual inspection.

## Educational Tools

Teachers and students can use it to learn machine learning interactively.

## Agriculture & Gardening

Helps gardeners or horticulturists classify plants and maintain records.

## Machine Learning Practice

Serves as a template for building other classification models for real-world data.

Shows how to train, test, and deploy a model using Flask.
