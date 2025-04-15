# 🔥 Fire Detection Using Deep Learning

This project implements a fire detection system using deep learning techniques and OpenCV. It aims to automatically detect fire in real-time from video streams or image inputs using a trained model, making it suitable for smart surveillance systems or safety mechanisms.

---

## 📁 Project Structure

Fire_Detection/ ├── Fire_Detection.ipynb # Jupyter notebook with all code ├── model/ # Directory to save trained model (if exported) ├── data/ # Directory for storing training and testing images ├── images/ # Sample input images ├── outputs/ # Outputs like prediction results or annotated images └── README.md

---

## 🚀 Features

- 🔍 Real-time fire detection using OpenCV
- 🧠 Deep learning model for image classification
- 📷 Works with video streams or image files
- 📊 Performance metrics and visualizations included
- 💾 Option to save trained model

---

## 📦 Requirements

Install dependencies using pip:

```bash
pip install -r requirements.txt
if requirements.txt is not available, install manually:
pip install opencv-python numpy matplotlib tensorflow keras

🧠 Model Overview
The model is a Convolutional Neural Network (CNN) trained on a dataset of fire and non-fire images. It classifies input frames/images as either "FIRE" or "NO FIRE".

Architecture
-Input Layer (resized image)

-Convolution + ReLU layers

-Max Pooling

-Fully Connected (Dense) Layers

-Output (Softmax or Sigmoid depending on implementation)

