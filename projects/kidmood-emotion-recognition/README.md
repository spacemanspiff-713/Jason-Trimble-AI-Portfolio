# KidMood: Classroom Emotion Recognition

**Course:** ITAI 1378 — Computer Vision and Artificial Intelligence  
**Project Type:** Final Capstone Project  
**Author:** Jason Trimble  
**Tier:** Transfer Learning (MobileNetV2)

---

## Overview

KidMood is a computer vision system that classifies facial expressions into four emotion categories — **Happy, Sad, Angry, Fear** — using the FER-2013 dataset and MobileNetV2 transfer learning with TensorFlow/Keras.

## Problem

Teachers and childcare workers cannot continuously monitor every student's emotional state during busy activities. Early signs of sadness, fear, or anger can be missed, delaying adult support. KidMood is designed as an assistive awareness signal, not a diagnostic tool.

## What I Built

- **Data pipeline:** FER-2013 loading, label filtering (4 classes), pixel parsing, normalization, 224×224 resizing, grayscale-to-RGB conversion, stratified train/val/test split
- **Model architecture:** MobileNetV2 transfer learning with custom classification head (GlobalAveragePooling → Dense(128) → Dropout(0.5) → Softmax(4))
- **Baseline model:** Simple CNN for comparison
- **Training pipeline:** Configurable epochs, batch size, learning rate, with checkpointing
- **Evaluation:** Accuracy, macro F1-score, confusion matrix, per-class metrics
- **Inference:** Single-image prediction with confidence scores
- **Documentation:** Full README, AI usage log, presentation materials, demo video script

## Tools & Concepts

| Category | Details |
|----------|---------|
| **Framework** | TensorFlow / Keras |
| **Model** | MobileNetV2 (transfer learning), baseline CNN |
| **Data** | FER-2013 facial expression dataset |
| **Libraries** | NumPy, pandas, matplotlib, scikit-learn, OpenCV |
| **Concepts** | Image classification, transfer learning, data augmentation, model evaluation |
| **Workflow** | Jupyter notebooks, Python scripts, Git version control |

## Repository

The full project with source code, notebooks, trained models, and results is maintained in its own repository:

**[github.com/spacemanspiff-713/KidMood-Final-Project](https://github.com/spacemanspiff-713/KidMood-Final-Project)**

---

[← Back to Portfolio](../../README.md)