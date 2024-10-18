# Criminal Activity Detection - Chicago Crime Report

This repository contains code for detecting and classifying criminal activities using real crime data from Chicago. The project utilizes a neural network model to predict the type of crime based on various features extracted from the dataset.

## Dataset

The dataset used is **ChicagoCrime_10000.csv**, which includes 10,000 crime reports from the city of Chicago. Each record provides information about specific crime incidents, such as:
- Crime Type (target variable)
- Location details
- Date and time of occurrence
- Whether an arrest was made, etc.

## Project Overview

The main code is implemented in the Jupyter notebook file: **crime-detection-from-chicago-real-crime-reports.ipynb**, which walks through the following steps:

1. **Data Loading and Preprocessing**:
   - Load the CSV file and handle missing values.
   - Convert categorical features into numerical form using techniques like one-hot encoding.
  
2. **Feature Selection**:
   - Select relevant features from the dataset for training.
  
3. **Model Building**:
   - Construct a feed-forward neural network using PyTorch.
  
4. **Model Training**:
   - Train the model over 50 epochs, tracking loss and accuracy on the training data.

5. **Model Evaluation**:
   - Evaluate the model on the test set and report the accuracy (approximately 90.32%).

## Model Details

- **Architecture**:
  - Input Layer: Takes the processed crime features.
  - Hidden Layers: Fully connected layers with ReLU activation.
  - Output Layer: Predicts the crime category (multi-class classification).
  
- **Loss Function**: Cross-entropy loss for classification.
- **Optimizer**: Adam optimizer for efficient weight updates.

## Results

- The model achieves an accuracy of **90.32%** on the test data, indicating strong performance on unseen crime reports.

## How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/Criminal-activity-detection-Chicago-Crime-Report.git
