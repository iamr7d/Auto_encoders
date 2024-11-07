# Autoencoder for MNIST Dataset

This project implements a simple Autoencoder model using TensorFlow and Keras to learn compressed representations (latent space) of images in the MNIST dataset. The model is trained to reconstruct the input images after compressing them into a lower-dimensional latent space. The code also includes visualizations to show the latent space and the reconstruction process.

## Table of Contents
- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
- [Code Explanation](#code-explanation)
- [Visualizations](#visualizations)
- [License](#license)

## Introduction

The goal of this project is to use an autoencoder to learn the compressed representation (latent space) of MNIST images. An autoencoder consists of two main parts:
1. **Encoder**: Maps the input image to a latent space of lower dimensions.
2. **Decoder**: Reconstructs the original image from the latent space representation.

This project uses a two-dimensional latent space for easy visualization. After training the autoencoder, the latent space is visualized with color-coded digits, and various stages of the autoencoder's performance (original image, latent space representation, and reconstructed image) are also visualized.

## Prerequisites

To run this code, you will need to have the following libraries installed:
- **TensorFlow**: Deep learning framework used for building the autoencoder.
- **NumPy**: For numerical operations.
- **Matplotlib**: For visualizing the results.
- **scikit-learn**: For dimensionality reduction (e.g., PCA, t-SNE) and clustering.

You can install the required dependencies with the following command:
```bash
pip install tensorflow numpy matplotlib scikit-learn
