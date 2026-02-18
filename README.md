# Data-Augmentation-with-the-CIFAR10-dataset
CIFAR10 images are of size 32 × 32 and contains pictures corresponding to 10 classes (e.g. airplane, cat, dog, ...) and our goal is deducing which class the image corresponds to. The dataset has 50,000 training and 10,000 test examples.

**ResNet-18 Image Classification on CIFAR-10**

This repository implements a ResNet-18 architecture using PyTorch to classify the CIFAR-10 dataset. The project explores the impact of Data Augmentation on model generalization and training stability.

**Architecture**: Utilized the ResNet-18 model, which uses skip connections (short-cuts) to allow gradients to flow through deeper layers without vanishing.

**Optimization**: Used the Adam optimizer with a learning rate of 0.001 and Cross-Entropy Loss.

**Data Augmentation Experiment**

I compared the performance of the model under two different conditions:

**Baseline**: Training on raw images.

**Augmented**: Training with Random Horizontal Flips and Random Crops.

**Result**: Data augmentation significantly reduced the gap between training and testing accuracy, effectively acting as a regularizer.

**Training Dynamics**

The experiments demonstrated that even with a smaller subset of data (1,000 samples per class), a powerful architecture like ResNet can achieve high performance when paired with proper regularization and augmentation techniques.

**Tech Stack**

**Framework**: PyTorch

**Computer Vision**: Torchvision

**Numerical Computing**: NumPy

**Visualization**: Matplotlib

**How to Run**

1.Clone the repository.

2.Install dependencies: pip install torch torchvision numpy matplotlib.

3.Open HW4_codes_thi_thi_khine.ipynb to view the ResNet implementation and the comparison plots between the baseline and augmented models.

