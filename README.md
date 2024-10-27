# Credit Card Fraud Detection Project 
![](https://www.datascienceportfol.io/static/profile_pics/pr14_A38ED02CE0D67F0A3BF5.jpg)

This fraud detection project trained a classifier to identify fraudulent transactions within an imbalanced dataset. Using an autoencoder for dimensionality reduction, essential transaction features were extracted to improve detection accuracy. A logistic regression model achieved high overall accuracy (95%) and strong performance in identifying non-fraudulent transactions. However, the model’s recall for fraudulent transactions was lower, indicating a need for further tuning to enhance fraud sensitivity. In summary, the project demonstrates effective fraud detection with room for improvement in capturing all instances of fraud.

### Overview of Model Training:
The objective of model training in this fraud detection project was to develop a reliable classifier to distinguish between normal (non-fraudulent) and fraudulent transactions. The dataset, which contained significantly more non-fraudulent transactions than fraudulent ones, required careful handling to ensure balanced model performance. Here’s a breakdown of the key steps in the training process:

- Data Preprocessing: The Amount feature was normalized to standardize transaction values, preventing large values from skewing the model’s learning process.
The dataset was split into training and test sets, ensuring a mix of both classes for evaluation.

- Dimensionality Reduction: An autoencoder was employed to capture the most informative features of the transaction data, reducing dimensionality while retaining essential patterns.
The autoencoder’s hidden representations were then used to create compressed features, enabling the model to focus on core transaction characteristics relevant to fraud detection.

- Classification Model: A logistic regression classifier was trained using the hidden representations from the autoencoder. This approach helped maintain a balance between computational efficiency and prediction accuracy.
Given the imbalanced dataset, precision, recall, and F1-score were critical metrics to assess the model’s effectiveness in predicting fraudulent transactions accurately.

- Performance Evaluation: The model was evaluated based on classification metrics including precision, recall, F1-score, and accuracy. While the overall accuracy reached 95%, recall for fraudulent transactions indicated that further tuning could improve detection rates.

### Conclusion of Model Training:
The model training process successfully yielded a classifier with high accuracy and strong predictive capabilities for non-fraudulent transactions. However, the model’s recall score for fraudulent transactions suggests a potential under-detection of fraud, indicating room for improvement.

### Key Takeaways:

- Strengths: The model performs reliably for non-fraudulent transactions, achieving high precision and recall in this class.

- Areas for Improvement: The reduced recall for fraud cases suggests the model could be further optimized for greater sensitivity to fraud patterns, potentially by addressing the class imbalance more intensively.

In summary, the model shows strong performance but could benefit from additional tuning to ensure it captures a higher number of fraudulent transactions accurately.

