# **Manhattan Distance**

## **Written by:** Aarish Asif Khan

## **Date:** 16 February 2024

# **Manhattan Distance**

Manhattan distance, also known as taxicab distance or city block distance, is a measure of the distance between two points in a grid-based system. It is named after the grid layout of the streets in Manhattan, where traveling from one point to another involves moving along the grid lines.

## **Formula**

The Manhattan distance between two points \( \mathbf{p} \) and \( \mathbf{q} \) in an \( n \)-dimensional space is given by the formula:

\[
\text{Manhattan distance}(\mathbf{p}, \mathbf{q}) = \sum_{i=1}^{n} |q_i - p_i|
\]

Where:
- \( \mathbf{p} = (p_1, p_2, ..., p_n) \) and \( \mathbf{q} = (q_1, q_2, ..., q_n) \) are the coordinates of the two points in the \( n \)-dimensional space.
- \( n \) is the number of dimensions.

## **Properties**

- **Non-Negativity**: The Manhattan distance between two points is always non-negative.
- **Identity of Indiscernibles**: The distance between two identical points is zero.
- **Symmetry**: The distance from point \( \mathbf{p} \) to point \( \mathbf{q} \) is the same as the distance from point \( \mathbf{q} \) to point \( \mathbf{p} \).
- **Triangle Inequality**: The sum of the lengths of any two sides of a triangle is greater than the length of the remaining side. In other words, the shortest path between two points is along the grid lines.

## **Applications**

- **Robotics**: Manhattan distance is commonly used in robotics for path planning and navigation tasks, where the movement is restricted to grid-based environments.
- **Computer Vision**: It is used for object tracking and image registration, especially when dealing with pixel-based distances.
- **Game Development**: Manhattan distance is useful in game development for implementing AI behaviors, collision detection, and pathfinding algorithms in grid-based game worlds.

## **Conclusion**

Manhattan distance provides a simple and intuitive way to measure distances between points in a grid-based system. Its properties and applications make it a valuable tool in various fields, particularly in scenarios where movement is constrained along grid lines.


