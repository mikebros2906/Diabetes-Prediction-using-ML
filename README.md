**Diabetes Prediction using Machine Learning (PIMA Dataset)**

**📜 Overview**
This project implements a machine learning model to predict whether a person has diabetes or not, based on diagnostic measurements included in the PIMA Indians Diabetes Dataset. A Support Vector Machine (SVM) classifier is used for this binary classification task.

**📊 Dataset**
The project uses the PIMA Indians Diabetes Dataset, which contains health-related data for female patients of Pima Indian heritage.

⦁	Total Samples (Rows): 768
⦁	
⦁	Total Features (Columns): 9
⦁	
⦁	Distribution of Outcome:
	1. Non-Diabetic (0): 500
	2. Diabetic (1): 268

**🛠 Dependencies**
The following Python libraries are required to run this project:

numpy

pandas

sklearn (specifically StandardScaler, train_test_split, svm, accuracy_score)

You can install them using pip:

Bash

pip install numpy pandas scikit-learn

**🔬 Data Preprocessing and Analysis**
Data Loading: The diabetes.csv file is loaded into a pandas DataFrame.

Feature and Label Separation: The data is split into features (X) by dropping the Outcome column and labels (Y) which is the Outcome column.

Data Standardization: To bring all features to a common range and prevent any single feature from dominating the model training due to its magnitude, a StandardScaler is applied to the features (X).

Train Test Split: The standardized data is split into training and testing sets:

Training Set: 80 of the data (used to train the model).

Test Set: 20 of the data (used to evaluate the model's performance on unseen data).

The split is performed with stratify=Y to ensure a proportional representation of diabetic and non-diabetic cases in both sets.

**⚙️ Model Training**
A Support Vector Machine (SVM) classifier with a linear kernel is used for training.

✅ Model Evaluation
The model is evaluated using the accuracy score on both the training and test datasets.

Dataset	Accuracy Score
Training Data	$\mathbf{78.66%}$
Test Data	$\mathbf{77.27%}$
