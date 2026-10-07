# Transcriptomic-Disease-Classification
# Translational Biomarker Discovery & Disease Classification Pipeline

## Overview
An end-to-end machine learning pipeline built to classify leukemia cancer subtypes (ALL vs. AML) using high-throughput gene expression profiling. Beyond predictive accuracy, this pipeline identifies and ranks key molecular biomarker genes driving the classification.

## Dataset
- **Source:** Golub Leukemia Benchmark Dataset via scikit-learn (`fetch_openml`).
- **Dimensions:** 7,129 gene expression features across 72 patient samples.

## Methodology
1. **Preprocessing & Splitting:** Performed stratified train-test splitting (80/20) to maintain class balance across high-dimensional transcriptomic spaces.
2. **Modeling:** Trained an ensemble Random Forest classifier to handle non-linear biological interactions.
3. **Evaluation:** Achieved a **93.3% Accuracy** and a **0.98 ROC-AUC Score** on unseen test data.
4. **Biomarker Extraction:** Isolated top predictive genes (`M84526_at`, `D88422_at`, etc.) using Gini feature importance metrics for downstream pathway analysis.

## Key Results
- **ROC-AUC:** 0.9800
- **Top Biomarkers:** Identified primary transcriptomic drivers distinguishing Acute Lymphoblastic Leukemia from Acute Myeloid Leukemia.

#### How to Run This Project

You can run this pipeline either in your browser via Google Colab (recommended) or locally on your machine.

### Option 1: Run in Google Colab (Recommended & Instant)
Click the badge below to open and run the notebook instantly in your browser:
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/daksh3122/Transcriptomic-Disease-Classification/blob/main/YOUR_EXACT_FILENAME.ipynb)

### Option 2: Run Locally
1. Clone the repository:
   ```bash
   git clone [https://github.com/daksh3122/Transcriptomic-Disease-Classification.git](https://github.com/daksh3122/Transcriptomic-Disease-Classification.git)
   cd Transcriptomic-Disease-Classification
   
