# 🌿 Herbal Leaf Classification using ResNet-50 and Autonomous Drones

This project presents an integrated system combining Unmanned Aerial Vehicles (UAVs) and deep learning for the real-time classification of herbal leaves. By leveraging a drone-mounted camera and a fine-tuned ResNet-50 model, this solution enables high-accuracy identification of medicinal plants in natural environments. The system supports research in botany, agriculture, traditional medicine, and ecological conservation.

---

## 📌 Key Features

- **Autonomous Drone-Based Image Capture**  
  Multi-rotor UAVs are used to capture high-resolution images of leaves from remote terrains.

- **Deep Learning Model (ResNet-50)**  
  A transfer learning-based ResNet-50 model trained on a curated dataset of 6,904 leaf images across 80 medicinal plant classes.

- **Real-Time Classification**  
  Live classification using webcam or drone feed, optimized for fast and accurate inference.

- **Model Interpretability**  
  Integrated Grad-CAM for visualizing the key regions of leaf images that influence classification decisions.

- **Domain Applications**  
  Useful in plant biodiversity surveys, environmental monitoring, Ayurvedic and pharmaceutical research, and smart agriculture.

---

## 🧠 Technical Overview

- **Architecture**: ResNet-50 (pre-trained on ImageNet, fine-tuned for 80 herbal leaf classes)  
- **Input Size**: 224 × 224 pixels  
- **Loss Function**: Cross-Entropy  
- **Optimizer**: Adam  
- **Validation Strategy**: 5-fold Stratified Cross-Validation  
- **Interpretability**: Gradient-weighted Class Activation Mapping (Grad-CAM)  
- **Accuracy Achieved**: ~99% on validation set  

---

## 🗂 Dataset

- **Source**: [Kaggle – Indian Medicinal Leaf Dataset](https://www.kaggle.com/)  
- **Total Images**: 6,904  
- **Classes**: 80 unique herbal plant species  
- **Format**: JPG, 224x224 pixels  
- **Preprocessing Includes**:
  - Petiole removal
  - Denoising and sharpening
  - Grayscale conversion & binarization
  - Edge extraction
  - Feature extraction using GLCM (contrast, energy, correlation, homogeneity)

---

## ⚙️ Installation & Setup

### 🔧 Prerequisites

- Python 3.7 or above  
- GPU-supported machine (for training)   
- Webcam or onboard drone camera  



```bash
pip install -r requirements.txt
