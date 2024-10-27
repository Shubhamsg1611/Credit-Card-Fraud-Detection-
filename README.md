# Credit Card Fraud Detection Project 
![](https://www.datascienceportfol.io/static/profile_pics/pr14_A38ED02CE0D67F0A3BF5.jpg)

### Overview of Model Training:
In this model training project, the goal was to classify transactions as either normal or fraudulent with high accuracy. To achieve this, we utilized a combination of data preprocessing, feature extraction through an autoencoder, and classification via logistic regression. The model’s performance was evaluated on precision, recall, F1-score, and accuracy.

1. **Data Preprocessing:**
- Standardized the Amount feature to match the range and scale of other features, creating consistency.
- Used an autoencoder to reduce dimensionality and emphasize essential patterns, especially for the smaller fraud class.

2. **Classification Model:**
- Trained a logistic regression model on extracted features to classify transactions, effectively capturing differences between normal and fraudulent behaviors.
- Evaluated the model to ensure balanced performance, focusing on both fraud detection and avoiding false positives in normal transactions.

### Conclusion: 
The final model achieved an overall accuracy of 98.5%, demonstrating a high capability in classifying transactions correctly:

- Normal Transactions (Class 0): Precision and recall were both close to perfect at 0.98 and 1.0, respectively, highlighting the model's accuracy in identifying non-fraudulent cases.

- Fraudulent Transactions (Class 1): Although precision was excellent (1.0), the recall was 0.59, meaning that while the model is very accurate when it labels a transaction as fraud, it missed some true fraud cases.

### Summary: 

- Strengths: The model is highly effective at identifying normal transactions with minimal false positives, which is crucial for maintaining smooth transaction flow in real-world applications.
- Areas for Improvement: To increase recall for fraudulent cases, additional strategies like advanced sampling techniques or further tuning of the autoencoder and classifier may be beneficial.

The model effectively identifies fraudulent transactions, achieving an optimal balance between accuracy and performance, though it could be fine-tuned to further enhance fraud detection sensitivity.
