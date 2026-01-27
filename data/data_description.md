# Dataset Description

## Dataset Source
The dataset used in this project is the PlantVillage dataset obtained from Kaggle  
(https://www.kaggle.com/datasets/abdallahalidev/plantvillage-dataset).  
It is a widely used and expertly curated dataset for plant disease classification in agriculture.

## Dataset Overview
Plant diseases are a major threat to global food security. The PlantVillage dataset was created to support research in automated plant disease diagnosis using computer vision techniques. The dataset contains images of healthy and diseased plant leaves collected under controlled conditions.

## Number of Images
The dataset provides approximately 54,000 RGB (color) images of plant leaves.  
Grayscale and segmented variants are also available in the dataset; however, this project uses **only the color images**.

## Classes
The dataset includes multiple crop species such as apple, tomato, potato, grape, corn, and others. Each crop contains healthy leaf images as well as images representing different disease categories. Each class is stored in a separate directory.

## Dataset Structure
Images are organized in class-wise folders under the `color/` directory.  
Class labels are inferred directly from the folder names.

## Intended Usage
Only the `color/` subset of the dataset is used for training and evaluation, as it preserves full RGB information required for Vision Transformer–based image classification models.
