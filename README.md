# Semantic Segmentation with MSI and SAR images

This project focuses on classifying satellite images using the Resnet50 model. The model has been trained to distinguish between various classes of satellite images, such as schools, airports, parks, and approximately 15 other categories.

## Model Training

### Training Parameters
The model is trained using the following parameters:

Number of epochs: 150 (Not necessary)
Learning rate scheduler: StepLR
### Training Loop
The training loop includes the following steps:

Load the EfficientNet-B0 model and configure the last layer to match the number of output classes.
Train the model using the training dataset and evaluate it on the test dataset at regular intervals.
Track the training loss and accuracy for each epoch.
Evaluate the model's performance on the test dataset and adjust training if accuracy decreases for consecutive epochs.

## Requirements

To run this project, you need the following Python libraries:

- torch
- torchvision
- tqdm
- matplotlib
- scikit-learn
- numpy
- random

