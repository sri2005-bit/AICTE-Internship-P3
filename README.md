# AICTE-Internship-P3
# E-Waste Classification using EfficientNet & TensorFlow

This project aims to automate the classification of electronic waste (e-waste) using a deep learning model based on EfficientNetV2. The model is trained on a custom image dataset and deployed with a Gradio web interface for real-time predictions.

---

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Setup Instructions](#setup-instructions)
- [Training Details](#training-details)
- [Evaluation](#evaluation)
- [Gradio App](#gradio-app)
- [Improvisations Done](#improvisations-done)
- [Results](#results)
- [Future Work](#future-work)
- [Author](#author)

---

## Project Overview

Manual sorting of e-waste is inefficient and prone to errors. This project uses deep learning to classify images of e-waste into predefined categories. The pipeline includes:
- Data preprocessing
- Transfer learning using EfficientNetV2B0
- Model evaluation and visualization
- A Gradio-powered interactive web app

---

## Dataset

- Custom dataset containing e-waste images organized in:
  - `train/` (Training set)
  - `val/` (Validation set)
  - `test/` (Testing set)
- Images are resized to 224x224 pixels
- Preprocessing includes normalization and batching

---

## Model Architecture

- Pretrained base: `EfficientNetV2B0`
- Layers added:
  - GlobalAveragePooling2D
  - Dense with ReLU
  - Output Dense layer with softmax activation
- Optimizer: `Adam`
- Loss Function: `categorical_crossentropy`
- Metrics: `accuracy`
- Callback: `EarlyStopping`

---

## Evaluation
-Training/Validation accuracy & loss plotted using matplotlib
-Confusion matrix and classification report
-Model saved for reuse using model.save()

---

## Improvisations Done
In this project, I developed an e-waste image classification model using deep learning. I organized and preprocessed the dataset, applied transfer learning with EfficientNetV2B0, and optimized training using early stopping and parameter tuning. I evaluated the model using accuracy metrics and visualized performance through plots. Additionally, I deployed the model using Gradio to create an interactive web interface for real-time predictions and compiled the entire workflow into a structured PowerPoint presentation.

---

## Results
-Successfully trained CNN model with EfficientNetV2
-Achieved good classification accuracy on unseen data
-Created a working Gradio demo for real-time testing

---


## Future Work
-Train on GPU to reduce training time
-Use larger, more diverse datasets
-Experiment with other model architectures (ResNet, MobileNet)
-Enhance the Gradio UI for usability

---


## Author
Srishti Jaiswal
B.Tech CSE Student
