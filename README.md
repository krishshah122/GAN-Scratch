# GAN from Scratch - Fashion MNIST

This project implements a simple Generative Adversarial Network (GAN) using TensorFlow to generate fashion item images similar to those in the [Fashion-MNIST](https://github.com/zalandoresearch/fashion-mnist) dataset.

## 📌 Project Overview

A **Generative Adversarial Network (GAN)** is a class of machine learning frameworks where two neural networks contest with each other:  
- The **Generator** tries to create realistic data.  
- The **Discriminator** tries to distinguish between real and fake data.

This notebook demonstrates how to:
- Load and preprocess the Fashion-MNIST dataset.
- Build a basic GAN from scratch using TensorFlow.
- Train the GAN to generate fake fashion item images.
- Visualize generator outputs across training epochs.

## 🚀 Tech Stack

- **Python**
- **TensorFlow 2.x**
- **TensorFlow Datasets (tfds)**
- **Matplotlib** for plotting results
- **NumPy**

## 🧠 Model Architecture

### Generator

- **Input**: Random noise vector (latent space)  
- **Output**: 28x28 grayscale image  
- **Layers**: Dense layers + BatchNorm + LeakyReLU + Reshape + Conv2DTranspose

### Discriminator

- **Input**: 28x28 image  
- **Output**: Probability of being a real image  
- **Layers**: Conv2D + LeakyReLU + Dropout + Flatten + Dense

### Loss Functions

- **Binary Crossentropy** used for both generator and discriminator  
- **Adam Optimizer** for both networks

## 🏋️ Training

- Trains over multiple epochs  
- The discriminator and generator are trained alternately  
- Generator improves in generating realistic images over time

## 📊 Results

After each epoch, generated samples are visualized and saved to track improvement.



