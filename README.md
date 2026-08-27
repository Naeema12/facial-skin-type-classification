# Facial Skin Type Classification

A deep learning project for classifying facial skin types into three categories:

- **Dry**
- **Normal**
- **Oily**

The project investigates the use of **ResNet18 and transfer learning** for facial skin type classification and compares several training strategies to improve generalization on unseen images.

## Project Overview

Facial skin type classification is a computer vision problem in which facial images are categorized according to their predominant skin type.

In this project, a ResNet18-based classifier was developed and evaluated through a series of controlled experiments. The goal was not only to train a model, but also to investigate how different training strategies affect model generalization.

The workflow includes:

1. Dataset inspection
2. Data quality assessment
3. Label and content inspection
4. Face detection and dataset preparation
5. Duplicate removal
6. Image preprocessing
7. Data augmentation
8. ResNet18 transfer learning
9. Multiple training experiments
10. Model evaluation
11. Confusion matrix analysis
12. Sample image prediction

## Model

The main architecture used in this project is **ResNet18**.

ResNet18 is a convolutional neural network (CNN) architecture based on residual connections. Instead of training an entirely new network from random initialization, this project uses **transfer learning**, starting from pretrained ResNet18 weights and adapting the final classification layers to the three skin-type classes.

### Classes

```text
0 → Dry
1 → Normal
2 → Oily
