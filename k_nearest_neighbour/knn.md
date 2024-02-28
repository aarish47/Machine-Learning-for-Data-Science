# **K-Nearest Neighbours**

## **Written by:** Aarish Asif Khan

## **Date:** 16 February 2024

# **K-Nearest Neighbors (KNN) Algorithm**

K-Nearest Neighbors (KNN) is a simple and versatile supervised machine learning algorithm used for both classification and regression tasks. It is a non-parametric and lazy learning algorithm, meaning it doesn't make assumptions about the underlying data distribution and it doesn't learn a model during training phase, but instead, memorizes the training dataset.

## **How KNN Works**

1. **Data Representation**: KNN works on a dataset with labeled data points, where each data point is a feature vector in a multidimensional feature space.

2. **Distance Calculation**: To make predictions for a new data point, KNN calculates the distance between that point and all other points in the training dataset. Common distance metrics include Euclidean distance, Manhattan distance, or Minkowski distance.

3. **Finding Neighbors**: After calculating distances, KNN identifies the k nearest neighbors to the new data point based on the chosen distance metric.

4. **Majority Voting (Classification) / Mean Calculation (Regression)**: For classification tasks, KNN predicts the class label of the new data point by taking a majority vote among the labels of its k nearest neighbors. For regression tasks, it predicts the target value by calculating the mean of the target values of its k nearest neighbors.

## **Choosing the Value of k**

The choice of k, the number of nearest neighbors to consider, is crucial in KNN. A smaller value of k leads to more flexible decision boundaries, but it might be sensitive to noise. On the other hand, a larger value of k leads to smoother decision boundaries but might not capture local patterns well. Choosing an optimal value of k often involves experimentation and cross-validation.

## **Pros and Cons**

### **Pros:**

- Simple and intuitive algorithm.
- No training phase, making it computationally efficient during prediction.
- Can be effective for datasets with non-linear decision boundaries.

### **Cons:**

- Computationally expensive during prediction, especially for large datasets.
- Sensitive to irrelevant features and noisy data.
- Requires careful selection of the distance metric and value of k.
- Not suitable for high-dimensional data due to the curse of dimensionality.

## **Applications**

KNN has a wide range of applications across various domains, including:
- Recommender Systems
- Image Recognition
- Text Mining
- Healthcare
- Finance

## **Conclusion**

K-Nearest Neighbors is a simple yet powerful algorithm for both classification and regression tasks. While it has its limitations, it remains a popular choice for its simplicity and effectiveness, especially for smaller datasets and when interpretability is important.
