# 📘 ML Basic -- K-Means Clustering & KNN Classification

This project demonstrates a complete machine learning workflow using
breast cancer diagnostic data.\
It includes **data preprocessing**, **feature scaling**, **unsupervised
clustering**, and **supervised classification**, followed by performance
evaluation.

------------------------------------------------------------------------

## ⭐ Project Summary

The goal of this project is to classify breast cancer tumors as **Benign
(0)** or **Malignant (1)** using machine learning techniques.\
The workflow includes:

-   Data cleaning\
-   Label encoding\
-   Normalization\
-   Train/test splitting\
-   K-Means clustering\
-   K-Nearest Neighbors classification\
-   Model evaluation

------------------------------------------------------------------------

## 🧹 1. Data Preprocessing

### ✔ Encoding the Target Column

The `diagnosis` column contains: - **M → Malignant** - **B → Benign**

These values were converted into: - **M → 1** - **B → 0**

This encoding is necessary because machine learning models require
numerical targets.

------------------------------------------------------------------------

### ✔ Removing Unnecessary Columns

Two columns were dropped: - `id` → does not contribute to prediction\
- `Unnamed: 32` → an empty column with no values

------------------------------------------------------------------------

## 📏 2. Feature Scaling (Min-Max Normalization)

Min-Max Normalization was applied to all feature columns except the
target (`diagnosis`).\
This transforms each feature into a range between **0 and 1**, ensuring
fair contribution of all features.

------------------------------------------------------------------------

## 🔀 3. Splitting the Dataset

The dataset was split into:

-   **80% for training**
-   **20% for testing**

------------------------------------------------------------------------

## 🔵 4. K-Means Clustering (k = 2)

K-Means clustering was applied to group the dataset into **2 clusters**,
corresponding to benign and malignant types.\
Cluster labels were added to both training and test sets.

------------------------------------------------------------------------

## 🟢 5. Training a KNN Classifier (k = 5)

A **K-Nearest Neighbors (KNN)** classifier (k = 5) was trained to
predict tumor type based on feature similarity.

------------------------------------------------------------------------

## 📊 6. Model Evaluation

Evaluation metrics used:

-   **Accuracy**\
-   **Precision**\
-   **Recall**\
-   **F1-score**

------------------------------------------------------------------------

## 🗂️ Repository Structure

    ML_Basic/
    │── KNN_Kmeans.ipynb     # Main notebook
    │── README.md            # Project explanation
    └── Dataset.csv          # Dataset (optional)

------------------------------------------------------------------------

## 🎯 Conclusion

This project showcases: - Preprocessing\
- Normalization\
- Clustering (K-Means)\
- Classification (KNN)\
- Model evaluation

------------------------------------------------------------------------

## 📬 Contact

**Author:** Ahnaf
