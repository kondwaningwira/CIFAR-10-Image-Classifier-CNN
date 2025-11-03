# CIFAR-10-Image-Classifier-CNN
Deep Learning project to classify images from the CIFAR-10 dataset using a Convolutional Neural Network (CNN) built with Keras and TensorFlow.
# CIFAR-10 Image Classifier using Convolutional Neural Networks (CNN) 🖼️

This repository contains the code and resources for a deep learning project focused on image classification using the popular **CIFAR-10 dataset**.

The project implements a **Convolutional Neural Network (CNN)** built with **Keras** and **TensorFlow** to categorize images into 10 distinct classes.

## 🎯 Project Goal

The primary objective is to train a robust CNN model that can accurately classify low-resolution color images (32x32 pixels) from the CIFAR-10 dataset.

## 💾 Dataset Overview

The **CIFAR-10 dataset** consists of 60,000 32x32 color images in 10 classes, with 6,000 images per class.

The 10 classes are:
1.  **Airplane** ✈️
2.  **Automobile** 🚗
3.  **Bird** 🐦
4.  **Cat** 🐈
5.  **Deer** 🦌
6.  **Dog** 🐕
7.  **Frog** 🐸
8.  **Horse** 🐎
9.  **Ship** 🚢
10. **Truck** 🚚

## ⚙️ Key Technologies

* **Python**
* **TensorFlow** / **Keras** (For model construction and training)
* **NumPy** (For numerical operations)
* **Matplotlib** (For visualization)
* **ImageDataGenerator** (For real-time data augmentation)

## 🏗️ Model Architecture

The model is a Sequential CNN designed to extract hierarchical features from the image data. The architecture includes:

1.  **Convolutional Layers (`Conv2D`):** To learn features like edges and textures.
2.  **Pooling Layers (`MaxPooling2D`):** To downsample the feature maps and reduce computational load.
3.  **Batch Normalization:** To stabilize the learning process.
4.  **Dropout:** To prevent overfitting.
5.  **Dense Layers:** A final fully-connected layer with a **softmax** activation function for the 10-class classification output.

## 🧪 Training Strategy

The model is trained using several techniques to enhance performance and stability:

* **Optimizer:** **Adam** optimizer.
* **Loss Function:** **Categorical Cross-Entropy**.
* **Data Augmentation:** The `ImageDataGenerator` is used to introduce variations (e.g., shifts, flips) in the training data, improving generalization.
* **Callbacks:**
    * `ReduceLROnPlateau`: Dynamically reduces the learning rate when validation loss plateaus, helping the model converge better.
    * `EarlyStopping`: Stops training if the validation loss doesn't improve after a set number of epochs, preventing unnecessary training time and overfitting.

## 🚀 Getting Started

To run this project, you will need a Python environment with the required libraries.

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YourUsername/CIFAR-10-Image-Classifier-CNN.git](https://github.com/YourUsername/CIFAR-10-Image-Classifier-CNN.git)
    cd CIFAR-10-Image-Classifier-CNN
    ```
2.  **Install dependencies:**
    ```bash
    pip install tensorflow keras numpy matplotlib jupyter
    ```
3.  **Run the notebook:**
    Open the `CIFAR_Final_Project (1).ipynb` notebook in Jupyter or Google Colab and execute the cells.
