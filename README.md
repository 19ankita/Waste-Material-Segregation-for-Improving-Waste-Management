# Waste-Material-Segregation-for-Improving-Waste-Management

Waste Segregation using Convolutional Neural Networks (CNNs)

An AI-powered automated waste material classification system designed to streamline waste segregation, improve recycling efficiency, and reduce environmental pollution. This repository contains a deep learning solution that classifies common waste materials into distinct categories using Convolutional Neural Networks (CNNs).

## Project Overview

Improper waste disposal contributes heavily to environmental degradation and inefficient recycling processes. Manual sorting is labor-intensive, error-prone, and costly. This project addresses these challenges by automating waste sorting using deep learning, providing an automated solution suitable for:
• Smart Recycling Bins
• Automated Waste Sorting Facilities
• Waste Monitoring and Reporting

## Dataset Overview

The dataset used in this project is publicly available on Kaggle and contains approximately 7,000 raw images distributed across seven categories:
• Cardboard
• Food Waste
• Glass
• Metal
• Paper
• Plastic
• Other
Images are organized into class-specific folders without further subcategorization (e.g., the Food_Waste folder contains various organic items like coffee grounds and fruit peels grouped together).

## Project Pipeline

The workflow is implemented sequentially within a Jupyter Notebook and covers the following core phases:

1. Data Preparation & Preprocessing

• Image Loading: Custom functions to dynamically parse directory structures, load images, and map their respective labels.
• Data Visualization: Distribution analysis of the dataset classes using bar plots alongside sample image visualizations.
• Image Resizing: Standardizing image dimensions based on dataset characteristics to prepare them for neural network ingestion.
• Class Encoding: Transforming categorical target labels into numerical formats suitable for training.
• Data Splitting: Dividing the processed dataset into distinct training and validation sets to ensure robust evaluation.

2. Model Building & Training

• Architecture Design: Implementation of a custom Convolutional Neural Network (CNN) configuration.
• Compilation: Optimizing the model using appropriate loss functions and optimization algorithms (e.g., Adam, Categorical Cross-Entropy).
• Training: Training the network for a minimum of 10 epochs while tracking performance indicators to prevent overfitting.

3. Model Testing & Evaluation

• Performance assessment on a dedicated test dataset using standard evaluation metrics:
	• Precision
	• Recall
	• F1-Score
	• Classification Accuracy

4. Data Augmentation (Optional)

• Pipeline integration using transformations (rotation, scaling, flipping) to artificially expand dataset variety and improve model generalization.


## Key Insights & Outcomes

• Detailed analysis of class balance/imbalance across the 7,000 images.
• Model evaluation graphs demonstrating training vs. validation loss and accuracy curves over the epochs.
• Final evaluation matrix showing the model's reliability in distinguishing between visually similar recyclables.
Note: This project was developed as part of an applied deep learning assignment (Assignment ID: CNN/01) focusing on AI solutions for sustainable environmental practices.
