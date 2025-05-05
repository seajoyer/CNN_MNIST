# CNN for MNIST Digit Classification

This project implements a Convolutional Neural Network (CNN) to classify handwritten digits from the MNIST dataset using PyTorch.

## Project Overview

The MNIST dataset consists of 28x28 grayscale images of handwritten digits (0-9). This implementation achieves 99.06% accuracy on the test set using a simple CNN architecture.

## Model Architecture

The CNN architecture includes:
- 2 convolutional layers with ReLU activation
- 2 max pooling layers
- 2 fully connected layers

```
CNN Architecture:
Input (1x28x28) → Conv2d(64 filters) → ReLU → MaxPool → 
Conv2d(128 filters) → ReLU → MaxPool → 
Flatten → FC(1024) → FC(10) → Output
```

## Hyperparameters

- Epochs: 10
- Batch Size: 200
- Loss Function: CrossEntropyLoss
- Optimizer: Adam

## Results

- Final Training Loss: 0.0103
- Test Accuracy: 99.06%
