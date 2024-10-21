# Multimodal Damage Identification

## Overview
The objective of this project is to develop a machine learning solution to identify and categorize disaster damage based on social media data. The project leverages both images and text (captions) related to disasters to automatically classify damage types and generate informative disaster reports.

## Audience
Relief organizations and emergency responders often face challenges in quickly assessing damage in disaster-affected areas. Our solution aims to streamline this process by providing an AI-powered tool to automatically classify disaster images and generate preliminary reports, helping these organizations respond more efficiently.

## Statistics
  - AI-driven damage assessment can reduce response time by up to 40%, allowing quicker deployment of relief efforts.
  - Machine learning models have been shown to increase accuracy in identifying damage categories, helping prioritize areas for immediate attention.
  - Combining both image and text data improves classification accuracy by up to 20% over using either modality alone.

## Pain Points
  1. Manual Damage Assessment: Relief organizations often rely on manual review of damage reports, which can be time-consuming and error-prone.
  2. Limited Use of Social Media Data: Although social media provides valuable real-time insights, it is often underutilized due to the lack of automated tools.
  3. Need for Real-Time Updates: Decision-makers need up-to-date, real-time information to allocate resources effectively.

## Dataset Structure
Our dataset consists of captioned social media images, which are categorized into six types of damage:
  - Damaged Infrastructure
  - Damaged Nature
  - Fires
  - Flood
  - Human Damage
  - Non Damage

## Research & Analysis
Our team conducted thorough analysis and preprocessing of the social media dataset, which included cleaning the text and resizing and normalizing the images. Key tools applied in this process include:

  - StandardScaler: Used to normalize numerical data for better performance in machine learning models.
  - Principal Component Analysis (PCA): Employed for dimensionality reduction, helping improve model performance by reducing noise and computational complexity.
  - Inertia (K-Means Clustering): Used to evaluate the compactness of clusters, helping to identify the optimal number of clusters for classifying the data.

## Machine Learning Models Applied
  1. Convolutional Neural Network (CNN) - ResNet50: Used for feature extraction from disaster-related images.
    - Purpose: To identify specific types of damage, such as infrastructural damage, fires, and floods.
  2. LSTM (Long Short-Term Memory): Used for text processing to analyze the captions associated with the images.
    - Purpose: To capture the sequential nature of textual data, enhancing the model’s ability to classify damage based on descriptions.
  3. GPT-2 Fine-Tuning: Employed for generating disaster reports based on input images and text.
    - Purpose: To automate the creation of detailed reports that describe the extent and type of damage detected in the data.

## Proposed Solutions & Results
Our solution aims to deliver:

  1. Automated Damage Classification: Relief organizations will have access to an AI tool that quickly classifies disaster images and generates comprehensive damage reports, allowing for faster and more informed decision-making.
  2. Improved Resource Allocation: By identifying high-priority areas based on the severity of damage, organizations can allocate resources where they are needed most, improving the efficiency of disaster response efforts.

With our solution, relief organizations will experience:
  - Increased efficiency: Automated systems will reduce the need for manual review, freeing up time and resources.
  - Accurate prioritization: Damage categories will be clearly defined, allowing for more targeted relief efforts.
  - Scalable deployment: Our AI-powered tool can handle large volumes of social media data, making it scalable for widespread disaster events.

## Model Performance
The models developed in this project have been evaluated using test sets to ensure accuracy and reliability:

  - CNN Model:
  - InceptionV3:
  - LSTM Model:
  - GPT-2 Model:

## Deployment
The project includes a web application built with Flask to allow users to upload disaster images and receive an automatically generated report:

  - Web App: Allows users to upload images, which are processed by the models to produce a damage report.
  - Heroku Deployment: The application is ready for deployment on Heroku, ensuring accessibility to relief organizations worldwide.

## Project Members

Rasha Alkhatib, Maryam Irfan, Kevin Jayne, Kyle Sellers, Ivan Vargas, and Donovan Watson.

## Sources

https://archive.ics.uci.edu/dataset/456/multimodal+damage+identification+for+humanitarian+computing
