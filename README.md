# Chest X-Ray Disease Detection using Deep Learning

## Overview

Chest diseases such as Tuberculosis (TB) and Pneumonia continue to be major global health concerns. Early identification through chest X-ray analysis can assist healthcare professionals in screening and prioritizing patients for further diagnosis.

This project presents a deep learning-based system for classifying chest X-ray images into three categories:

- Normal
- Tuberculosis (TB)
- Pneumonia

The project involved curating and organizing a chest X-ray dataset containing over 10,000 images. In addition to publicly available data, clinically validated chest X-ray images were incorporated with guidance from a medical professional to improve dataset quality and diversity.

The primary objective was to train, evaluate, and compare multiple deep learning architectures to determine the most effective model for multi-class chest disease classification.

## Dataset

The dataset consists of **10,524 chest X-ray images** distributed across three classes.

| Split | Normal | TB | Pneumonia | Total |
|---------|---------|---------|---------|---------|
| Training | 2313 | 2313 | 2313 | 6939 |
| Validation | 885 | 486 | 420 | 1791 |
| Test | 887 | 487 | 420 | 1794 |
| Total | 4085 | 3286 | 3153 | 10524 |

### Dataset Preparation

- Curated and organized chest X-ray images into three diagnostic categories.
- Performed data cleaning and preprocessing before training.
- Incorporated additional clinically validated X-ray images with medical guidance.
- Created separate training, validation, and testing splits for unbiased evaluation.

## Models Evaluated

Three Convolutional Neural Network (CNN) architectures were trained and evaluated:

### DenseNet121
- Accuracy: **80%**

### EfficientNetB0
- Accuracy: **76%**

### ResNet50
- Accuracy: **75%**

## Performance Comparison

| Model | Accuracy |
|---------|---------|
| DenseNet121 | 80% |
| EfficientNetB0 | 76% |
| ResNet50 | 75% |

DenseNet121 achieved the highest accuracy and delivered the best overall performance on the dataset.

## Methodology

1. Dataset collection and curation
2. Image preprocessing and normalization
3. Model development using CNN architectures
4. Model training and validation
5. Performance evaluation on unseen test data
6. Comparative analysis of model performance

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
- Jupyter Notebook

## Repository Structure

```text
Notebooks/
├── densenet121-improvefinal.ipynb
├── resnet50-final-improve.ipynb
└── testingallmodels.ipynb
