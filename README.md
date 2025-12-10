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

**🧹 1. Data Preprocessing**
**✔ Encoding the Target Column using Label Encoding**

The diagnosis column contains:

M → Malignant

B → Benign

These values were converted into:

M → 1

B → 0

This encoding is necessary because machine learning models require numerical targets.

**✔ Removing Unnecessary Columns**

Two columns were dropped:

id → does not contribute to prediction

Unnamed: 32 → an empty column with no values

Removing irrelevant features improves model accuracy and reduces noise.

**📏 2. Feature Scaling (Min-Max Normalization)**

Min-Max Normalization was applied to all feature columns except the target (diagnosis).
This transforms each feature into a range between 0 and 1, which ensures that:

All features contribute equally

Distance-based algorithms (KNN, K-Means) work correctly

The model avoids bias toward larger numerical values

**🔀 3. Splitting the Dataset**

The dataset was split into:

80% for training

20% for testing

This ensures that the model is trained on one portion of data and evaluated fairly on unseen data.

**🔵 4. K-Means Clustering (k = 2)**

K-Means clustering was applied to group the dataset into 2 clusters, since there are two classes:

Cluster 0

Cluster 1

This helps visualize and understand how benign and malignant samples naturally group based on their feature patterns — without using labels.

The cluster labels were added to both the training and testing sets.

**🟢 5. Training a KNN Classifier (k = 5)**

A K-Nearest Neighbors (KNN) model with k = 5 was trained on the structured data.

Why KNN?

Simple & effective

Works well on normalized data

Makes predictions based on similarity

The model predicts whether a tumor is benign or malignant.

**📊 6. Model Evaluation**

After prediction, the model was evaluated using:

✔ Accuracy

Percentage of correct predictions.

✔ Precision

How many predicted malignant cases were truly malignant.

✔ Recall

How well the model identifies actual malignant cases.

✔ F1-score

Balance between precision and recall.

These metrics help measure the overall performance and reliability of the classification model.
