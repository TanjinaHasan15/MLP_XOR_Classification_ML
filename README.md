# MLP from Scratch: Solving the XOR Classification Task

## Overview
This project implements a **Multilayer Perceptron (MLP) from scratch using NumPy** to solve the **XOR classification problem**.  
The XOR problem is a classical non-linear classification task that cannot be solved by a single-layer perceptron but can be solved using an MLP with a hidden layer.



## Architecture
- **Input Layer**: 2 neurons (X1, X2)  
- **Hidden Layer**: 2 neurons (activation: Sigmoid / ReLU)  
- **Output Layer**: 1 neuron (activation: Sigmoid)  
- **Training Algorithm**: Backpropagation with Mean Squared Error (MSE) loss  
- **Optimization**: Gradient Descent  



## Features
- Implemented **from scratch in NumPy** (no high-level ML libraries).  
- Supports two activation functions in the hidden layer: **Sigmoid** and **ReLU**.  
- Tunable hyperparameters:  
  - Learning rate: `{0.01, 0.1, 0.5}`  
  - Iterations: `{500, 1000, 5000}`  
- Evaluation Metrics (implemented from scratch):  
  - Accuracy  
  - Precision  
  - Recall  
  - F1-Score  
  - ROC Curve + AUC  



## Results
- With **Sigmoid hidden layer**, learning rate `0.1`, and `5000` iterations → **100% accuracy**.  
- With **ReLU hidden layer**, convergence is slower but also reaches **100% accuracy** after sufficient iterations.  
- Small learning rates (`0.01`) → slower convergence.  
- High learning rates (`0.5`) → unstable oscillations.  


