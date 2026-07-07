# Lung Cancer Detection and Classification using Deep Learning

A deep learning project for automated multi-class lung cancer classification from CT scan images using transfer learning. The project compares multiple convolutional neural network (CNN) architectures and evaluates their performance on medical imaging data.

## Overview

Lung cancer is one of the leading causes of cancer-related deaths worldwide. Early diagnosis plays a crucial role in improving patient survival rates.

This project uses transfer learning on CT scan images to classify different types of lung cancer. Multiple pretrained CNN architectures were trained, fine-tuned, and compared using standard evaluation metrics to identify the best-performing model.

## Features

- Multi-class lung cancer classification
- Transfer learning using pretrained CNN models
- CT scan image preprocessing
- Data augmentation for improved model generalization
- Performance comparison across multiple deep learning architectures
- Evaluation using standard classification metrics

## Models Used

- ResNet50
- ResNet101
- DenseNet121
- VGG16
- MobileNetV2

The models were fine-tuned using:

- Transfer Learning
- Dropout Regularization
- Early Stopping
- Learning Rate Scheduling

## Dataset

The project uses approximately **18,500 CT and PET DICOM images** belonging to four lung cancer categories.

### Classes

- Adenocarcinoma
- Squamous Cell Carcinoma
- Small Cell Carcinoma
- Large Cell Carcinoma

> **Note:** The dataset is not included in this repository due to its size and licensing restrictions.

## Image Preprocessing

The preprocessing pipeline includes:

- DICOM image loading
- Slice filtering
- Image resizing
- Pixel normalization
- Data augmentation
  - Rotation
  - Horizontal flipping

## Results

| Model | Accuracy |
|--------|----------|
| ResNet50 | 98.62 |
| ResNet101 | 98.57 |
| DenseNet121 | 91.94 |
| VGG16 | 97.35|
| MobileNetV2 | 95.06 |

**Best Performing Model:** ResNet50
<img width="703" height="771" alt="image" src="https://github.com/user-attachments/assets/c66f14d4-9cf4-48ac-b0eb-1679c94c9134" />

Evaluation metrics used:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- Classification Report

## Technologies Used

- Python
- TensorFlow
- Keras
- OpenCV
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
