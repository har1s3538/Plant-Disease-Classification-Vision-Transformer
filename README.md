# 🌱 Plant Disease Classification using Vision Transformer (ViT)

## 📌 Project Overview

Plant diseases significantly reduce agricultural productivity and pose a serious threat to global food security. Early and accurate detection of plant diseases can help farmers take timely preventive measures and minimize crop losses. This project addresses this challenge by applying **deep learning–based image classification** in the **agriculture domain**, with a focus on a **Vision Transformer (ViT) trained from scratch**.

A **Convolutional Neural Network (CNN)** is implemented as a baseline model, and its performance is compared with the Vision Transformer to evaluate the effectiveness of Transformer-based architectures for plant disease recognition.

---

## 🧠 Key Algorithm & Domain

* **Primary Algorithm:** Vision Transformer (Transformer-based model)
* **Baseline Algorithm:** Convolutional Neural Network (CNN)
* **Domain:** Agriculture
* **Task:** Multi-class plant disease classification
* **Number of Classes:** 38

✅ All models achieved accuracy **well above the 75% minimum requirement**.

---

## 🎯 Objectives

* Build an end-to-end plant disease classification system
* Implement a **Vision Transformer from scratch** (no pretrained weights)
* Establish a CNN baseline for comparison
* Perform rigorous training, validation, and testing
* Provide a working demo for real-time inference

---

## 📊 Dataset Description

* **Dataset Name:** PlantVillage Dataset
* **Source:** Kaggle
* **Total Images:** 54,305
* **Number of Classes:** 38
* **Image Type:** RGB images of healthy and diseased plant leaves

### 🔧 Preprocessing & Augmentation

* Images resized to **224 × 224**
* Dataset split into **training, validation, and test sets**
* Data augmentation applied only to the training set:

  * Random horizontal and vertical flips
  * Random rotations
  * Random zoom
* Image normalization performed within the model architectures

---

## ⚙️ Methodology

### 1️⃣ CNN Baseline (From Scratch)

A Convolutional Neural Network was designed from scratch using stacked convolutional, pooling, and dense layers. This model serves as a baseline to evaluate the relative performance of the Vision Transformer.

### 2️⃣ Vision Transformer (From Scratch)

The Vision Transformer model was implemented without pretrained weights and consists of:

* Patch embedding layer
* Positional encoding
* Multiple Transformer encoder blocks with multi-head self-attention
* Global average pooling layer
* Fully connected classification head

The ViT model was selected to assess the suitability of Transformer-based architectures for agricultural image classification tasks.

---

## 🧪 Experimental Setup

* **Train / Validation / Test Split:** Used to prevent data leakage
* **Loss Function:** Sparse Categorical Crossentropy
* **Optimizer:** Adam
* **Hardware:** Google Colab with NVIDIA T4 GPU
* **Framework:** TensorFlow & Keras

---

## 📈 Results & Evaluation

### ✅ Test Accuracy

* **CNN (from scratch): 91.40%**
* **Vision Transformer (from scratch): 94.83%**

The Vision Transformer consistently outperformed the CNN baseline, demonstrating superior generalization on the unseen test set.

### 📉 Visualizations

* Training and validation accuracy/loss curves for CNN and ViT
* Confusion matrices computed on the test set
* Model comparison bar chart

All visual results are stored in the `results/` directory.

---

## 🔍 Model Comparison

| Model                             | Training Accuracy | Validation Accuracy | Test Accuracy |
| --------------------------------- | ----------------- | ------------------- | ------------- |
| CNN (from scratch)                | ~87%              | ~94%                | **91.40%**    |
| Vision Transformer (from scratch) | ~96%              | ~95%                | **94.83%**    |

---

## 🎬 Demo

A working demo is provided inside the notebook:

* Inference on a dataset image to verify correct learning
* Inference on an external Google image to demonstrate real-world generalization and domain shift

This demo highlights both the strengths and limitations of the trained model.

---

## 💡 Discussion & Lessons Learned

* Vision Transformers can outperform CNNs even when trained from scratch
* Data augmentation significantly improves robustness and generalization
* Domain shift affects performance on real-world images
* Proper experiment tracking and version control are essential for reproducibility

---

## ⚠️ Limitations & Future Work

* Reduced robustness to complex real-world backgrounds
* Future improvements may include:

  * Training on real-field agricultural images
  * Applying leaf segmentation before classification
  * Deploying the model as a web or mobile application

---

## 🛠️ Installation & Usage

```bash
pip install -r requirements.txt
```

Run the notebook:

```bash
notebooks/Plant_Disease_Classification_ViT.ipynb
```

---

## 📁 Repository Structure

```
├── data/
├── notebooks/        # Model training, evaluation, and demo
├── results/          # Plots and confusion matrices
├── src/              # (Optional) helper modules
├── docs/             # Reports and presentation material
├── README.md
├── requirements.txt
```

---

## 📚 References

Relevant research articles (2024 onward) and detailed literature reviews are included in the **Short Project Report**.

---

## 🙏 Acknowledgments

* PlantVillage Dataset contributors
* Kaggle community
* TensorFlow & Keras open-source developers
