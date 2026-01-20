# lung-cancer-detection-ct
Lung cancer classification from CT images using EfficientNetB0 transfer learning

# Lung Cancer Detection from CT Images

This project focuses on automated lung cancer classification from chest CT images using deep learning techniques.

## Overview
- Task: Multi-class classification of lung CT images  
- Classes: Benign, Malignant, Normal  
- Approach: Transfer learning with EfficientNetB0  
- Platform: Google Colab

## Dataset
The IQ-OTH/NCCD lung CT dataset was used.  
Due to class imbalance and variability in image quality, exploratory data analysis (EDA) was performed prior to model training.

## Preprocessing
The following preprocessing pipeline was applied:
- Image resizing to 224×224
- Grayscale conversion
- Contrast enhancement using CLAHE
- Pixel intensity normalization

## Model
- Backbone: EfficientNetB0 (ImageNet pre-trained)
- Grayscale CT images adapted to RGB-compatible input
- Data augmentation applied to the training set
- Training strategies: early stopping, learning rate scheduling, model checkpointing

## Results
- Train / Validation / Test split: 70 / 15 / 15
- **Test accuracy: ~89.8%**
- Performance evaluated using confusion matrix and accuracy-based metrics

## Project Links
- Google Colab Notebook (view-only): https://colab.research.google.com/drive/1mgmVdcUkxqWZEJlSoVtWiRZcez7MUFwH?usp=sharing
- Dataset: https://www.kaggle.com/datasets/hamdallak/the-iqothnccd-lung-cancer-dataset

## Notes
This project was developed as part of the *Introduction to Image Processing* course and follows an academic-style experimental workflow.

