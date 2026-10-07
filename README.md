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
## 🚀 How to Run This Project

You can run this pipeline either in your browser via Google Colab (recommended) or locally on your machine.

### Option 1: Run in Google Colab (Recommended & Instant)
1. Click the button below to open the notebook directly in Google Colab:
   [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/daksh3122/Transcriptomic-Disease-Classification/blob/main/YOUR_NOTEBOOK_NAME.ipynb) *(Replace with your actual Colab/GitHub notebook link)*
2. Run the cells sequentially to fetch the dataset, train the Random Forest model, and generate biomarker importance plots.

### Option 2: Run Locally via Terminal
If you prefer running it locally, clone the repository and install the dependencies:

```bash
# 1. Clone the repository
git clone [https://github.com/daksh3122/Transcriptomic-Disease-Classification.git](https://github.com/daksh3122/Transcriptomic-Disease-Classification.git)
cd Transcriptomic-Disease-Classification

# 2. Create and activate a virtual environment (recommended for Linux/macOS)
python3 -m venv venv
source venv/bin/activate

# 3. Install dependencies
pip install -r notebook/outputs/requirements.txt

# 4. Run the analysis notebook or script
