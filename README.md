Project Name : Customer Churn Prediction using Artificial Neural Network (ANN)

Project Overview:
This project aims to predict whether a bank customer will churn (leave the bank) using an Artificial Neural Network (ANN).
The model is trained on customer demographic and financial data and achieves high prediction accuracy.

1. Dataset :

Source: Kaggle – Credit Card Customer Churn Dataset
File Used: Churn_Modelling.csv

2. Target Variable :
Exited
1 → Customer exited
0 → Customer retained

3. Technologies Used :

  a. Python 3
  b. NumPy
  c. Pandas
  d. Scikit-learn
  e. TensorFlow / Keras
  f. Matplotlib

4. Data Preprocessing

   Removed unnecessary columns:
     a. RowNumber
     b. CustomerId
     c. Surname

   One-hot encoding applied to:
     a. Geography
     b. Gender

5. Train-test split: 80% / 20%
   Feature scaling using StandardScaler

6. Model Architecture :
    | Layer          | Neurons | Activation |
| -------------- | ------- | ---------- |
| Input Layer    | 11      | —          |
| Hidden Layer 1 | 16      | ReLU       |
| Hidden Layer 2 | 8       | ReLU       |
| Output Layer   | 1       | Sigmoid    |

7. Model Compilation :
   
    model.compile(
    optimizer='adam',
    loss='binary_crossentropy',
    metrics=['accuracy'])

8. Model Training
     Epochs: 100
     Batch Size: 32
     Validation Split: 20%
9. Evaluation Metrics
     Accuracy
     Confusion Matrix
     ROC–AUC Curve
     Loss & Accuracy graphs
10. Results :
    | Metric      | Value   |
 | ----------- | ------- |
 | Accuracy    | ~86–88% |
 | ROC-AUC     | ~0.87   |
 | Overfitting | Minimal |
Model performs well on unseen data
Good generalization
Suitable for business use cases

11. Visualizations Included :
    
    Training vs Validation Loss
    Training vs Validation Accuracy
    Confusion Matrix
    ROC Curve

12. Future Improvements :
    Add Dropout layers
    Hyperparameter tuning
    Use XGBoost / Random Forest
    Handle class imbalance with SMOTE
    Deploy using Streamlit or Flask
    
13 Conclusion:

    This project demonstrates how Artificial Neural Networks can effectively predict customer churn.
    Such a model can help banks retain customers by identifying churn risks early.

