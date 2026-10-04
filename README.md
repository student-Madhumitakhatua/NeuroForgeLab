# NeuroForgeLab 🧠

A PyTorch-based deep learning project for handwritten digit classification using the MNIST dataset.

## 📌 Project Overview

This project builds a fully connected neural network using PyTorch and implements the complete training process, including forward propagation, loss calculation, backpropagation, and optimizer updates.

Two neural network architectures were trained and compared based on validation performance.

## 🛠️ Technologies Used

- Python
- PyTorch
- Torchvision
- NumPy
- Matplotlib
- Scikit-learn

## 📊 Dataset

MNIST handwritten digit dataset.

- Training samples: 54,000
- Validation samples: 6,000
- Test samples: 10,000
- Image size: 28 × 28 pixels
- Classes: 10 digits (0–9)

## 🧠 Neural Network Architectures

### Architecture 1
`784 → 128 → 64 → 10`

### Architecture 2
`784 → 256 → 128 → 10`

Both architectures use ReLU activation functions and the Adam optimizer.

## ⚙️ Training Setup

- Loss Function: Cross-Entropy Loss
- Optimizer: Adam
- Learning Rate: 0.001
- Batch Size: 64
- Epochs: 5
- Train/Validation Split: 90/10

## 📈 Results

| Architecture | Validation Accuracy | Test Accuracy |
|---|---:|---:|
| 784 → 128 → 64 → 10 | **97.22%** | **97.26%** |
| 784 → 256 → 128 → 10 | 97.12% | Not evaluated |

### 🏆 Best Model

The first architecture achieved the best validation performance with **97.22% validation accuracy**.

Its final test accuracy was **97.26%**.

## 📉 Training Analysis

Training and validation loss curves were plotted for both architectures.

The validation loss generally decreased during training, with a slight increase in the final epoch indicating mild overfitting.

## 📁 Project Structure

```text
NeuroForgeLab/
├── data/
├── models/
│   └── mnist_best_model.pth
├── notebooks/
│   └── deep_learning_intro.ipynb
├── plots/
├── README.md
├── requirements.txt
└── .gitignore