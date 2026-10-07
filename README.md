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
