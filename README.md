# **PLANT LEAF DISEASE DETECTION**

## Project Overview

Agriculture is a key pillar of food security and economic growth, especially in developing countries where many people depend on farming for their livelihoods. However, crop diseases remain a major threat to productivity causing yield losses and food insecurity. This project focuses on detecting plant leaf diseases in corn, tomato and potato crops using image classification techniques. By automating disease detection, farmers can take timely action to prevent disease spread and reduce reliance on manual expert-based inspection.

## 1.0 Business Understanding
**Business Problem**

Crop diseases such as blight, leaf spots and rust severely reduce the productivity of corn, tomato and potato crops. Traditional detection methods depend on manual inspection, which is slow and often inaccurate. There is a need for an automated solution that can quickly and accurately identify diseases to help farmers take timely action and prevent crop losses.

**Main Busines Objective**

To develop an image classification model that can automatically detect and classify leaf diseases in corn, tomato and potato plants.

**Stakeholder Audience**
 - Farmers: Use the system to detect crop diseases early and improve yields.

 - Agricultural Extension Officers: Provide timely and accurate disease diagnosis support to farmers.

 - Agritech Companies: Integrate the model into smart farming solutions to enhance agricultural productivity.

 - Researchers: Analyze data and improve models for better understanding and management of crop diseases.

## 2.0 Data Understanding
The dataset used in this project comes from [Mendeley Data — “PlantVillage Dataset: Potato Leaf Disease”](https://data.mendeley.com/datasets/tywbtsjrjv/1). It contains labeled images of potato leaves under 10 categories

**Data Summary:**

 - Total images: 15848 original images.

 - Classes: 10

 - Format: JPEG

 - Resolution: Variable, to be resized to 224×224 for model training

 - Image collection: Captured under field and controlled lighting conditions

**Libraries Used**
1. Visualization: `matplotlib, seaborn`
2. Computation: `numpy`
3. File Handling: `os, hashlib, PIL`
4. Data & Model Libraries: `tensorflow, keras, MobileNetV2`
5. Evaluation: sklearn metrics (`classification_report, confusion_matrix, compute_class_weight`)

## 3.0 Data Preparation and Exploratory Data Analysis (EDA)
### Data Preparation
During the data preparation stage, several steps were performed to ensure the dataset was clean, balanced, and ready for training the deep learning model.

1. Removing Duplicates

Duplicate images were identified and removed using hash values to ensure that no identical samples appeared more than once in the dataset. This step helped prevent the model from being biased by repeated images.

2. Splitting the Data

The dataset was divided into three subsets:

            - 70% Training data for model learning

            - 15% Validation data for fine-tuning hyperparameters

            - 15% Testing data for final model evaluation


3. Dealing with Class Imbalance

Class weights were computed to balance the model’s learning process. This ensured that all classes contributed equally during training, preventing the model from favoring classes with more samples.

### Exploratory Data Analysis (EDA)

Exploratory Data Analysis was conducted to better understand the structure and composition of the dataset before model training.
1. Visual Inspection of Sample Images
A random selection of images from different classes was displayed to visually confirm the variety and quality of the data.
![leafs](Images\leafs.png)

2. Class Distribution Analysis
This visualization provided insights into class balance within the dataset, revealing that some classes had significantly more samples than others. 
![counts](Images\counts.png)

## Modeling

## Evaluation

## Deployment

## Conclusion