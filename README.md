# Breast_Cancer_Diagnosis_Prediction
Problem Statement: The aim of this project is to classify breast cancer cases using K-Nearest Neighbors (KNN) and K-Means clustering.

Data Preprocessing: Preprocessing steps that were performed to prepare the data for modeling are:
1.	Diagnosis Encoding: The target variable diagnosis was converted into numerical form for model compatibility. Malignant tumors were encoded as 1 and benign tumors were encoded as 0.
2.	Removal of Irrelevant Columns: The ID column was removed as it does not contribute to prediction. The Unnamed: 32 column contained only null values and was therefore dropped to avoid unnecessary noise.
3.	Handling Missing Values: The dataset was checked for missing or null values after column removal. Rows or columns with missing data were removed to maintain dataset integrity.
4.	Feature Scaling (Min-Max Normalization): All feature columns (excluding the diagnosis label) were scaled using Min-Max Normalization. This transformation scales feature values into the range [0, 1] ensuring that no single feature dominates the distance-based algorithms. Feature scaling is especially important for KNN and K-Means as both algorithms rely on distance calculations.
5.	Train-Test Split: The dataset was split into 80% training data and 20% testing data. The training set was used for model learning, while the testing set was used for unbiased evaluation of model performance.

Algorithms that has been used are:
1.	K-Nearest Neighbors (classification): A supervised learning algorithm used for classification which predicts the class based on the majority class of the nearest neighbors.
2.	K-Means (clustering): An unsupervised learning algorithm which groups the data into two clusters to analyze natural separation between malignant and benign cases.
