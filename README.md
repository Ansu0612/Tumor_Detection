# Tumor_Detection

Introduction

This project aims to help medical professionals accurately detect tumors in medical images. By leveraging the power of machine learning, specifically the Random Forest algorithm, we've developed a model capable of analyzing images and identifying potential tumor indicators.

Data and Preprocessing

We utilized a dataset comprising [number] medical images, each labeled as either "benign" or "malignant." To prepare the data for model training, we performed the following preprocessing steps:

Image Resizing: All images were resized to a uniform size to ensure consistent input for the model.
Data Augmentation: To increase the diversity of the training data, we applied techniques like rotation, flipping, and zooming to generate additional training samples.
Data Normalization: The pixel values of the images were normalized to a specific range (e.g., 0-1) to improve model performance.
Model Training

We employed a Random Forest classifier, a powerful ensemble learning technique, to train our model. The training process involved:

Data Splitting: The dataset was divided into training and testing sets in an 80:20 ratio.
Model Training: The Random Forest model was trained on the training set, learning to identify patterns associated with tumor presence.
Model Evaluation: The trained model was evaluated on the testing set to assess its performance.
Results and Evaluation

Our model achieved an accuracy of 96.4% on the test set. To gain deeper insights into the model's performance, we analyzed the confusion matrix:

[[106   2]
 [  4  59]]
              precision    recall  f1-score   support

           0       0.96      0.98      0.97       108
           1       0.97      0.94      0.95        63

    accuracy                           0.96       171
   macro avg       0.97      0.96      0.96       171
weighted avg       0.96      0.96      0.96       171
