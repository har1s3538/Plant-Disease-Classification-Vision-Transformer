# Plant Disease Classification Using Vision Transformers for Smart Agriculture

## Abstract
Plant diseases pose a significant threat to agricultural productivity and global food security. Traditional disease identification methods rely on manual inspection, which is time-consuming and requires expert knowledge. This project proposes an automated plant disease classification system using Vision Transformers (ViT) to accurately identify plant diseases from leaf images. The proposed approach aims to enable early disease detection and support sustainable agriculture practices.

## Introduction
Agriculture is a critical sector for global food supply, yet crop diseases continue to cause substantial yield losses each year. Early and accurate detection of plant diseases can help farmers take timely preventive actions. With recent advancements in deep learning, transformer-based architectures have demonstrated strong performance in computer vision tasks. This project explores the application of Vision Transformers for classifying plant diseases from leaf images and compares their performance with a conventional CNN baseline.

## Objectives
- Develop an automated plant disease classification system
- Implement a Vision Transformer (ViT) model for image classification
- Compare Vision Transformer performance with a CNN baseline
- Achieve classification accuracy above 75%
- Contribute to sustainable and precision agriculture

## SDG Alignment
**SDG-2: Zero Hunger**  
Early detection of plant diseases helps reduce crop losses and improves food production, supporting global food security.

## Dataset

This project uses the **PlantVillage dataset**, a publicly available and expertly curated dataset for plant disease classification.

- **Source:** Kaggle – PlantVillage Dataset  
- **Link:** https://www.kaggle.com/datasets/abdallahalidev/plantvillage-dataset  
- **Images:** ~54,000 RGB (color) images  
- **Crops:** Apple, Tomato, Potato, Grape, Corn, and others  
- **Classes:** Healthy and multiple disease categories  

The dataset also provides grayscale and segmented image variants; however, this project utilizes **only the color images** to preserve full RGB information, which is essential for Vision Transformer–based models.

Images are organized into class-wise folders, and labels are inferred directly from directory names.
