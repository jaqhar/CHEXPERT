# CHEXPERT
MSc Project - Comparative Analysis of Multilabel Chest Radiograph Models
This project involved developing and evaluating various deep neural network architectures for multi-label classification of chest radiographs using the CheXpert dataset.

Models Implemented
ResNet34
ResNet50
ResNet101
DenseNet121
MobileNet
These models leverage transfer learning from ImageNet weights as a starting point. The models were further optimized through techniques like fine-tuning, regularization via dropout, data augmentation, learning rate scheduling and early stopping.

Training Framework
Loading the CheXpert dataset images and labels
Preprocessing and augmenting the images
Building generators for training and validation data
Loading pretrained base models like ResNet and DenseNet
Adding custom classification layers
Compiling and training the models with callbacks for learning rate scheduling and early stopping
Saving the trained models for later evaluation
The models were trained on Google Colab GPUs for computational acceleration.

Evaluation and Analysis
Accuracy, specificity, precision, recall
F1 score (overall and per-class)
Precision-recall curves
Confusion matrices
Hamming loss
Of all the models, DenseNet121 achieved the highest accuracy of 81.38% along with balanced metrics. ResNet50 also performed well. The comparative assessment provided insights into each model's strengths and limitations.

The analysis suggests pathways for further optimization of deep learning for automated chest radiograph interpretation.

Requirements
tensorflow >= 2.0
keras
pandas
scikit-learn
matplotlib

References
CheXpert Dataset
Keras Applications for pretrained models
Stanford ML Group
