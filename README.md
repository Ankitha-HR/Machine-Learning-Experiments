
# Machine Learning Experiments

## Overview
This project implements and compares Machine Learning algorithms using three datasets for boosting, classification, and clustering.

## 1. Insurance Dataset — Boosting

**Dataset:** `insurance_pre.csv`

**Objective:** Predict medical insurance charges.

**Algorithms used:**
- AdaBoost Regressor
- Gradient Boosting Regressor
- Hist Gradient Boosting Regressor

### Results

| Algorithm | MAE | RMSE | R2 Score |
|---|---:|---:|---:|
| Gradient Boosting | 2428.89 | 4344.26 | 0.8784 |
| Hist Gradient Boosting | 2577.51 | 4607.72 | 0.8632 |
| AdaBoost | 4253.85 | 5181.86 | 0.8270 |

**Best Algorithm:** Gradient Boosting

## 2. Social Network Ads — Classification

**Dataset:** `Social_Network_Ads.csv`

**Objective:** Predict whether a user purchases a product based on age and estimated salary.

**Algorithms used:**
- Logistic Regression
- Decision Tree
- Random Forest
- Support Vector Machine (SVM)

### Results

| Algorithm | Accuracy | Precision | Recall | F1 Score |
|---|---:|---:|---:|---:|
| SVM | 0.9000 | 0.8387 | 0.8966 | 0.8667 |
| Random Forest | 0.9000 | 0.8387 | 0.8966 | 0.8667 |
| Decision Tree | 0.8625 | 0.7647 | 0.8966 | 0.8254 |
| Logistic Regression | 0.8375 | 0.8636 | 0.6552 | 0.7451 |

**Best Algorithms:** SVM and Random Forest (tie by F1 Score).

## 3. Mall Customers — Clustering

**Dataset:** `Mall_Customers.csv`

**Objective:** Group customers based on annual income and spending score.

**Algorithms used:**
- K-Means
- Agglomerative Clustering
- DBSCAN

### Results

| Algorithm | Clusters Found | Silhouette Score |
|---|---:|---:|
| K-Means | 5 | 0.555 |
| Agglomerative Clustering | 5 | 0.554 |
| DBSCAN | 2 | 0.388 |

**Best Algorithm:** K-Means

## Technologies Used
- Python
- Google Colab
- Pandas and NumPy
- Scikit-learn
- GitHub

## Evaluation Metrics
- **Boosting:** MAE, RMSE, R2 Score
- **Classification:** Accuracy, Precision, Recall, F1 Score
- **Clustering:** Silhouette Score and number of clusters

## Conclusion
The experiments compare different Machine Learning algorithms on three datasets.

Gradient Boosting achieved the highest R2 score among the tested boosting models. SVM and Random Forest achieved the highest F1 score among the tested classification models. K-Means achieved the highest Silhouette Score among the tested clustering models.

## Repository Contents
- `Experiment_1__Insurance_dataset_Boosting_.ipynb`
- `Experiment_2__Social_Network_Ads_Classification.ipynb`
- `Experiment_3_Mall_Customers_Clustering.ipynb`
- `insurance_pre.csv`
- `Social_Network_Ads.csv`
- `Mall_Customers.csv`
