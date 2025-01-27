# Real-Time Road Accident Detection System

This repository contains the implementation of a **real-time road accident detection system** using surveillance cameras. The system is based on four different models: **YOLO, CNN**, and two hybrid approaches (**YOLO-XGBoost** and **CNN-XGBoost**). The project aims to enhance road safety by automating accident detection and severity classification.


## 📋 Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Models](#models)
- [Results](#results)
- [Installation and Usage](#installation-and-usage)
- [Contributors](#contributors)
- [Refrences](#Refrences)


## 🛠️ Introduction

Road accidents are a critical global issue, causing fatalities and long-term injuries. Delayed emergency response times exacerbate the problem. This project use **deep learning** and **hybrid techniques** to detect accidents in real-time using images captured by surveillance cameras.


## 📊 Dataset

The dataset has acquisition from kaggle [1] and is divided into 4 classes:
1. **Accident Scenarios**:
   - Minor Impact
   - Substantial Impact
   - Critical Impact
2. **Non-Accident Scenarios**

### Preprocessing Steps:
- **Resizing**: Images resized to 320x320 pixels.
- **Augmentation**: Techniques include flipping, cropping, brightness adjustment, and noise addition.
- **Balancing**: Class distribution was balanced using data augmentation to prevent bias.



## 🤖 Models

### 1. YOLO
- **Description**: State-of-the-art detection model optimized for real-time performance.

### 2. CNN
- **Description**: Focused on feature extraction and classification for accident detection.

### 3. YOLO-XGBoost
- **Description**: Combines YOLO’s feature extraction with XGBoost for improved classification performance.

### 4. CNN-XGBoost
- **Description**: Combines CNN’s feature extraction with XGBoost for improved classification performance.



## 📈 Results

| **Model**         | **Accuracy (%)** | **Train Loss**  | **Validate Loss** |
|--------------------|------------------|---------------|------------------|
| YOLO              | 95.73           | 0.02164      | 0.78611         |
| CNN               | 92              | 0.066        | 0.266           |
| YOLO-XGBoost      | 92.36           | 0.0260       | 0.2624          |
| CNN-XGBoost       | 94.13           | 0.0133       | 0.1762          |

**Detailed metrics**, including confusion matrices and performance charts, are available in the `results/` folder.


## 👥 Contributors
- Aljohara Abdulhakeem Bin Dokhi
- Amal Misfer Alqahtani
- Amwaj Mohammed Alzahrani
- Fai Abdulaziz Bin Onayq
Supervisor: Dr. Manal Khaled Alsabhan

## Refrences
[1] Prithvi Ragavendiran R and Surya Prabhakaran, “Road Accidents from CCTV Footages Dataset,” https://www.kaggle.com/dsv/7518784.
