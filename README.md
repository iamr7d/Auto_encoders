# Autoencoder for MNIST Dataset

## Understanding Autoencoders
![image](https://github.com/user-attachments/assets/87d868f0-6c1c-4331-b166-f9b49e11cbd2)


For a deeper understanding of autoencoders and their applications, you can read the detailed article I wrote on Medium.

[Understanding Autoencoders - Medium Article](https://medium.com/p/6befc7016a9f/edit)

This article provides an intuitive explanation, a real-world analogy, and detailed math behind how autoencoders work, including how they compress and reconstruct data.

This project implements a simple Autoencoder model using TensorFlow and Keras to learn compressed representations (latent space) of images in the MNIST dataset. The model is trained to reconstruct the input images after compressing them into a lower-dimensional latent space. The code also includes visualizations to show the latent space and the reconstruction process.

## Table of Contents
- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
- [Code Explanation](#code-explanation)
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
```
## Getting Started

### Clone this repository:
```bash
git clone https://github.com/your-repository-url.git
cd your-repository-folder
```
### Run the Python script:
```bash
git clone https://github.com/your-repository-url.git
cd your-repository-folder
```
## Code Explanation

#### 1. Loading and Preprocessing the MNIST Dataset:
The MNIST dataset is loaded and normalized (pixel values between 0 and 1). It is also reshaped to fit the input shape of the autoencoder model.

#### 2. Encoder Model:
The encoder part of the autoencoder is a neural network that compresses the input image into a lower-dimensional latent space. It uses two fully connected layers followed by an output layer representing the latent space.

#### 3. Decoder Model:
The decoder reconstructs the original image from the latent space. It uses a fully connected network to upsample the latent representation back to the original image dimensions (28x28).

#### 4. Autoencoder Model:
The autoencoder combines both the encoder and decoder models. It is trained by minimizing the reconstruction loss (Mean Squared Error) between the original and reconstructed images.

#### 5. Training:
The autoencoder is trained using the MNIST training dataset for 10 epochs with a batch size of 256. The loss is calculated using the MSE (Mean Squared Error) loss function.

#### 6. Visualization:

#### Latent Space Visualization:
A scatter plot of the latent space where each point is colored according to the digit label.

#### Data at Different Stages:
For a few test samples, the original image, latent space encoding, and reconstructed image are displayed side by side.

## License
This project is licensed under the MIT License - see the LICENSE file for details.


