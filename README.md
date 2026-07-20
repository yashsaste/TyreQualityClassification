# Tyre Quality Classification using Deep Learning

## Project Overview

This project presents an automated tyre quality classification system developed using Deep Learning techniques. The objective is to classify tyre images into two categories:

- Good Tyres
- Defective Tyres

Two deep learning approaches were implemented and compared:

- Custom Convolutional Neural Network (CNN)
- Transfer Learning using ResNet50

The models were developed using the PyTorch framework and evaluated using standard classification metrics.

---

## Dataset

The dataset consists of tyre images belonging to two classes:

- Good
- Defective

### Dataset Split

| Dataset | Number of Images |
|----------|-----------------:|
| Training | 1297 |
| Validation | 278 |
| Testing | 278 |
| **Total** | **1853** |


The project uses a publicly available tyre image dataset obtained from Kaggle.

---

## Image Preprocessing

The following preprocessing steps were applied:

- Resize images to **224 × 224** pixels
- Convert images to tensors
- Normalize using ImageNet mean and standard deviation

---

## Models Implemented

### Custom CNN

The custom CNN architecture consists of:

- 4 Convolutional Blocks
- Batch Normalization
- ReLU Activation
- Max Pooling
- Adaptive Average Pooling
- Fully Connected Layers
- Dropout Regularization

### ResNet50

The transfer learning model includes:

- Pretrained ResNet50
- Frozen feature extraction layers
- Modified fully connected classifier
- Fine-tuning for tyre classification

---

## Hyperparameter Experiments

The following experiments were conducted using the custom CNN:

- Optimizer Comparison (Adam vs SGD)
- Learning Rate Comparison
- CNN Depth Comparison (3 vs 4 Convolutional Blocks)
- Epoch Comparison (10, 15 and 20 Epochs)

---

## Performance

| Model | Test Accuracy |
|--------|--------------:|
| Custom CNN | **87.77%** |
| ResNet50 | **95.68%** |

The pretrained ResNet50 achieved the highest performance, demonstrating the effectiveness of transfer learning for tyre quality classification.

---

## Evaluation Metrics

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- Classification Report

---

## Libraries

- PyTorch
- NumPy
- Matplotlib
- Jupyter Notebook

---

## Repository Structure

```
TyreQualityClassification/

├── notebook/
├── models/
├── report/
├── results/
├── README.md
├── requirements.txt
├── LICENSE
└── .gitignore
```

---

## References

1. Krizhevsky, A., Sutskever, I., & Hinton, G. E. (2012). *ImageNet Classification with Deep Convolutional Neural Networks.*

2. He, K., Zhang, X., Ren, S., & Sun, J. (2016). *Deep Residual Learning for Image Recognition.*

---

## Author

**Yash Saste**

Department of Applied Mechanics

Indian Institute of Technology, Madras

Developed using **PyTorch** for deep learning-based tyre quality classification.
