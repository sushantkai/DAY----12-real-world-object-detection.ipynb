🌟 U-Net Based Image Super-Resolution

A Deep Learning Approach to Enhance Image Resolution

📌 Project Overview

This project implements a U-Net model for image super-resolution, trained on the CelebA dataset.
The goal is to upscale low-resolution (64×64) images into high-resolution (256×256) outputs using deep learning.

The notebook demonstrates:

Dataset loading & preprocessing

U-Net architecture for super-resolution

Model training with MAE loss

Visual outputs generated after each epoch

Evaluation of reconstructed high-resolution images

🚀 Model Architecture — U-Net

U-Net is widely used for image-to-image translation tasks because of:

Encoder–decoder structure

Skip connections

Ability to preserve spatial information

In this project, U-Net learns to map low-resolution images to high-resolution outputs.

📂 Dataset — CelebA

Contains 200k+ celebrity face images

Resized to 64×64 (low-res) and 256×256 (target high-res)

Preprocessed for training (normalization, batching, shuffling)

🧠 Training Summary

Loss Function: Mean Absolute Error (MAE)

Optimizer: Adam

Training Behavior:

MAE consistently decreases over epochs

Generated samples improve visually over time

This shows that the model successfully learns high-resolution reconstruction.

📊 Results

The model reconstructs sharper and more detailed images compared to the low-res inputs.

Sample outputs after each epoch show noticeable improvement.

You can view sample outputs in this repository under the results/ folder (optional, if you add images).

📈 Possible Improvements

To further enhance performance, consider:

🔹 Perceptual Loss (VGG-based)
Produces sharper, more realistic textures.

🔹 GAN-based Super-Resolution Models
Such as SRGAN, ESRGAN.

🔹 Larger or More Diverse Dataset
Helps the model generalize better.

🔹 Hyperparameter Tuning
Batch size, learning rate, depth of U-Net, etc.

🛠️ Tech Stack

Python

TensorFlow / Keras

NumPy

Matplotlib

Google Colab

CelebA Dataset
