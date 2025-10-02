# Project Overview

## Step 1: Data Loading
- Reads a CSV file (data.csv) with 8,143 rows and 6 columns
- The data appears to be for a binary classification problem

## Step 2: Data Preparation  
- Separates features (X) from target variable (Y)
- Splits data into training (80%) and testing (20%) sets using train_test_split

## Step 3: Feature Scaling
- Uses StandardScaler to normalize the features
- Scales both training and test sets to improve model performance

## Step 4: Model Architecture
Creates a Sequential neural network with:
- Input layer: 5 neurons (takes 5 features)
- Hidden layer 1: 100 neurons with ReLU activation
- Hidden layer 2: 50 neurons with ReLU activation
- Hidden layer 3: 25 neurons with ReLU activation
- Output layer: 1 neuron with Sigmoid activation (binary classification)
- Total: 6,981 trainable parameters

## Step 5: Model Compilation
- Uses adam optimizer
- Uses binary_crossentropy loss function
- Tracks accuracy metric

## Step 6: Early Stopping
- Implements early stopping to prevent overfitting
- Monitors validation loss with patience of 10 epochs
- Restores best weights

## Step 7: Training
- Trains for up to 50 epochs with batch size of 25
- Uses 20% validation split
- Achieves 98.97% accuracy on training data

## Step 8: Visualization
- Plots training and validation accuracy/loss over epochs

## Step 9: Evaluation
- Evaluates model on training set showing excellent performance
