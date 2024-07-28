# Image Classification with CIFAR-10: Custom Neural Network vs. PyTorch CNN

## Overview

This project demonstrates image classification on the CIFAR-10 dataset using two different approaches:

1. A custom neural network implementation from scratch.
2. A convolutional neural network (CNN) built using PyTorch.

The CIFAR-10 dataset consists of 60,000 32x32 color images in 10 classes, with 6,000 images per class. The task is to classify these images into one of the 10 categories.

## Project Structure

### 1. Custom Neural Network Implementation

- **Data Preparation:**

  - Load, normalize, and preprocess CIFAR-10 dataset using `torchvision`.
  - Convert images to flattened numpy arrays for custom processing.

- **Neural Network Class:**

  - Implement a neural network with He initialization, forward and backward propagation, and Adam optimization.
  - Cost function includes cross-entropy loss with L2 regularization.

- **Training:**

  - Train the custom neural network on the CIFAR-10 dataset.
  - Evaluate and print training and validation accuracy.

- **Prediction and Visualization:**
  - Predict labels for test images and display them using `matplotlib`.

### 2. PyTorch CNN Implementation

- **Data Preparation:**

  - Use PyTorch's `DataLoader` to load and preprocess CIFAR-10 dataset.
  - Split dataset into training and validation sets.

- **CNN Architecture:**

  - Define and train two CNN models:
    - **SimpleCNN:** Basic CNN with convolutional layers, batch normalization, and dropout.
    - **ModifiedCNN:** Enhanced CNN with additional convolutional layers and increased dropout.

- **Training and Validation:**
  - Train the models using PyTorch's optimization tools.
  - Evaluate and print validation accuracy.

## Requirements

- Python 3.x
- PyTorch
- NumPy
- Matplotlib
- torchvision

## Installation

To install the required packages, use `pip`:

```bash
pip install torch torchvision numpy matplotlib
```
