# -DATA-MODELING-FOR-MEDICAL-DIAGNOSIS
A Machine Learning Based Data Modeling for Medical Diagnosis
Introduction
This project implements machine learning models for the diagnosis of Heart Disease and Eye Disease using various classification techniques. The goal is to predict medical outcomes by leveraging classification algorithms like:

Decision Tree
Naive Bayes
Support Vector Machine (SVM)
K-Nearest Neighbors (KNN)
Random Forest
The dataset is preprocessed with feature selection based on a correlation matrix, and the models are applied with different splits of testing and training data. The accuracy of each model is evaluated and compared.

🔗 Colab Notebook: Access the code

Dataset Information
The dataset used for diagnosis includes various medical parameters like age, cholesterol levels, blood pressure, etc. The data undergoes preprocessing to check for missing values and outliers.

Dataset Summary: The dataset contains 1,025 instances with 14 features.
Missing Values: None detected.
Summary Statistics:
Statistic	Age	Chol	BP	etc.
Mean	54.43	246.0	131.6	...
Std Dev	9.07	51.59	17.51	...
Min	29	126	94	...
Max	77	564	200	...
Data Visualization
To understand the dataset better and identify outliers, the following visualizations were used:

Bar Plots
Box Plots
Histograms
A Correlation Matrix was calculated to select features based on their correlation with the target variable. Features with a correlation coefficient ≥ 0.15 were selected.

Model Descriptions
1. Decision Tree Classifier
Decision Tree builds a tree-like structure to classify data. The model was trained with different train-test splits, and the highest accuracy was observed for the 80-20 split:

80-20: 1.00
70-30: 0.99
60-40: 0.95
50-50: 0.94
2. Support Vector Machine (SVM)
SVM aims to create a hyperplane that separates the data points into different classes. The highest accuracy:

80-20: 0.79
70-30: 0.77
60-40: 0.76
50-50: 0.78
3. Naive Bayes Classifier
Naive Bayes calculates class probabilities based on Bayes' theorem. The highest accuracy:

80-20: 0.82
70-30: 0.79
60-40: 0.77
50-50: 0.79
4. K-Nearest Neighbors (KNN)
KNN classifies a point based on the labels of its nearest neighbors. The highest accuracy:

80-20: 0.92
70-30: 0.89
60-40: 0.87
50-50: 0.85
5. Random Forest Classifier
Random Forest is an ensemble learning method using multiple decision trees. The highest accuracy:

80-20: 1.00
70-30: 0.99
60-40: 0.99
50-50: 0.97
K-Fold Cross Validation
K-fold cross-validation was applied with 10 folds. The following accuracies were achieved:

Model	Accuracy
Decision Tree	1.00
Random Forest	1.00
KNN	0.97
SVM	0.87
Naive Bayes	0.79
Conclusion
The Random Forest and Decision Tree models achieved the highest accuracy of 1.00 with both the 80-20 split and 10-fold cross-validation.
Other models like KNN and SVM also performed well but didn't reach perfect accuracy.
How to Run the Code
Clone this repository:

bash
Copy code
git clone https://github.com/ABI0508/medical-diagnosis-ml.git
Open the Jupyter notebook or Colab notebook from the link above.

Run the code to see the models in action with the dataset.

Requirements
Python 3.x
Libraries:
pandas
numpy
scikit-learn
seaborn
matplotlib
Install them using:

Copy code
pip install pandas numpy scikit-learn seaborn matplotlib
License
This project is licensed under the MIT License. See the LICENSE file for more details.

Contact
For any questions or feedback, please reach out to:

Name: Abinaya V
Email: 127177002@sastra.ac.in
