# ML-Based Bearing Fault Diagnosis

An end-to-end machine learning project for classifying bearing faults from vibration data using the **Case Western Reserve University (CWRU) Bearing Dataset**.

The project explores vibration-signal preprocessing, exploratory data analysis, feature extraction, dimensionality reduction, and machine learning-based fault classification for mechanical condition monitoring.

## 🎯 Objective

The objective of this project is to develop a machine learning framework capable of identifying different bearing operating conditions from vibration signals.

Bearing faults generate characteristic changes in vibration behavior. By extracting meaningful features from these signals, machine learning models can be used for automated fault diagnosis and condition monitoring.

## ⚙️ Problem Statement

Unexpected bearing failures can lead to:

- Equipment downtime
- Production losses
- Increased maintenance costs
- Reduced equipment reliability

This project investigates whether vibration-based features can be used to automatically distinguish between different bearing fault conditions.

## 📊 Dataset

The project uses the **Case Western Reserve University (CWRU) Bearing Dataset**, a widely used benchmark dataset for bearing fault diagnosis.

The dataset contains vibration measurements collected under different operating and fault conditions.

### Fault Conditions

- Normal operating condition
- Inner race fault
- Outer race fault
- Ball fault

## 🔄 Project Workflow

CWRU Vibration Data  
↓  
Data Preprocessing  
↓  
Exploratory Data Analysis  
↓  
Feature Extraction  
↓  
Feature Scaling  
↓  
PCA Dimensionality Reduction  
↓  
ML Classification  
↓  
Cross-Validation  
↓  
Model Evaluation

## 🔬 Exploratory Data Analysis

Initial analysis is performed to understand the characteristics of the vibration signals.

The analysis includes:

- Signal visualization
- Feature distributions
- Statistical analysis
- Class distribution
- Correlation analysis
- Identification of relevant vibration characteristics

## 🛠️ Feature Engineering

Features are extracted from vibration signals to represent the mechanical behavior of the bearings.

### Time-Domain Features

- Mean
- Standard deviation
- Variance
- RMS
- Kurtosis
- Skewness
- Peak-to-peak value

### Frequency-Domain Analysis

Frequency-domain characteristics are investigated to identify patterns associated with different bearing fault conditions.

**FFT-based analysis** is used to examine the frequency characteristics of vibration signals.

## 📉 Dimensionality Reduction

**Principal Component Analysis (PCA)** is used to reduce feature dimensionality while retaining the most informative variance in the dataset.

PCA helps to:

- Reduce feature redundancy
- Visualize high-dimensional data
- Improve computational efficiency
- Identify dominant feature directions

## 🤖 Machine Learning Models

Multiple classification algorithms are investigated.

### Support Vector Machine (SVM)

Used to identify decision boundaries between different bearing fault classes.

### k-Nearest Neighbors (kNN)

Used as a distance-based classification baseline.

### XGBoost

Used as a gradient-boosting classifier to model relationships between engineered vibration features and bearing fault classes.

## 📏 Model Evaluation

The models are evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- Cross-validation

The evaluation focuses on overall classification performance and the ability to correctly identify individual fault classes.

## 🔍 Key Analysis

The project investigates:

1. Which vibration features are most informative for fault classification?
2. How effectively can ML models distinguish different bearing faults?
3. Does PCA improve classification performance?
4. How do SVM, kNN, and XGBoost compare?
5. How consistent are model results under cross-validation?

## 💻 Technologies Used

| Category | Tools / Technologies |
|---|---|
| Programming | Python |
| Data Processing | NumPy, Pandas |
| Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn, XGBoost |
| Dimensionality Reduction | PCA |
| Signal Analysis | FFT |
| Evaluation | Accuracy, Precision, Recall, F1-score |

## 📁 Project Structure

```text
ML-Based-Bearing-Fault-Diagnosis/
│
├── data/
│   └── CWRU/
│
├── notebooks/
│   └── bearing_fault_classification.ipynb
│
├── src/
│   ├── preprocessing.py
│   ├── feature_engineering.py
│   ├── models.py
│   └── evaluation.py
│
├── results/
│   ├── figures/
│   └── model_results.csv
│
├── requirements.txt
└── README.md
