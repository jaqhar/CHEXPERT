# CHEXPERT MSc Project - Comparative Analysis of Multilabel Chest Radiograph Models

## Project Description

This project involved developing and evaluating various deep neural network architectures for multi-label classification of chest radiographs using the CheXpert dataset.

## Models Implemented

- ResNet34
- ResNet50
- ResNet101
- DenseNet121
- MobileNet

These models leverage transfer learning from ImageNet weights as a starting point. The models were further optimized through techniques like fine-tuning, regularization via dropout, data augmentation, learning rate scheduling, and early stopping.

## Training Framework

1. Loading the CheXpert dataset images and labels
2. Preprocessing and augmenting the images
3. Building generators for training and validation data
4. Loading pretrained base models like ResNet and DenseNet
5. Adding custom classification layers
6. Compiling and training the models with callbacks for learning rate scheduling and early stopping
7. Saving the trained models for later evaluation

The models were trained on Google Colab GPUs for computational acceleration.

## Evaluation and Analysis

- Accuracy, specificity, precision, recall
- F1 score (overall and per-class)
- Precision-recall curves
- Confusion matrices
- Hamming loss

Of all the models, DenseNet121 achieved the highest accuracy of 81.38% along with balanced metrics. ResNet50 also performed well. The comparative assessment provided insights into each model's strengths and limitations.

The analysis suggests pathways for further optimization of deep learning for automated chest radiograph interpretation.

## Requirements

- tensorflow >= 2.0
- keras
- pandas
- scikit-learn
- matplotlib

## References

- [CheXpert Dataset](https://drive.google.com/drive/folders/1i7Mr78I63-nNxOOgYPaPszZnGy4eSbl2?usp=drive_link)

- [Stanford ML Group](https://stanfordaimi.azurewebsites.net/datasets/8cbd9ed4-2eb9-4565-affc-111cf4f7ebe2) 
