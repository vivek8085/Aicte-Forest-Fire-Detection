# Fire Detection Using Convolutional Neural Networks

## Overview
This project implements a fire detection system using Convolutional Neural Networks (CNNs) to classify images as either containing fire or not. The model is trained on a dataset of wildfire images and can predict the presence of fire in new images.

## Table of Contents
- [Installation](#installation)
- [Dataset](#dataset)
- [Usage](#usage)
- [Model Architecture](#model-architecture)
- [Training](#training)
- [Evaluation](#evaluation)
- [Prediction](#prediction)
- [Example](#Example_Usage)

## Installation
To run this project, you need to have Python installed along with the following libraries:
- TensorFlow
- NumPy
- Matplotlib
- Kaggle

You can install the required libraries using pip:
```bash
pip install tensorflow numpy matplotlib kaggle

```
## Dataset
The dataset used for training and testing the model is the Wildfire Dataset, which can be downloaded from Kaggle. The dataset contains images categorized into two classes:

-Fire
-No Fire

# The dataset is structured into three directories:
-train: for training the model
-val: for validating the model
-test: for testing the model

## Usage
Clone the repository:

```bash
git clone https://github.com/vivek8085/Aicte-Forest-Fire-Detection
cd Aicte-Forest-Fire-Detection
```
Download the dataset using Kaggle API:

```bash
import kagglehub
path = kagglehub.dataset_download("elmadafri/the-wildfire-dataset")
print("Path to dataset files:", path)
```
Run the fire_detection.py script to train the model and evaluate its performance.

## Model Architecture
The CNN model consists of the following layers:

-Input layer
-Convolutional layers with ReLU activation
-MaxPooling layers
-Flatten layer
-Dense layers with Dropout for regularization
-Output layer with sigmoid activation for binary classification

## Training
The model is trained using the following parameters:

-Batch size: 32
-Epochs: 12
-Optimizer: Adam
-Loss function: Binary Crossentropy

Training and validation accuracy and loss are plotted for analysis.

## Evaluation
After training, the model is evaluated on the test dataset, and the test accuracy is printed.

## Prediction
A function predict_fire(img_path) is provided to predict whether a new image contains fire or not. The function loads the image, preprocesses it, and uses the trained model to make predictions.

## Example_Usage
```bash
predict_fire('/path/to/test/image.jpg')
```
