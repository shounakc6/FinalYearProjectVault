# Master Thesis Submission

Name: Priya T  
Roll No: 224CS2001  
Project: A novel Convolutional Tsetlin Architecture for classification of Satellite images under limited supervision


# Master Thesis Submission – Priya T

## Overview

This repository contains the complete implementation, documentation, and results of my Master’s thesis on satellite image classification using interpretable machine learning.

The work addresses key challenges in remote sensing:

- Limited availability of labeled data  
- High-dimensional and noisy satellite imagery (especially SAR)  
- Lack of interpretability in deep learning models  

To overcome these challenges, a hybrid CNN–Tsetlin Machine (CNN–TM) framework is proposed, combining deep learning for feature extraction with rule-based learning for interpretability.

---

## Key Contributions

- Novel CNN–Tsetlin Machine hybrid architecture  
- Multi-scale CNN for spatial feature extraction  
- Structured binary feature encoding for interpretability  
- Rule-based classification using Tsetlin Machine  
- Intrinsic explainability (not post-hoc)  
- High accuracy under limited supervision (low-data setting)  
- Cross-dataset evaluation across multiple satellite modalities  

---

## Methodology

The proposed framework consists of three main stages:

### 1. Feature Extraction (CNN)
- Multi-scale convolutional layers (3×3, 5×5, 7×7)  
- Captures fine-to-coarse spatial patterns  
- Produces high-dimensional feature maps  

### 2. Structured Binary Encoding
- Converts CNN features into Boolean representations  
- Uses patch-based statistics:
  - Relative intensity  
  - Texture variation  
  - Coefficient of variation  

### 3. Classification (Tsetlin Machine)
- Learns logical clauses over binary features  
- Produces interpretable decisions  
- Enables clause-based reasoning and attribution  

---

## Results Summary

- Achieved 98.39% accuracy on the MSTAR-10 dataset under limited data conditions  
- Outperformed multiple deep learning baselines  
- Demonstrated strong generalization across:
  - SAR datasets  
  - Multispectral datasets  
  - Hyperspectral datasets  

---

## Repository Structure



Priya_T_224CS2001/
│
├── Thesis/
│ ├── 224CS2001_Priya_complete_Thesis.pdf
│ └── thesis_paper_version.pdf
│
├── PPT/
│ └── presentation.pptx
│
├── Paper/
│ ├── paper.pdf
│ └── paper.zip
│
├── Code/
│ ├── CNNModel.ipynb
│ ├── ConvTM_SAR_Base_Paper.ipynb
│ ├── ProposedModel_Optuna.ipynb
│ ├── ProposedModel_differentdatasets.ipynb
│ ├── CTM_5G_Jamming_Detection.ipynb
│ └── ablation_feature.ipynb
│
├── Figures/
│ ├── architecture diagrams (.drawio)
│ ├── heatmaps
│ ├── confusion matrices
│ ├── comparison plots
│ └── other result visualizations
│
└── README.md



---

## Code Description

The `Code/` directory contains Jupyter notebooks for:

- CNN-based feature extraction  
- Tsetlin Machine implementation  
- Hybrid CNN–TM framework  
- Hyperparameter optimization using Optuna  
- Ablation studies  
- Dataset-specific experiments  

---

## Figures

The `Figures/` directory includes:

- Model architecture diagrams  
- Binary encoding visualizations  
- Heatmaps and interpretability outputs  
- Performance comparison plots  
- Confusion matrices  

---

## Paper and Thesis

- Full thesis document  
- Research paper version  
- Supporting submission materials  

---

## Technologies Used

- Python  
- PyTorch  
- NumPy  
- Pandas  
- Scikit-learn  
- PyTsetlinMachine  
- Optuna  

---

## Key Advantages

- Combines accuracy with interpretability  
- Effective under limited labeled data conditions  
- Provides rule-based explanations  
- Applicable across multiple satellite modalities  
- Avoids black-box decision-making  

---
