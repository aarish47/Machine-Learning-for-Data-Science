# **Minkowski Distance**

## **Written by:** Aarish Asif Khan

## **Date:** 16 February 2024

# **Minkowski Distance**

Minkowski distance is a generalization of both the Euclidean distance and the Manhattan distance. It is a metric used to measure the distance between two points in a multidimensional space. The Minkowski distance formula allows for adjusting the distance calculation based on a parameter \( p \), which determines the order of the distance metric.

## **Formula**

The Minkowski distance between two points \( \mathbf{p} \) and \( \mathbf{q} \) in an \( n \)-dimensional space is given by the formula:

\[
\text{Minkowski distance}(\mathbf{p}, \mathbf{q}, p) = \left( \sum_{i=1}^{n} |q_i - p_i|^p \right)^{\frac{1}{p}}
\]

Where:
- \( \mathbf{p} = (p_1, p_2, ..., p_n) \) and \( \mathbf{q} = (q_1, q_2, ..., q_n) \) are the coordinates of the two points in the \( n \)-dimensional space.
- \( n \) is the number of dimensions.
- \( p \) is a parameter that determines the order of the distance metric. When \( p = 1 \), it reduces to the Manhattan distance, and when \( p = 2 \), it reduces to the Euclidean distance.

## **Properties**

- **Non-Negativity**: The Minkowski distance between two points is always non-negative.
- **Identity of Indiscernibles**: The distance between two identical points is zero.
- **Symmetry**: The distance from point \( \mathbf{p} \) to point \( \mathbf{q} \) is the same as the distance from point \( \mathbf{q} \) to point \( \mathbf{p} \).
- **Triangle Inequality**: The sum of the lengths of any two sides of a triangle is greater than the length of the remaining side.

## **Applications**

- **Machine Learning**: Minkowski distance is used in machine learning algorithms like K-Nearest Neighbors (KNN) for measuring the similarity between data points, offering flexibility in adjusting the distance metric based on the problem domain.
- **Image Processing**: It is employed in image processing tasks such as object recognition and image matching, where different features may have varying importance and require different distance metrics.
- **Geographic Information Systems (GIS)**: Minkowski distance is utilized in GIS applications for spatial analysis, such as calculating distances between geographical points considering different factors like terrain and accessibility.

## **Conclusion**

Minkowski distance provides a flexible framework for measuring distances between points in multidimensional spaces, allowing for customization through the parameter \( p \). Its versatility and adaptability make it a valuable tool in various domains, especially in scenarios where different distance metrics are needed based on the problem requirements.

