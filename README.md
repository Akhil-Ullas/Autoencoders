

# Autoencoders — Representation Learning with MNIST & Fashion-MNIST

This repository contains implementations and experiments on **Autoencoders** carried out as part of my **Data Science & Machine Learning (DSML) internship**.
The focus is on **unsupervised representation learning**, **latent space analysis**, and **reconstruction behavior** using standard vision benchmarks.

---

## 📌 Objectives

* Learn compact **latent representations** of image data
* Study the effect of **bottleneck size and architecture depth**
* Compare dense vs convolutional encoders
* Analyze the role of **regularization and noise** in representation learning

---

## 📂 Datasets

Experiments were conducted using:

* **MNIST** — handwritten digits
* **Fashion-MNIST** — clothing and apparel images

These datasets allow controlled comparison across:

* Simple vs visually complex structures
* Dense vs spatial feature representations

---

## 🧠 Autoencoder Architectures Implemented

### 1. Vanilla Autoencoder

* Single hidden-layer encoder–decoder
* Baseline for reconstruction quality and compression

### 2. Deep Autoencoder

* Multiple hidden layers with symmetric encoder–decoder structure
* Increased representational capacity

### 3. Convolutional Autoencoder

* Convolution + pooling in encoder
* Upsampling / transpose convolution in decoder
* Better spatial feature preservation for image data

### 4. Sparse Autoencoder

* Sparsity constraints applied to latent representations
* Encourages selective neuron activation

### 5. Denoising Autoencoder

* Trained to reconstruct clean inputs from corrupted data
* Noise injection used as a regularization strategy

---

## 🔬 Experimental Focus

* Effect of **latent dimension size** on reconstruction loss
* Dense vs convolutional encoders on image structure retention
* Impact of sparsity and noise on feature robustness
* Reconstruction performance across MNIST vs Fashion-MNIST

---

## ⚙️ Training Details

* Loss function: Reconstruction loss (MSE / Binary Cross-Entropy as appropriate)
* Optimizer: Adam
* Models trained without labels (unsupervised setting)
* Performance evaluated via reconstruction quality and loss trends

---

## 📊 Evaluation

* Visual comparison of original vs reconstructed images
* Reconstruction loss analysis
* Qualitative assessment of learned representations

---

## 🛠️ Tech Stack

* Python
* TensorFlow
* Keras
* NumPy
* Matplotlib

---

## 📚 Key Learnings

* Autoencoders learn **data-dependent latent representations**, not generic compression
* Bottleneck size critically affects information retention
* Regularization (sparsity, noise) is essential to prevent identity mapping
* Convolutional autoencoders outperform dense models on image data

---


