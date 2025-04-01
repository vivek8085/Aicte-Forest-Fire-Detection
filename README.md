# Aicte-Forest-Fire-Detection
Building a CNN model for Forest Fire Detection
# Wildfire Detection using Deep Learning

This project aims to develop a deep learning model for detecting wildfires in images. It utilizes a Convolutional Neural Network (CNN) trained on a dataset of wildfire and non-wildfire images.

## Dataset

The project uses the "The Wildfire Dataset" available on Kaggle. It contains a diverse collection of images depicting both wildfire and non-wildfire scenarios.

## Model

The model is built using TensorFlow and Keras. It consists of several convolutional layers, max pooling layers, and fully connected layers. Data augmentation techniques are employed to improve model generalization and prevent overfitting. Transfer learning is explored with a pre-trained VGG16 model as a feature extractor. BatchNormalization is added to stabilize the training process.
