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
       - Created callbacks for ModelCheckpoint,EarlyStopping & Reduced learning rate
       - Final Train Accuracy = 63.11 , Validation Accuracy = 55.52
         ![image](https://github.com/user-attachments/assets/41ee1dfe-980c-4b4b-84a9-4f86f62388fe)
       - Issue- Overfitting, Low Accuracy
         ![image](https://github.com/user-attachments/assets/f7b406d5-1fcc-4580-98cb-b6aeb597ae0b)


   - **Same CNN model with Image Augmentation:**
        -  Train Accuracy = 57.64 , Validation Accuracy = 59.28
          ![image](https://github.com/user-attachments/assets/ed12b842-a067-4913-9d92-54000b834529)
        - Overfitting Resolved, Issue- Low Accuracy
          ![image](https://github.com/user-attachments/assets/3806d67c-f59b-44cf-881b-941a84e6981d)


   - **Transfer Learning VGGNET:** 
       - Inspired by the VGGNet model, with multiple convolutional layers followed by pooling, focusing on smaller filter sizes (3x3) and deeper networks.
       - Train Accuracy = 58.31 , Validation Accuracy = 56.48
         ![image](https://github.com/user-attachments/assets/a3b11698-5884-4f30-8c0e-9e155419ecc5)
         ![image](https://github.com/user-attachments/assets/c6e377f9-81ca-46f3-914a-267117bc1492)


   - **Transfer Leanring - ResNet50:** 
       - Incorporated class wieghts for imbalanced data and allow for better feature learning in deeper networks.
   
4. **Evaluation:**
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
