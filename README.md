# Skin Disease Classification using Transfer Learning and Machine Learning

## Project Overview

This project focuses on automated skin disease classification using deep learning and machine learning techniques. A hybrid classification pipeline was developed using transfer learning-based feature extraction and machine learning classifiers for comparative performance evaluation.

The system analyzes dermatological images and predicts different categories of skin diseases using extracted deep learning features.

---

# Features

* Skin disease image classification
* Transfer learning using pretrained CNN models
* Deep feature extraction
* Comparative evaluation of multiple classifiers
* Prediction on custom skin disease images
* Confusion matrix visualization
* Accuracy comparison plots

---

# Dataset

The project uses the HAM10000 (Human Against Machine with 10000 Training Images) dataset for skin disease classification.

HAM10000 is a widely used dermatoscopic image dataset containing multiple categories of pigmented skin lesions used for medical image analysis and deep learning research.

### Dataset Source

* [HAM10000 Dataset (Kaggle)](https://www.kaggle.com/datasets/kmader/skin-cancer-mnist-ham10000?utm_source=chatgpt.com)

### Dataset Categories

The dataset contains images from multiple skin lesion categories including:

* Melanocytic nevi
* Melanoma
* Benign keratosis-like lesions
* Basal cell carcinoma
* Actinic keratoses
* Vascular lesions
* Dermatofibroma

---

# Data Preprocessing and Cleaning

The following preprocessing steps were performed before model training:

* Removed corrupted or unreadable image files
* Resized all images to `224 x 224`
* Normalized pixel values
* Converted categorical labels into numerical classes
* Split dataset into training, validation, and testing sets
* Applied image augmentation using `ImageDataGenerator`

### Data Augmentation Techniques

* Rotation
* Horizontal flipping
* Zooming
* Rescaling

These preprocessing techniques improved model generalization and reduced overfitting.

---

# Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* OpenCV
* Matplotlib
* Scikit-learn

---

# Models Implemented

## Deep Learning Model

* VGG16

The pretrained VGG16 model was used for deep feature extraction from skin disease images.

## Machine Learning Models

* Support Vector Machine
* Random Forest

The extracted deep learning features were used to train machine learning classifiers for comparative evaluation.

---

# Workflow

1. Dataset preprocessing and cleaning
2. Image augmentation and normalization
3. Transfer learning using VGG16
4. Feature extraction from convolutional layers
5. Training SVM and Random Forest classifiers
6. Comparative performance analysis
7. Prediction on custom skin disease images

---

# Prediction System

The notebook supports prediction on custom skin disease images.

### Prediction Workflow

* Upload input image
* Preprocess image
* Extract deep learning features
* Generate prediction using trained classifier
* Display predicted skin disease category

---

# Model Evaluation

The models were evaluated using:

* Accuracy
* Confusion Matrix
* Classification Report
* Comparative Accuracy Visualization

The transfer learning-based CNN model achieved the best overall performance for skin disease classification.

---

# Results

The project demonstrates that transfer learning-based deep features significantly improve skin disease image classification performance compared to standalone traditional machine learning approaches.

Among the evaluated models, the VGG16-based transfer learning model achieved the best overall prediction performance.

---

# Future Improvements

* Increase dataset size
* Improve class balancing
* Deploy as a web application
* Add real-time image upload functionality
* Experiment with advanced architectures such as EfficientNet and DenseNet
* Integrate explainable AI techniques for medical interpretability
