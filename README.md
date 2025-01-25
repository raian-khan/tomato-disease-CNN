# Tomato Disease Classification Using CNN

## Overview
This project involves classifying tomato diseases using a Convolutional Neural Network (CNN). The dataset for this task was sourced from Kaggle and contains images of 256x256 pixels, categorized into 10 disease classes. The primary objective is to accurately classify images into one of these 10 classes.

## Dataset
- **Source**: Kaggle
- **Image Dimensions**: 256x256 pixels
- **Number of Classes**: 10 (representing 10 different tomato diseases)

## Preprocessing
Several preprocessing steps were applied to prepare the dataset for training:
1. **Resizing**: All images were resized to 256x256 pixels.
2. **Scaling**: Pixel values were scaled to the range [0, 1] for normalization.
3. **Data Augmentation**: Techniques like flipping and rotating the images were employed to increase dataset variability and prevent overfitting.

## Model Architecture
A custom CNN architecture was built for this task:
- **Convolutional Layers**: 6 convolutional layers to extract features.
- **Max Pooling Layers**: Added after each convolutional layer to reduce spatial dimensions and computational complexity.
- **Dense Layers**:
  - A fully connected layer with 64 units and ReLU activation.
  - A final dense layer with 10 units and softmax activation for 10-class classification.

## Training Details
- **Epochs**: 50
- **Data Split**:
  - 80% Training Data
  - 10% Validation Data
  - 10% Test Data
- **Metrics**: Training and validation accuracy and loss were calculated during training.

## Results
- **Training Accuracy**: 97%
- **Validation Accuracy**: 95%
- **Test Data Performance**: Predictions on the test set showed promising results, confirming the model’s ability to generalize well.

## Future Work
I plan to deploy this model on a web platform, allowing users to upload images of tomato leaves and receive predictions on potential diseases.


