# 🚀 Mars Landmark Classifier  

## 📚 Table of Contents
1. [Project Overview](#project-overview)  
2. [Key Features](#key-features)  
3. [System Architecture](#system-architecture)  
4. [Technologies Used](#technologies-used)  
5. [How to Use](#how-to-use)  
6. [Results](#results)  
7. [Acknowledgments](#acknowledgments)  

---

## 🌍 Project Overview  
The **Mars Landmark Classifier** is a deep learning-based system designed to optimize data transmission between Mars rovers and mission control by implementing an image compression pipeline combined with a classification model. This system ensures efficient communication while preserving crucial scientific data, enabling researchers to identify Mars landmarks with high accuracy.  

---

## ✨ Key Features  
- **CNN AutoEncoder for Compression**  
  - Compresses 224x224 resolution images by **99%**, reducing image size to 500-length latent vectors while preserving image quality.  
- **Mars Landmark Classification**  
  - Achieved **84.26% classification accuracy** on landmarks using decoded feature vectors.  
- **Data Augmentation**  
  - Addressed class imbalance by generating **2000 synthetic images**, improving robustness and generalization of the classifier.  

---

## 🏗️ System Architecture  

```plaintext
Raw Mars Images
       ↓
  Image Compression (CNN AutoEncoder)
       ↓
Compressed Latent Vectors (500-D)
       ↓
  Decoded Images
       ↓
Mars Landmark Classification (CNN Classifier)
