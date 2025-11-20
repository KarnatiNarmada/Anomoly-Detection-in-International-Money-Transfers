# Anomoly-Detection-in-International-Money-Transfers


Overview:
This project demonstrates an end to end fraud detection pipeline using a synthetic dataset modeled after international money transfer activity. The goal is to accurately identify fraudulent transactions by combining unsupervised and supervised machine learning techniques. The project follows a structured data science workflow covering data preparation, anomaly detection, model training, evaluation, and risk scoring.

Project Summary:
The dataset contains transaction level information such as amount, exchange rate, account age, past transactions and whether the transfer is international. A hybrid fraud label was created by combining true fraud records with anomalies detected using the Isolation Forest algorithm. This approach improves the ability to capture unusual patterns that are not labeled in the original dataset.

The training process includes cleaning the data, scaling the numeric features, applying SMOTE to handle class imbalance, and splitting the data into training and testing sets. A Balanced Random Forest model was then trained to classify transactions as normal or fraudulent. The model was evaluated using accuracy, precision, recall, F1 score, ROC curve and a confusion matrix. The system also identifies the top twenty highest risk transactions for manual investigation.

Key Steps:

Loaded and cleaned the synthetic dataset representing Remitly style transactions.

Selected key numerical features for modeling and applied standard scaling.

Used Isolation Forest to detect anomalies and built a combined hybrid fraud label.

Split the dataset into training and testing groups using an 80 20 ratio.

Applied SMOTE to balance the dataset and improve fraud detection.

Trained a Balanced Random Forest classifier to learn fraud behavior.

Evaluated the model using standard performance metrics.

Generated visual results including confusion matrix, ROC curve and performance summary.

Exported the highest risk transactions for further review.

Saved the trained model for future use.

Model Performance Summary:
Accuracy approximately 97 percent
Precision approximately 96 percent
Recall approximately 96 percent
F1 score approximately 0.96
ROC AUC approximately 0.998

These results show that the model performs extremely well in distinguishing fraud from normal transactions with minimal false positives and false negatives.

Project Outcomes:
This project demonstrates strong capability in building practical fraud detection solutions using both unsupervised and supervised learning. It highlights skills in Python, data processing, anomaly detection, machine learning model development, evaluation and reporting. The work simulates real world financial fraud detection environments and showcases the ability to handle imbalanced and high risk data.

Directory Structure:
data folder contains the synthetic dataset
models folder contains the saved model file
results folder contains exported high risk predictions
main script performs the entire fraud detection workflow

Conclusion:
This project serves as a complete demonstration of developing a robust fraud detection system. It reflects strong technical understanding of machine learning techniques and the ability to translate them into practical, production ready workflows.
