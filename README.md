# -DATA-MODELING-FOR-MEDICAL-DIAGNOSIS
Machine Learning-Based Data Modeling for Medical Diagnosis
Introduction
This project focuses on building machine learning models for medical diagnosis using heart disease and eye disease datasets. The primary goal is to classify diseases with high accuracy by applying various machine learning models such as:

Decision Tree
Naive Bayes
Support Vector Machine (SVM)
K-Nearest Neighbors (KNN)
Random Forest
The dataset was preprocessed, feature selection was performed using a correlation matrix, and models were evaluated with different train-test split ratios. The performance of each model is discussed in detail.

Google Colab Notebook Link :https://colab.research.google.com/drive/1w26kWgQBnx71QpfLtDJRUbhlehgw4ar5?usp=sharing

Data Preprocessing
Null Value Check:
Checked if the dataset contains any missing values.

Output:
TRUE: Missing values exist
FALSE: No missing values
Summary Statistics:
The summary statistics for various attributes like age, cholesterol, heart rate, etc., were computed to provide insights into the dataset. Metrics such as mean, median, standard deviation, and quartiles were calculated.

Data Visualization
Data exploration was carried out using various plots:

Bar Plot
Boxplot
Histogram
These visualizations helped in outlier detection and understanding data distribution.

Feature Selection
A correlation matrix was used to determine which attributes are highly correlated with each other. Features with a correlation threshold of >= 0.15 were selected for model building:

oldpeak
trestbps
thal
thalach
ca
fbs
chol
target
slope

Classification Models and Results
1. Decision Tree
Decision Trees are a powerful supervised learning method for classification. We tested the model with various train-test split ratios:

Split Ratio	Accuracy
80-20	1.00
70-30	0.99
60-40	0.95
50-50	0.94
Best Accuracy: 1.00 (80-20 Split)
2. Support Vector Machine (SVM)
SVM aims to find the optimal hyperplane for class separation in feature space.

Split Ratio	Accuracy
80-20	0.79
70-30	0.77
60-40	0.76
50-50	0.78
Best Accuracy: 0.79 (80-20 Split)
3. Naive Bayes
Naive Bayes classifiers utilize Bayes’ Theorem and assume independence among features.

Split Ratio	Accuracy
80-20	0.82
70-30	0.79
60-40	0.77
50-50	0.79
Best Accuracy: 0.82 (80-20 Split)
4. K-Nearest Neighbors (KNN)
KNN classifies data points based on the majority class of their nearest neighbors.

Split Ratio	Accuracy
80-20	0.92
70-30	0.89
60-40	0.87
50-50	0.85
Best Accuracy: 0.92 (80-20 Split)
5. Random Forest
Random Forest is an ensemble learning method that builds multiple decision trees and aggregates their results.

Split Ratio	Accuracy
80-20	1.00
70-30	0.99
60-40	0.99
50-50	0.97
Best Accuracy: 1.00 (80-20 Split)
K-Fold Cross Validation
To further validate the models, we employed 10-fold cross-validation, dividing the dataset into 10 equal parts. The models were trained and tested 10 times, with a different part being reserved for testing each time.

KNN: 0.97
SVM: 0.87
Decision Tree: 1.00
Naive Bayes: 0.79
Random Forest: 1.00
Conclusion
The project successfully applied multiple machine learning models to classify heart and eye disease datasets. The best performing models were:

Random Forest with an accuracy of 1.00 in both the 80-20 split and 10-fold cross-validation.
Decision Tree also achieved 1.00 accuracy with both the 80-20 split and 10-fold cross-validation.
These models can serve as a foundation for further medical diagnosis research and improvements.

Libraries Used
Python 3.x
Scikit-learn
Pandas
Numpy
Matplotlib
Seaborn
License
This project is licensed under the MIT License. See the LICENSE file for more details.
