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
   - Built a deep learning model using TensorFlow/Keras.
   - Experimented with various CNN architectures for optimized performance.
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

### Setup
1. Clone the repository and install dependencies:
   ```bash
   git clone <repository_url>
   cd <repository_directory>
   pip install -r requirements.txt
