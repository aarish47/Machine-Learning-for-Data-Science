# **The types of Boosting**

## **Written by:** Aarish Asif Khan

## **Date:** 18 February 2024

# **Boosting and the Types of Boosting**

Boosting is a powerful ensemble machine learning technique that combines the predictions of multiple weak models to create a strong model. 

The main idea behind boosting is to train models in a sequential manner, where each new model is trained to correct the mistakes made by the previous models. In this markdown file, we will explore the concept of boosting and the different types of boosting algorithms.

# **Boosting Algorithm**

1. The basic boosting algorithm can be summarized in the following steps:

2. Initialize the weights of the training samples to be equal.

3. For each iteration (or boosting round), train a weak model on the training data, with the weights of the misclassified samples being increased.

4. Calculate the weighted error of the weak model.

5. Calculate the weight of the weak model based on its weighted error.

6. Update the weights of the training samples based on the weak model's predictions.

7. Repeat steps 2-5 for a fixed number of iterations.

8. Combine the predictions of the weak models to make the final prediction.

# **Types of Boosting**

There are several types of boosting algorithms, including:

# **AdaBoost (Adaptive Boosting):**

AdaBoost is one of the most popular boosting algorithms. It assigns higher weights to the misclassified samples and lower weights to the correctly classified samples. The weights of the weak models are also adjusted based on their performance.

# **Example**

```python
from sklearn.ensemble import AdaBoostClassifier
from sklearn.datasets import load_iris
from sklearn.model_selection import train_test_split

iris = load_iris()
X = iris.data
y = iris.target

X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)

ada = AdaBoostClassifier(n_estimators=100, learning_rate=1, algorithm="SAMME")
ada.fit(X_train, y_train)

print("Accuracy:", ada.score(X_test, y_test))
```

# **Gradient Boosting:**

Gradient Boosting is another popular boosting algorithm that minimizes the loss function using gradient descent. It can be used for both regression and classification tasks.

# **Example**

```python
from sklearn.ensemble import GradientBoostingClassifier
from sklearn.datasets import load_iris
from sklearn.model_selection import train_test_split

iris = load_iris()
X = iris.data
y = iris.target

X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)

gb = GradientBoostingClassifier(n_estimators=100, learning_rate=0.1, max_depth=1, random_state=42)
gb.fit(X_train, y_train)

print("Accuracy:", gb.score(X_test, y_test))
```

# **XG Boost:**

XGBoost is a highly optimized implementation of gradient boosting that is widely used in Kaggle competitions. It has several advanced features, such as regularization, parallel processing, and tree pruning.

# **Example**

```python
import xgboost as xgb
from sklearn.datasets import load_iris
from sklearn.model_selection import train_test_split

iris = load_iris()
X = iris.data
y = iris.target

X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)

xgb = xgb.XGBClassifier(n_estimators=100, learning_rate=0.1, max_depth=1, random_state=42)
xgb.fit(X_train, y_train)

print("Accuracy:", xgb.score(X_test, y_test))
```