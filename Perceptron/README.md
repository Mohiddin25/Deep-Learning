# Perceptron From Scratch using Iris Dataset

This project demonstrates the implementation of a Perceptron from scratch using the Iris dataset.  
The main goal of this project is to understand the intuition behind how a perceptron learns and updates its decision boundary during training.

---

# What is a Perceptron?

A Perceptron is one of the earliest and simplest neural network models used for binary classification problems.

It learns by:
- taking inputs,
- applying weights,
- calculating an output,
- and updating weights whenever a wrong prediction occurs.

The perceptron tries to separate data using a straight line (or hyperplane in higher dimensions).

---

# Mathematical Intuition

The perceptron learns from mistakes.

Whenever the prediction is incorrect, the weights are adjusted using the update rule:

w = w + α(y - y_pred)x

Where:
- w → weights
- α → learning rate
- y → actual output
- y_pred → predicted output
- x → input features

## Intuition Behind the Equation

- If prediction is correct:
  - no update happens.
- If prediction is wrong:
  - weights are adjusted toward the correct direction.

The learning rate controls how large the update step should be.

This process gradually shifts the decision boundary toward better classification.

---

# Dataset Used

Iris Dataset (Binary Classification)

Classes used:
- Setosa
- Versicolor

Features used:
- Sepal Length
- Petal Length

The dataset is almost linearly separable, making it suitable for understanding perceptron learning.

---

# Steps Involved in the Code

## 1. Import Required Libraries
Libraries such as:
- NumPy
- Matplotlib
- scikit-learn

are used for computation and visualization.

---

## 2. Load the Iris Dataset
The Iris dataset is loaded using scikit-learn.

Only two classes are selected for binary classification.

---

## 3. Select Features
Two features are selected to visualize the decision boundary in 2D space.

---

## 4. Initialize Weights
Weights are initialized randomly.

These weights define the initial decision boundary.

---

## 5. Define Activation Function
The activation function predicts:
- +1 for one class
- -1 for another class

based on the weighted sum.

---

## 6. Train the Perceptron
For every training example:
- predict output,
- compare with actual label,
- update weights if prediction is incorrect.

This is called the Perceptron Learning Rule.

---

## 7. Visualize Decision Boundary
The decision boundary is plotted to observe how the perceptron separates the data.

---

# Key Learning Outcomes

Through this project, we understand:
- how perceptrons learn,
- the importance of weight updates,
- decision boundary movement,
- the role of learning rate,
- and the intuition behind binary classification.

---

# Disadvantages of Perceptron

## 1. Works Only for Linearly Separable Data
Perceptrons fail when data cannot be separated using a straight line.

Example:
- XOR problem

---

## 2. Limited Learning Capability
A single perceptron cannot learn complex patterns.

---

## 3. No Probability Output
Perceptrons provide only hard classifications.

---

## 4. Sensitive to Learning Rate
Very high learning rates may lead to unstable learning.

---

# Conclusion

The perceptron is one of the foundational concepts of deep learning and neural networks.

Although simple, it provides strong intuition about:
- learning from mistakes,
- weight updates,
- and decision boundary optimization.

Understanding perceptrons builds the foundation for advanced neural networks and deep learning architectures.
