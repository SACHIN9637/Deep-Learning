# Alzheimer's Disease Classification using ResNet50

## 📌 Project Overview
This project implements **Alzheimer's Disease Classification** using a **pre-trained ResNet50 model**. The dataset used is [Best Alzheimer MRI Dataset (99% Accuracy)](https://www.kaggle.com/datasets/lukechugh/best-alzheimer-mri-dataset-99-accuracy).

---

## 🚀 Workflow Breakdown

### **Task 1: Dataset Preparation**
- **Dataset:** Kaggle - Best Alzheimer MRI Dataset
- **Preprocessing:**
  - Resizing images to **224x224** (ResNet50 input size)
  - Data Augmentation: **Rotation, Flipping, Zooming**
  - Splitting data into **Train (70%) / Validation (15%) / Test (15%)**

### **Task 2: Model Implementation & Fine-Tuning**
- **Pre-trained Model:** ResNet50 (ImageNet weights)
- **Modifications:**
  - **Froze initial 140 layers**, fine-tuned top layers
  - Added `Flatten → Dense (256) → Dropout (0.5) → Softmax`
- **Hyperparameter Optimization:**
  - **Learning Rate:** `0.0001`
  - **Optimizer:** `Adam`
  - **Epochs:** `10`
- **Feature Map Visualization** for early convolutional layers
- **Saved Model:** `alzheimers_resnet50_finetuned.h5`

### **Task 3: Model Evaluation & Performance Comparison**
- **Metrics Computed:**
  - **Accuracy, Precision, Recall, F1-score, Confusion Matrix**
- **Visualizations:**
  - Accuracy & Loss trends over epochs
  - Confusion Matrix heatmap
- **Comparison with Research Paper:**
  - **Achieved Accuracy:** `XX%` (Replace with actual result)
  - **Paper Reported Accuracy:** `99%`
- **Potential Improvements:**
  - Fine-tune more layers
  - Experiment with different optimizers
  - Increase dataset augmentation for robustness

---


## 📜 References
- **Dataset:** [Kaggle Alzheimer’s MRI Dataset](https://www.kaggle.com/datasets/lukechugh/best-alzheimer-mri-dataset-99-accuracy)
- **Research Paper:** Alzheimer’s Disease Prediction using Deep Learning



