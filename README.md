# Message Intelligence System

## Project Overview

The **Message Intelligence System** is a machine learning classification project designed to identify whether a digital message is **Spam** or **Legitimate**. The project applies probability-based, distance-based, and margin-based classification techniques to compare their effectiveness in spam detection.

### Objective

The objective of this project is to:

* Build a spam message classification system.
* Analyze message behavior and sender-related features.
* Compare multiple machine learning classifiers.
* Evaluate model performance using standard classification metrics.
* Understand the role of probability theory in classification.

### Target Classes

| Label | Class              |
| ----- | ------------------ |
| 0     | Legitimate Message |
| 1     | Spam Message       |

---

## Dataset Description

The dataset contains message-related and sender-related numerical features such as:

* Message Length
* Word Count
* Number of URLs
* Number of Digits
* Number of Special Characters
* Spam Keyword Score
* Legitimate Keyword Score
* Sender Activity Score
* Sender Account Age
* Messages Sent in Last 24 Hours
* Hour of Day
* Day of Week

Target Variable:

* `spam_label`

---

## Project Workflow

### Part A: Probability & Conceptual Foundation

* Conditional Probability
* Bayes' Theorem
* Naive Bayes Assumptions
* Working Principle of K-Nearest Neighbors (KNN)
* Comparison of Distance, Probability, and Margin-Based Classifiers

### Part B: Dataset Understanding & Preparation

* Data Loading
* Missing Value Handling using SimpleImputer
* Feature Selection
* Train-Test Split
* Feature Scaling using StandardScaler
* Class Imbalance Analysis

### Part C: K-Nearest Neighbors (KNN)

* Implement KNN Classifier
* Experiment with Different K Values
* Analyze Distance Metrics
* Identify Misclassified Messages
* Confusion Matrix Evaluation

### Part D: Support Vector Machine (SVM)

* Linear Kernel SVM
* RBF Kernel SVM
* Support Vector Analysis
* Performance Comparison with KNN

### Part E: Naive Bayes Classifier & Probability

* Gaussian Naive Bayes Implementation
* Manual Conditional Probability Calculation
* Bayes' Theorem Demonstration
* Comparison of Theoretical and Model Probabilities

### Part F: Model Comparison & Evaluation

Models Compared:

1. K-Nearest Neighbors (KNN)
2. Support Vector Machine (SVM)
3. Naive Bayes

Evaluation Metrics:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

### Part G: Final Analysis

* Strengths and Weaknesses of Each Model
* Trade-off Between Interpretability and Performance
* Real-World Deployment Recommendations

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Imbalanced-Learn (SMOTE)

---

## Data Preprocessing

The following preprocessing steps were performed:

* Missing value treatment using Median Imputation
* Removal of irrelevant features

  * message_id
  * message_text
  * timestamp
* Feature Scaling using StandardScaler
* Class Balancing using SMOTE

---

## Machine Learning Models

### K-Nearest Neighbors (KNN)

A distance-based classification algorithm that predicts class labels based on the majority vote of nearest neighbors.

### Support Vector Machine (SVM)

A margin-based classifier that separates classes using optimal decision boundaries.

### Gaussian Naive Bayes

A probability-based classifier that applies Bayes' Theorem under feature independence assumptions.

---

## Results

The models were evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

The best-performing model was selected based on overall classification performance and spam detection capability.

---

## Project Structure

```text
Message-Intelligence-System/
│
├── Message_Intelligence.csv
├── Part_B_EDA_Preprocessing.ipynb
├── Part_C_KNN.ipynb
├── Part_D_SVM.ipynb
├── Part_E_Naive_Bayes.ipynb
├── confusion_matrix_knn.png
├── confusion_matrix_svm.png
├── confusion_matrix_nb.png
├── model_comparison.png
├── README.md
└── requirements.txt
```

---

## Conclusion

This project demonstrates how machine learning algorithms can be applied to spam message detection. By comparing KNN, SVM, and Naive Bayes, the study highlights the advantages and limitations of different classification approaches while showcasing the importance of preprocessing, probability theory, and model evaluation in building intelligent message filtering systems.
