# 🌿 Herbal Leaf Classification using ResNet-50 and Drones

This project integrates drone technology with deep learning to perform real-time classification of herbal plant leaves. Using a drone equipped with a high-resolution camera and a fine-tuned ResNet-50 model, the system classifies medicinal plants into 80 categories. Grad-CAM is employed to make the classification interpretable by highlighting important image regions.

---

## 🚀 Overview

- **Drone-based Image Capture**: UAVs are used to autonomously capture leaf images in natural environments.
- **Deep Learning Model**: A ResNet-50 model, fine-tuned on a dataset of 6,904 herbal leaf images.
- **Real-Time Classification**: Live webcam classification using OpenCV.
- **Interpretability**: Grad-CAM visualization highlights decision-making regions.
- **Application Areas**: Botanical research, agriculture, conservation, Ayurveda.

---

## 🖼️ Dataset

- **Source**: [Kaggle]
- **Classes**: 80 herbal leaf species
- **Total Images**: 6,904
- **Preprocessing**:
  - Petiole removal
  - Grayscale & binarization
  - Image sharpening, denoising
  - Feature extraction using GLCM (texture) and shape descriptors

---

## 🧠 Model

- **Architecture**: ResNet-50 (pretrained on ImageNet, fine-tuned)
- **Input Size**: 224 × 224 pixels
- **Loss Function**: Cross-Entropy
- **Optimizer**: Adam
- **Metrics**: Accuracy (~99%), validation with stratified 5-fold cross-validation
- **Visualization**: Grad-CAM

---

## 🛠️ Requirements

```bash
Python 3.7+
TensorFlow/Keras
OpenCV
NumPy
Drone SDK (for UAV communication)
