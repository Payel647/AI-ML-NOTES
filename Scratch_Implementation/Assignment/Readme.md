# KNN Regressor from Scratch (Without scikit-learn)

This assignment demonstrates how to implement a **K-Nearest Neighbours (KNN) Regressor from scratch** using Python, **without using scikit-learn**.

The goal is to understand the internal working of KNN regression by manually computing distances, finding nearest neighbors, and predicting continuous target values.

---

## Problem Statement

Given a dataset of input features and continuous target values, implement a **KNN Regressor** that:

1. Computes distances between data points
2. Finds the **k nearest neighbours** using **Euclidean distance**
3. Predicts the output as the **average of the neighbours’ target values**

---

##  Dataset

### Training Data

```python
X_train = [[1], [2], [3], [4], [5]]
y_train = [2, 4, 6, 8, 10]
```

### Testing Data

```python
X_test = [[1.5], [3.5], [6]]
```

---

## Algorithm Used

### K-Nearest Neighbours (KNN) Regression

* Distance Metric: **Euclidean Distance**
* Prediction Rule:
  [
  \hat{y} = \frac{1}{k} \sum_{i=1}^{k} y_i
  ]
  where ( y_i ) are the target values of the k nearest neighbors.

---

## Steps to Implement

1. Store the training data (`X_train`, `y_train`)
2. Compute **Euclidean distance** between a test point and all training points
3. Sort distances in ascending order
4. Select the **k nearest neighbors**
5. Compute the **mean of their target values**
6. Return the predicted value
