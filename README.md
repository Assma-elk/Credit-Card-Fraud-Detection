# Credit-Card-Fraud-Detection



## Overview

This project explores the problem of credit card fraud detection using machine learning techniques. Fraudulent transactions are rare but critical to identify, as they can lead to major financial losses. The main goal here is to accurately classify transactions as fraudulent or genuine, despite the strong class imbalance.

The project uses the famous [Kaggle credit card fraud dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud), which contains anonymized data for over 280,000 transactions, with just 0.17% labeled as fraud.

## Project Steps

* **Data Exploration:** Initial inspection and visualization to understand the distribution and detect possible data issues.
* **Data Preprocessing:** Scaling the transaction amount and removing unhelpful columns.
* **Model Training:** Training both a Decision Tree and a Random Forest classifier on the data.
* **Model Evaluation:** Assessing models using confusion matrices and classification metrics (accuracy, precision, recall, F1-score).
* **Handling Imbalanced Data:** Using the SMOTE technique to oversample the minority class (frauds) and improve model performance.
* **Performance Comparison:** Evaluating the impact of oversampling on detection rates.

## Dataset

* **Source:** [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
* **Features:**

  * `V1` to `V28`: Principal components resulting from PCA, due to privacy reasons.
  * `Amount`: Transaction amount (scaled in preprocessing)
  * `Time`: Seconds elapsed between each transaction and the first transaction in the dataset (removed in preprocessing)
  * `Class`: Target variable (0 = genuine, 1 = fraud)

## Requirements

* Python 3.x
* pandas
* numpy
* matplotlib
* scikit-learn
* imbalanced-learn

## Installation

```bash
pip install pandas numpy matplotlib scikit-learn imbalanced-learn
```

## How to Run

1. Download the dataset from Kaggle and place the `creditcard.csv` file in the appropriate folder.
2. Run the Jupyter notebook or Python script step by step.
3. Results, plots, and evaluation metrics will be displayed for each step.

## Results

* Random Forest outperforms Decision Tree on this dataset.
* Handling class imbalance with SMOTE leads to a significant improvement in fraud detection rates, especially recall for the minority class.
* The project highlights the importance of proper preprocessing and balancing techniques in real-world fraud detection tasks.

## Acknowledgments

* Dataset: [Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
* Tutorial inspiration: DataFlair and various Kaggle kernels
