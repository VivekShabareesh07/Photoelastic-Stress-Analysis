# Photoelastic Stress Classification

Deep learning project for classifying stress levels in photoelastic materials using pixel-level RGB intensity time-series.

---

## Overview
This project applies machine learning and deep learning techniques to classify stress regions in synthetic photoelastic data.  
Each pixel contains RGB intensity values recorded across **720 load steps** and is labeled into one of four stress categories:

- High stress  
- Medium stress  
- Low stress  
- Residual stress  

A 1D Convolutional Neural Network (CNN) is trained to learn temporal patterns in these signals and perform classification.

---

## Dataset
The dataset contains pixel-level signals extracted from synthetic photoelastic simulations.

**Data characteristics**
- 720 time steps per pixel
- 3 channels (Red, Green, Blue)
- 4 stress classes
- Train samples: 32,000 pixels  
- Test samples: 8,000 pixels  

Final model input shape: (720, 3)


---

## Project Pipeline
1. Data preprocessing and cleaning  
2. Exploratory data analysis (EDA)  
3. Baseline model (Logistic Regression)  
4. Time-series deep learning using 1D CNN  
5. Evaluation on unseen test data  

---

## Models & Results

| Model | Accuracy |
|------|----------|
| Logistic Regression (baseline) | ~95% |
| 1D CNN (final model) | ~98% |

The CNN significantly improves performance by learning temporal and cross-channel signal patterns.

---

## Technologies Used
- Python
- NumPy & Pandas
- Scikit-learn
- TensorFlow / Keras
- Matplotlib



