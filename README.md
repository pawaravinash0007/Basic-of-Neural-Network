<div align="center">

# 🔬 Basic-of-Neural-Network

### Neural Network Fundamentals from Scratch

[![Language](https://img.shields.io/badge/Language-Python-blue?style=flat-square&logo=python)](.)
[![Framework](https://img.shields.io/badge/Framework-NumPy%20%7C%20TensorFlow-orange?style=flat-square)](.)
[![Notebook](https://img.shields.io/badge/Notebook-Jupyter-orange?style=flat-square&logo=jupyter)](.)
[![Level](https://img.shields.io/badge/Level-Beginner%20Friendly-green?style=flat-square)](.)

</div>

---

## 📖 Overview

A beginner-friendly introduction to **Artificial Neural Networks (ANN)** — built from scratch using NumPy before transitioning to TensorFlow/Keras. This project demystifies how neural networks learn by implementing forward propagation, backpropagation, and gradient descent manually.

---

## 🎯 What You'll Learn

- What is a neuron and how does it work?
- Activation functions: Sigmoid, ReLU, Tanh, Softmax
- Forward propagation — computing predictions
- Loss functions: MSE, Binary Cross-Entropy, Categorical Cross-Entropy
- Backpropagation — computing gradients
- Gradient Descent and its variants (SGD, Adam, RMSProp)
- Building multi-layer perceptrons (MLP)

---

## 🏗️ Implementation Stages

### Stage 1 — From Scratch (NumPy)
```python
# Single neuron
z = np.dot(weights, inputs) + bias
output = sigmoid(z)

# Backpropagation
dW = (1/m) * np.dot(dZ, A_prev.T)
db = (1/m) * np.sum(dZ, axis=1, keepdims=True)
```

### Stage 2 — With Keras
```python
model = Sequential([
    Dense(64, activation='relu', input_shape=(n_features,)),
    Dense(32, activation='relu'),
    Dense(1, activation='sigmoid')
])
model.compile(optimizer='adam', loss='binary_crossentropy', metrics=['accuracy'])
```

---

## 📚 Topics Covered

| Topic | Description |
|-------|-------------|
| Perceptron | Single-layer binary classifier |
| MLP | Multi-layer perceptron |
| Activation Functions | Sigmoid, ReLU, Tanh, Softmax |
| Loss Functions | MSE, BCE, CCE |
| Optimizers | SGD, Momentum, Adam |
| Regularization | L1, L2, Dropout |
| Batch Normalization | Stabilizing training |

---

## 🚀 Getting Started

```bash
git clone https://github.com/pawaravinash0007/Basic-of-Neural-Network.git
cd Basic-of-Neural-Network
pip install numpy matplotlib tensorflow jupyter
jupyter notebook Neural_Network_Basics.ipynb
```

---

## 📁 Repository Structure

```
Basic-of-Neural-Network/
├── 01_Perceptron.ipynb             # Single neuron from scratch
├── 02_MLP_NumPy.ipynb              # Multi-layer perceptron (NumPy)
├── 03_Activation_Functions.ipynb   # Activation function comparison
├── 04_Backpropagation.ipynb        # Backprop derivation & code
├── 05_Keras_MLP.ipynb              # Keras implementation
└── README.md
```

---

## 🛠️ Tech Stack

`Python` · `NumPy` · `TensorFlow` · `Keras` · `Matplotlib` · `Jupyter`

---

## 👤 Author

**Avinash Pawar** | [@pawaravinash0007](https://github.com/pawaravinash0007)

<div align="center">⭐ Star this repo if you find it useful! ⭐</div>
