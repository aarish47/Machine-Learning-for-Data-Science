# **Logistic Regression**

## **Written by:** Aarish Asif Khan

## **Date:** 17 February 2024

# **Logistic Regression**

Logistic regression is a statistical method used for binary classification, which means predicting the probability of an observation belonging to one of two classes. Despite its name, logistic regression is a classification algorithm rather than a regression algorithm.

## **How it Works**

In logistic regression, we model the probability that an observation belongs to a particular class. The output of logistic regression is a logistic function (also called the sigmoid function) that maps any real-valued number to a value between 0 and 1. This function is represented by the equation:

\[ P(Y=1|X) = \frac{1}{1 + e^{-z}} \]

**where:**

- \( P(Y=1|X) \) is the probability of the observation belonging to class 1,
- \( X \) represents the input features,
- \( z \) is the linear combination of the input features and their associated weights.

The logistic function transforms the output of a linear equation into a probability, making it suitable for classification tasks.

## **Types of Logistic Regression**

- **Binary Logistic Regression**: Used for binary classification problems with two classes.

- **Multinomial Logistic Regression**: Used when there are more than two classes but each observation belongs to only one class.

- **Ordinal Logistic Regression**: Used when the classes have a natural order or ranking.

## **Applications**

Logistic regression is widely used in various fields for classification tasks, including:

- Predicting whether an email is spam or not.

- Identifying whether a customer will purchase a product based on demographic and behavioral data.

- Medical diagnosis, such as predicting whether a patient has a particular disease based on symptoms and test results.

## **Evaluation**

The performance of a logistic regression model can be evaluated using metrics such as:

- **Accuracy**: Measures the proportion of correctly classified observations.

- **Precision and Recall**: Evaluate the trade-off between false positives and false negatives.

- **Receiver Operating Characteristic (ROC) Curve and Area Under the Curve (AUC)**: Measures the ability of the model to discriminate between classes.

## **Conclusion**

Logistic regression is a powerful and interpretable method for binary classification tasks. Despite its simplicity, it's often used as a baseline model and can perform well in many real-world scenarios.
