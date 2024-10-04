# Two-Layer Perceptron for Parity Problem

This notebook implements a **two-layer perceptron** to solve the **4-bit parity problem** using **backpropagation**.

## Data Generation

We generate a dataset where the input consists of all possible 4-bit binary numbers, and the output is 1 if the input has an odd number of 1s, and 0 otherwise.

## Neural Network Architecture

The neural network consists of:
- 4 input neurons (for the 4-bit binary input)
- 4 hidden neurons in the hidden layer
- 1 output neuron (for predicting the parity)

We initialize weights and biases randomly and use **sigmoid activation** for all neurons.

## Training Procedure

The network is trained using backpropagation with different learning rates. We measure the loss (error) at each epoch and track how quickly the network converges for different values of `η` (learning rate).

## Results

The learning curves below show how the network performs with various learning rates. As expected:
- Lower learning rates (e.g., `0.05`) result in slower convergence.
- Higher learning rates (e.g., `0.3`) allow the network to converge faster, but beyond a certain point, it may get stuck in local minima.

## Conclusion

In this notebook, we explored how varying the learning rate affects the convergence of a neural network trained to solve the parity problem. The results show that a balanced learning rate is essential for efficient training.
