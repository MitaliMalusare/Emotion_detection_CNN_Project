# Emotion Detection from Scratch

## Overview
This project implements an image classifier from scratch to detect emotions in facial expressions using the Kaggle FER-2013 Dataset. The dataset consists of grayscale images (48x48 pixels) categorized into seven emotion classes: Angry, Disgust, Fear, Happy, Sad, Surprise, and Neutral.

## Dataset
- **Source:** [Kaggle FER-2013 Dataset](https://www.kaggle.com/datasets/msambare/fer2013)
- Each image is pre-processed to center the face and ensure consistent sizing.

## Methodology
1. **Data Preparation:** 
   - Downloaded and unzipped the dataset using Kaggle's API.
   - Performed exploratory data analysis (EDA) to understand the dataset distribution.
2. **Model Implementation:**
   - **Basic CNN:** 
       - A model with a few convolutional and pooling layers, primarily for baseline performance comparison.
     - **VGG-like Architecture:** 
       - Inspired by the VGGNet model, with multiple convolutional layers followed by pooling, focusing on smaller filter sizes (3x3) and deeper networks.
     - **Residual Networks (ResNet-like):** 
       - Incorporated skip connections to mitigate the vanishing gradient problem and allow for better feature learning in deeper networks.
     - **Custom CNN with Dropout and Batch Normalization:**
       - Added dropout layers to reduce overfitting and batch normalization to speed up convergence and stabilize training.
3. **Evaluation:**
   - Validated the model on test data.
   - Assessed performance using metrics like accuracy and confusion matrix.

## Key Features
- **Preprocessing:** Handled grayscale images for emotion recognition.
- **Model Training:** Designed and trained a convolutional neural network (CNN) for multi-class classification.
- **Results Visualization:** Displayed sample predictions and model evaluation metrics.

## Getting Started
### Requirements
- Python
- TensorFlow
- OpenCV
- Matplotlib
- Pandas
- NumPy
