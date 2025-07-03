# Credit-Card-Fraud-Detection

To detect fraudulent credit card transactions using machine learning algorithms. The goal is to classify each transaction as fraudulent (1) or legitimate (0) based on transaction details.
Dataset Description:
Files:

fraudtrain.csv – Training data with labeled transactions

fraudtest.csv – Test data for evaluating the model

Columns (after cleanup):

amount, merchant, category, gender, city_pop, amt, etc.

is_fraud – Target variable (0: not fraud, 1: fraud)

Methodology:
Data Cleaning:

Dropped unnecessary or personal-identifiable information (e.g., names, card numbers, timestamps).

Encoded categorical features using One-Hot Encoding.

Feature Scaling:

Used StandardScaler to normalize numerical data (especially useful for Logistic Regression).

Model Training:

Tried and compared multiple classifiers:

Logistic Regression (baseline)

Decision Tree Classifier

Random Forest Classifier

Evaluation Metrics:

Accuracy: Overall correctness

Precision & Recall: Important due to class imbalance

F1-score: Harmonic mean of precision and recall

Confusion Matrix: Visual representation of true vs. predicted classes

Handling Class Imbalance (Optional):

Option to use class_weight='balanced' or SMOTE (Synthetic Minority Oversampling Technique) if fraud cases are rare.

Tools Used:
Python

Pandas

Scikit-learn

Seaborn / Matplotlib for plotting

Result:
Random Forest generally achieved the highest accuracy and recall for detecting fraud.

Logistic Regression was fastest but slightly less accurate.

Models can be further improved using ensemble techniques or deep learning.
