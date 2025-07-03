# SVM-Classification
OBJECTIVE:
Use Support Vector Machines (SVM) for linear and non-linear classification on the Breast Cancer dataset.

TOOLS USED:
Python
Scikit-learn
NumPy
Pandas
Matplotlib

DATASET:
The dataset used is the "Breast Cancer Wisconsin (Diagnostic)" dataset containing 569 instances with 30 numeric features each. The target variable is 'diagnosis' with two classes:
Malignant (M)
Benign (B)

STEPS FOLLOWED:
1. Data Loading and Preprocessing:
->Loaded the dataset using Pandas.
->Dropped the 'id' column as it's not useful for classification.
->Encoded the 'diagnosis' column to binary values (M=1, B=0).
->Selected features and target variable.
->Standardized features using StandardScaler.

2. Splitting the Data:
Split the data into training and testing sets using train_test_split (80% train, 20% test).

3. SVM Classification:
Trained a Linear SVM using SVC(kernel='linear').

Trained a Non-Linear SVM using the RBF Kernel (SVC(kernel='rbf')).

Evaluated both models using classification reports (precision, recall, f1-score).

4. Visualization:
Selected the top 2 features based on variance for 2D visualization.

Plotted the decision boundary for the RBF kernel using Matplotlib.

5. Hyperparameter Tuning:
Used GridSearchCV to find the best hyperparameters for SVM (C and gamma).

Evaluated the best model using cross-validation and test set performance.

Key Hyperparameters:
C: Regularization parameter (tested values: 0.1, 1, 10, 100).

Gamma: Kernel coefficient (tested values: 0.01, 0.1, 1, 'scale').

RESULTS:
Achieved high classification accuracy with both Linear and RBF SVMs.

Visualized decision boundaries to better understand model behavior.

Hyperparameter tuning further improved model performance.

HOW TO RUN:
Install required libraries:

bash
Copy
Edit
pip install numpy pandas scikit-learn matplotlib
Place the breast cancer dataset CSV in your working directory.
Run the provided Python script.

CONCLUSION:
Support Vector Machines are powerful classifiers for both linear and non-linear problems. Proper scaling, hyperparameter tuning, and visualization can significantly improve performance and understanding.

AUTHOR:
LAKSHMI CHANDANA YANAMANDRA

