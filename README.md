# Credit Card Fraud Detection using Regression Techniques and Neural Networks

---

**Topic:** Credit card fraud detection using regression techniques and neural networks

**Data source:** [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/mlg-ulb/creditcardfraud)

---

## Context:

Fraudulent credit card transactions pose a significant threat to both financial institutions and consumers. Detecting such transactions accurately is crucial to prevent financial losses and maintain trust in the banking system. This project focuses on utilizing regression techniques and neural networks to identify fraudulent transactions effectively.

---

## Content:

This project aims to detect credit card fraud using various machine learning models, including logistic regression, support vector machine (SVM), random forest, XGBoost, multi-layer perceptron (MLP), and a neural network built with TensorFlow/Keras. The dataset used for this project contains transactions made by credit cards in September 2013 by European cardholders, obtained from Kaggle.

1. **Data Understanding:**
   - The dataset comprises transactions from two days, with 492 frauds out of 284,807 transactions, making it highly imbalanced.
   - Features V1 to V28 are the principal components obtained with PCA, while 'Time' and 'Amount' are the only untransformed features.
   - The 'Class' feature denotes the transaction's class, with 1 indicating fraud and 0 indicating a legitimate transaction.

2. **Data Processing and Undersampling:**
   - Standardization of the 'Amount' feature using StandardScaler.
   - Random undersampling employed to address the class imbalance issue, using the imblearn library.

3. **Modeling and Evaluation:**
   - Five machine learning models are trained and evaluated:
     - Logistic Regression
     - Support Vector Machine (SVM)
     - Random Forest
     - XGBoost
     - Multi-layer Perceptron (MLP)
     - Neural Network with TensorFlow/Keras
   - Evaluation metrics include accuracy, precision, recall, F1 score, area under the ROC curve (AUC), and precision-recall curve.
   - Each model's performance is visualized through confusion matrices, ROC curves, and precision-recall curves.

4. **Findings:**
   - Logistic regression achieved an accuracy of 0.95 and an AUC of 0.97.
   - SVM yielded an accuracy of 0.94 and an AUC of 0.97.
   - Random forest exhibited an accuracy of 0.95 and an AUC of 0.97.
   - XGBoost attained an accuracy of 0.94 and an AUC of 0.97.
   - MLP achieved an accuracy of 0.95 and an AUC of 0.98.
   - The neural network with TensorFlow/Keras achieved an accuracy of 0.95 and an AUC of 0.97.

---

## Conclusion:

The analysis demonstrates that while all models performed reasonably well, the multi-layer perceptron (MLP) and the neural network built with TensorFlow/Keras showed slightly better performance, particularly in terms of AUC. However, considering various factors such as computational complexity and interpretability, the choice of the best model may vary depending on specific requirements and constraints.

---

## Recommendations:

- Continuous monitoring and updating of the fraud detection system to adapt to evolving fraud patterns.
- Exploration of ensemble methods and more advanced deep learning architectures to further enhance model performance.
- Collaboration with domain experts to incorporate additional features or insights that could improve fraud detection accuracy.

---

## References:
- Kaggle - Credit Card Fraud Detection Dataset. Retrieved from [https://www.kaggle.com/mlg-ulb/creditcardfraud](https://www.kaggle.com/mlg-ulb/creditcardfraud)
- Documentation of scikit-learn, TensorFlow, and imbalanced-learn libraries.
