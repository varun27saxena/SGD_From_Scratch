<div align="center">

# Stochastic Gradient Descent From Scratch

### Multiple Linear Regression using SGD + Learning Rate Scheduling

<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white"/>
<img src="https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white"/>
<img src="https://img.shields.io/badge/Matplotlib-ffffff?style=for-the-badge&logo=plotly&logoColor=black"/>

<br><br>

<img width="850" src="https://miro.medium.com/v2/resize:fit:1400/1*ty9QYBBO9leUbRtlXmQBiQ.gif">

</div>

---

# Project Overview

This project is a **complete implementation of Stochastic Gradient Descent (SGD) from scratch** for **Multiple Linear Regression** using only **NumPy**.

Instead of relying on Scikit-learn’s internal optimizer, this notebook manually implements:

* Gradient computation
* Weight updates
* Bias optimization
* Learning rate scheduling
* Loss tracking
* Prediction logic

The goal of this project is to deeply understand how optimization algorithms actually work behind modern Machine Learning libraries.

---

# Why This Project?

Most ML projects only use high-level APIs.

This project focuses on understanding the **core mathematics and optimization mechanics** behind Machine Learning models.

Building algorithms manually helps understand:

* How models learn
* How gradients work
* Why optimization converges
* The effect of learning rates
* The role of stochastic updates

---

# Features

## Core ML Features

* Multiple Linear Regression
* Stochastic Gradient Descent
* Learning Rate Scheduling
* Dynamic Weight Updates
* Mean Squared Error Loss Tracking

## Visualizations

* Loss vs Epochs
* Learning Rate Decay
* Actual vs Predicted Graphs
* SGD Convergence Analysis

## Engineering Features

* Fully Vectorized NumPy Operations
* Object-Oriented Implementation
* Clean & Modular Code
* Professional Documentation

---

# Mathematical Formulation

## Multiple Linear Regression

$$
\hat{y} = w_1x_1 + w_2x_2 + \dots + w_nx_n + b
$$

---

## SGD Update Rule

$$
w := w - \eta \frac{\partial L}{\partial w}
$$

$$
b := b - \eta \frac{\partial L}{\partial b}
$$

Where:

- η = learning rate
- L = loss function
- w = weights
- b = bias/intercept


---

# Learning Rate Scheduling

A dynamic learning rate schedule is implemented to improve convergence stability.

$$
\eta_t = \frac{\eta_0}{1 + decay \times epoch}
$$

### Why Learning Scheduling Matters

Without scheduling:

* Training may oscillate
* Optimization becomes unstable
* Convergence can slow down

With scheduling:

* Faster early learning
* Stable late convergence
* Better optimization performance

---

# Dataset Used

This project uses the famous **Diabetes Dataset** from Scikit-learn.

### Dataset Information

| Property | Value      |
| -------- | ---------- |
| Features | 10         |
| Samples  | 442        |
| Task     | Regression |

---

# Technologies Used

<div align="center">

| Technology   | Purpose                |
| ------------ | ---------------------- |
| Python       | Core Programming       |
| NumPy        | Matrix Computation     |
| Pandas       | Data Handling          |
| Matplotlib   | Visualization          |
| Scikit-learn | Dataset & Benchmarking |

</div>

---

# Project Structure

```bash
├── Stochastic_Gradient_Descent_From_Scratch.ipynb
├── README.md
```

---

# Results

The custom implementation successfully learns regression parameters and achieves strong performance comparable to Scikit-learn’s SGD implementation.

### Evaluation Metric

* R² Score

---

# Concepts Covered

## Machine Learning

* Linear Regression
* Gradient Descent
* Stochastic Gradient Descent
* Optimization Algorithms
* Learning Rate Scheduling

## Mathematics

* Partial Derivatives
* Chain Rule
* Gradient Computation
* Loss Minimization

## Programming

* NumPy Vectorization
* OOP in Python
* Matrix Operations
* Random Sampling

---

# Future Improvements

Possible future extensions:

* Mini Batch Gradient Descent
* Momentum Optimization
* Adam Optimizer
* RMSProp
* Early Stopping
* Regularization (L1/L2)
* Feature Scaling Pipeline

---

# Key Takeaway

Modern Machine Learning frameworks internally perform operations very similar to what is implemented manually in this notebook.

Understanding these internals builds stronger intuition for:

* Deep Learning
* Neural Networks
* Optimization Theory
* ML Research

---

# Run Locally

```bash
git clone https://github.com/your-username/your-repository-name.git
```

Install dependencies:

```bash
pip install numpy pandas matplotlib scikit-learn
```

Run the notebook:

```bash
jupyter notebook
```

---

# Author

## Varun Saxena

