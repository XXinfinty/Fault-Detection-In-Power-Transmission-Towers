# Fault-Detection-In-Power-Transmission-Towers

Overview
This project implements a deep learning-based image classification system to identify faults in power transmission systems. The model is trained on the insPLAD dataset using a Convolutional Neural Network (CNN) with data augmentation, dropout, and L2 regularization. It achieves strong performance, with a test accuracy of 83.72%.

The project includes:

Model training and evaluation scripts

Model saving and loading

Table of Contents
Overview

Dataset

Model Architecture

Training Details

Performance

Testing

Dataset
Name: insPLAD (Power Transmission Fault Images)

Classes: 11 

Layers:

Data Augmentation (random flip, rotation, zoom)

3x Conv2D + MaxPooling2D

GlobalAveragePooling2D

Dense(128) with ReLU and Dropout(0.5)

Output: Dense(11) with Softmax

Regularization: Dropout(0.5), L2(0.001)

Optimizer: Adam, learning rate scheduler with ReduceLROnPlateau

Training Details
Loss: Sparse categorical crossentropy

Metrics: Accuracy

Early stopping: Enabled (restore best weights)

Data split: Train / Validation / Test

Peak Validation Accuracy: ~78%

Test Accuracy: 83.72%
