# Deep Learning Project 5 – Activation Functions

## Project Overview

This project demonstrates and compares three commonly used activation functions in Deep Learning:

- **Sigmoid**
- **ReLU (Rectified Linear Unit)**
- **Tanh (Hyperbolic Tangent)**

The implementation is created in Python using **NumPy** for numerical calculations and **Matplotlib** for visualization.

## Objective

The objective of this project is to understand how different activation functions transform input values and to visualize their behavior over a continuous range of inputs.

## Technologies Used

- Python
- NumPy
- Matplotlib
- Jupyter Notebook

## Activation Functions

### 1. Sigmoid

The Sigmoid function is implemented as:

```python
def sigmoid(x):
    return 1 / (1 + np.exp(-x))
```

It maps input values to a range between **0 and 1**.

### 2. ReLU

The ReLU function is implemented as:

```python
def relu(x):
    return np.maximum(0, x)
```

It returns **0 for negative inputs** and returns the input value for positive inputs.

### 3. Tanh

The Tanh function is implemented as:

```python
def tanh(x):
    return np.tanh(x)
```

It maps values approximately to the range **-1 to 1**.

## Implementation

The notebook first imports NumPy and Matplotlib:

```python
import numpy as np
import matplotlib.pyplot as plt
```

The three activation functions are then defined and tested using input values from **-5 to 5**.

A continuous input range from **-5 to 5** containing 1000 points is also generated to plot and compare the three activation functions.

## Output

The project produces:

1. Numerical outputs of Sigmoid, ReLU, and Tanh for selected input values.
2. A combined graph comparing the three activation functions.

### Observations

- **Sigmoid** produces smooth outputs between 0 and 1.
- **ReLU** outputs zero for negative values and follows the input for positive values.
- **Tanh** produces smooth outputs between approximately -1 and 1.
- The plotted graph makes the different behaviors of the activation functions easy to compare.

## Project Structure

```text
DL_Project_5/
│
├── DL_project_5.ipynb
└── README.md
```

## How to Run

1. Install Python.
2. Install the required libraries:

```bash
pip install numpy matplotlib jupyter
```

3. Open the notebook:

```bash
jupyter notebook DL_project_5.ipynb
```

4. Run all cells in order.

## Conclusion

This project provides a practical demonstration of three fundamental activation functions used in neural networks. By calculating their outputs and plotting their curves, the project shows how Sigmoid, ReLU, and Tanh respond differently to input values.
