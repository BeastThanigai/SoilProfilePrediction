# 🌱 Soil Profile Analysis System  
### Soil Type & Density Detection using Machine Learning (TFLite + Streamlit)

## 📌 Project Overview

This project implements an **intelligent soil profile analysis system** that automatically:
- Verifies whether an uploaded image is a valid soil profile
- Segments the soil profile into multiple horizontal layers
- Predicts the **soil type** and **soil density** for each detected layer
- Merges similar adjacent layers for better geological interpretation

The system is built as an **interactive Streamlit web application** and uses **TensorFlow Lite (TFLite)** models for efficient inference.

---

## 🎯 Objectives

- Automate soil profile interpretation from images  
- Detect and segment soil layers based on intensity variations  
- Classify soil types using trained ML models  
- Estimate soil density numerically  
- Provide a visual and user-friendly soil analysis tool  

---

## 🧠 Key Concepts Used

- Image preprocessing and enhancement  
- Gamma correction for visual normalization  
- Gradient-based image segmentation  
- Machine Learning inference using TFLite  
- Streamlit-based UI for interactive analysis  

---

## ⚙️ Features

- ✅ Soil image validation (filters non-soil images)
- ✅ Automatic soil layer segmentation
- ✅ Soil type classification per layer
- ✅ Soil density prediction per layer
- ✅ Layer merging based on similarity
- ✅ Visual display of segmented layers
- ✅ Lightweight inference using TFLite models

---

## 🧪 Soil Types Supported

The system currently classifies soil into the following categories:
- Alluvial soil  
- Black soil  
- Clay soil  
- Red soil  

---


---

## 🔄 System Workflow

1. User uploads a soil profile image  
2. Image is validated using a soil-check model  
3. Image is segmented into horizontal soil layers  
4. Each segment undergoes:
   - Gamma correction
   - Soil type prediction
   - Soil density estimation  
5. Similar adjacent layers are merged  
6. Final results are visualized and displayed  

---

## 🖼️ Image Segmentation Approach

- Converts image to grayscale  
- Divides image vertically into slices  
- Computes mean intensity per slice  
- Applies Gaussian smoothing  
- Uses gradient peaks to detect layer boundaries  
- Filters boundaries using minimum gap constraints  

This approach mimics **real soil stratification patterns**.

---

## 🛠️ Technologies Used

| Component | Technology |
|--------|------------|
| Frontend | Streamlit |
| Backend | Python |
| ML Inference | TensorFlow Lite |
| Image Processing | OpenCV, PIL |
| Numerical Ops | NumPy |
| Smoothing | SciPy |

---


