# Detecting At-Risk Students With Early Interventions

## Project Overview

This project leverages **machine learning** to identify students at risk of academic withdrawal or failure based on historical academic and demographic data. 
By detecting at-risk students early, educational institutions can initiate targeted interventions and significantly improve student retention and outcomes.

The system is designed with a **Python-based GUI** (built using `Tkinter`) to allow educators to:
- Upload and preprocess datasets.
- Train predictive models using various ML algorithms.
- Visualize performance metrics.
- Predict student withdrawal risks.

## Dataset

We use the **Open University Learning Analytics Dataset (OULAD)**. It contains:
- Course/module identifiers
- Assessment types and weights
- Demographic features (gender, region, age, disability)
- Student performance metrics

The raw data was spread across **7 CSV files**, which were merged and cleaned to produce a unified dataset of **173,912 records**. After preprocessing and dimensionality reduction, the final dataset had **156,520 rows and 10 features**.

## Methodology

### 1. Preprocessing
- **Label Encoding** of categorical variables
- **Missing Value Handling** (rows with nulls were dropped)
- **Dimensionality Reduction** using **Principal Component Analysis (PCA)**

### 2. Visualization
- **Matplotlib** and **Seaborn** used for:
  - Bar Graphs
  - Heatmaps
  - Correlation Matrices

### 3. Performance Metrics
- **Accuracy**
- **F1-Score**
- **AUC-ROC**
- **Sensitivity & Specificity**

### 4. Machine Learning Models
The following models were trained and evaluated:
-  **Random Forest** – Highest accuracy: **88.5%**
-  **Generalized Linear Model (GLM)** – Accuracy: **81.9%**
-  **Gradient Boosting Machine (GBM)** – Accuracy: **80.4%**
-  **Multilayer Perceptron (MLP)** – Accuracy: **79.6%**
-  **Feed Forward Neural Network (FFNN)** – Accuracy: **74.5%**

### 5. GUI
Developed using **Tkinter** to provide a user-friendly interface for:
- Dataset upload
- Preprocessing & PCA
- Model training
- Accuracy plotting
- Risk prediction

