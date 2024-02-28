# **Important Terminologies**

## **Written by:** Aarish Asif Khan

## **Date:** 16 February 2024

# **Entropy, Gini impurity and Information Gain**

Decision trees are a popular machine learning algorithm for classification tasks. In the process of building decision trees, several metrics are used to measure the impurity or randomness of a dataset, as well as the effectiveness of attributes in classifying the data. Three key metrics in this context are entropy, Gini impurity, and information gain.

## Entropy

Entropy is a measure of impurity in a dataset. It quantifies the uncertainty or randomness of the data. The entropy of a dataset \( S \) is calculated using the formula:

\[ \text{Entropy}(S) = - \sum_{i=1}^{c} p_i \log_2(p_i) \]

# **Where:**

- \( c \) is the number of classes
- \( p_i \) is the probability of class \( i \) occurring in the dataset

A lower entropy value indicates a more homogeneous dataset, while a higher entropy value indicates greater uncertainty or randomness.

## **Gini Impurity**

Gini impurity is another metric used to measure impurity in a dataset. It is calculated as follows:

\[ \text{Gini}(S) = 1 - \sum_{i=1}^{c} p_i^2 \]

Similar to entropy, Gini impurity ranges from 0 to 1, where 0 represents perfect purity and 1 represents maximum impurity.

## **Information Gain**

Information gain is used to determine the best attribute for splitting the dataset in decision tree algorithms. It measures the reduction in entropy or Gini impurity achieved by splitting the data on a particular attribute. The formula for information gain is:

\[ \text{Information Gain}(S, A) = \text{Entropy}(S) - \sum_{v \in \text{Values}(A)} \frac{|S_v|}{|S|} \text{Entropy}(S_v) \]

# **Where:**

- \( A \) is the attribute being considered for the split
- \( \text{Values}(A) \) is the set of possible values for attribute \( A \)
- \( |S_v| \) is the number of instances in subset \( S_v \)
- \( |S| \) is the total number of instances in \( S \)

Information gain helps in selecting the attribute that provides the most significant reduction in impurity when creating decision trees.

In summary, entropy, Gini impurity, and information gain are crucial metrics used in decision tree algorithms to measure impurity in datasets and guide the selection of attributes for splitting the data.
