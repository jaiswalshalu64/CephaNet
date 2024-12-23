# CephaNet**
**CephaXNet: Landmark Detection for Medical Images**

**Overview**

CephaXNet is a convolutional neural network designed for landmark detection in medical images. The project uses image augmentation, deep learning techniques, and a custom architecture featuring a Squeeze-and-Excitation Block and Convolution-MaxPooling (CNM) layers. The model predicts the coordinates of anatomical landmarks in grayscale medical images.

**Table of Contents**

Project Features

Dataset Description

Model Architecture

Tools and Techniques Used

How to Run

Results

Acknowledgments

**Project Features**

Custom deep learning model: Incorporates Squeeze-and-Excitation Blocks, CNM layers, and skip connections.

Image preprocessing and augmentation: Increases dataset diversity using transformations such as zoom, shear, and flips.

End-to-end pipeline: Data preparation, training, validation, and testing.

Regression model: Predicts the x and y coordinates of landmarks in medical images.

**Dataset Description**

**Input images:** Grayscale patches of size 64x64 pixels.

**Labels:** Coordinates (x, y) of anatomical landmarks.


**Splits:**

Training: 70%

Validation: 10%

Testing: 20%


**Model Architecture**

Input size: (64, 64, 1)

**Convolutional Layers:**

1.CNM layers with ReLU activation and MaxPooling.

2.Squeeze-and-Excitation Block:

Improves feature recalibration for better learning.

**Fully Connected Layers:**

Dense layers with dropout for regression tasks.

**Optimizer:** Adam with a learning rate of 0.001.

**Loss Function:** Mean Squared Error (MSE).



**Tools and Techniques Used**

**Programming Language:** Python

**Libraries**:

**pandas:** Data handling.

**tensorflow.keras:** Deep learning model creation and training.

**sklearn:** Data splitting.

**matplotlib:** Visualizing training and validation loss.
**Data Augmentation:**
Horizontal flipping, zooming, shearing, and rescaling using ImageDataGenerator.
