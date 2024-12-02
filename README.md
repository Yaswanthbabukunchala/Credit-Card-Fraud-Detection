Credit Card Fraud Detection using Support Vector Machine (SVM)

Overview
This project focuses on detecting fraudulent transactions in credit card datasets using a Support Vector Machine (SVM) algorithm. Fraud detection is crucial in ensuring the security of online transactions, and machine learning techniques like SVM can help accurately identify fraudulent behavior.

Table of Contents
Introduction
Dataset
Methodology
Requirements
Installation and Setup
Usage
Results
Contributing
License
Introduction
Credit card fraud detection involves classifying transactions as fraudulent or non-fraudulent. Due to the imbalanced nature of the dataset (fewer fraudulent transactions compared to genuine ones), specialized techniques such as oversampling and under-sampling are often used to improve model performance. SVM is effective in separating classes with a clear boundary and works well even in high-dimensional spaces.

Dataset
The dataset used in this project is a publicly available credit card dataset:

Source: Kaggle Credit Card Fraud Detection Dataset
Features:
30 features including Time, Amount, and 28 anonymized principal components obtained via PCA.
Class: Target variable where 1 = Fraudulent and 0 = Non-fraudulent.
Preprocessing Steps
Data scaling using StandardScaler to normalize transaction Amount and Time.
Addressing class imbalance using techniques like SMOTE (Synthetic Minority Oversampling Technique).
Methodology
Data Preprocessing:

Remove noise and scale numerical features.
Balance the dataset.
Model Selection:

SVM with kernel options (linear, RBF, poly) is tested.
Evaluation Metrics:

Accuracy, Precision, Recall, F1-Score, and AUC-ROC.
Implementation:

Libraries used include scikit-learn, pandas, and numpy.
Model tuning with grid search for optimal hyperparameters.
Requirements
Software
Python 3.8 or higher
Jupyter Notebook (optional)
Python Libraries
pandas
numpy
scikit-learn
matplotlib
seaborn
imbalanced-learn
Install dependencies with:

bash
Copy code
pip install -r requirements.txt
Installation and Setup
Clone the repository:
bash
Copy code
git clone https://github.com/your-username/CreditCardFraudDetection.git
cd CreditCardFraudDetection
Install dependencies:
bash
Copy code
pip install -r requirements.txt
Run the notebook or script:
bash
Copy code
python fraud_detection.py
Usage
Place the dataset (creditcard.csv) in the data/ directory.
Run the script to preprocess data and train the model.
Evaluate the model on the test set using the provided evaluation metrics.
