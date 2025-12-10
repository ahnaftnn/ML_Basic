"# ML Basic"

**KNN_Kmeans.ipynb**
This project applies Machine Learning classification and clustering techniques on a breast cancer dataset.
The workflow includes preprocessing, encoding, normalization, clustering using K-Means, and classification using K-Nearest Neighbors (KNN).

**📌 Project Overview**

This notebook performs the following machine learning tasks:

1. Load and inspect dataset

2. Encode target labels (diagnosis column)

3. Drop unnecessary columns

4. Apply Min-Max Normalization

5. Split dataset into training and test sets

6. Apply K-Means clustering (k = 2)

7. Train a KNN Classifier (k = 5)

8. Evaluate model performance

     -Accuracy

     -Precision

     -Recall

     -F1-score

**📂 Dataset**

The dataset contains breast cancer diagnostic data, including features such as radius, texture, smoothness, compactness, etc.

 **Target Column**

   diagnosis:

    M → 1 (Malignant)

    B → 0 (Benign)

   Dropped Columns:

     id

     Unnamed: 32
