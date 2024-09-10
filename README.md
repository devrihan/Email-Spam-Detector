# Spam Detection Model

## Overview
This project demonstrates a basic spam detection system using **Naive Bayes** classification. The system is trained to distinguish between spam and non-spam messages using a dataset of SMS messages.

## Dataset
The dataset used is `spam.csv`, containing two columns:
- **Category**: Indicates whether the message is "spam" or "ham" (non-spam).
- **Message**: The content of the SMS message.

## Steps
1. **Data Preprocessing**: 
   - The `Category` column is converted into a binary format where `1` represents spam and `0` represents ham.
2. **Feature Extraction**:
   - Used `CountVectorizer` to transform the text data into a matrix of token counts.
3. **Modeling**:
   - Applied **Multinomial Naive Bayes** classifier to the tokenized data.
4. **Evaluation**:
   - The model achieved an accuracy score of **98.64%** on the test data.
5. **Prediction**:
   - Tested the model with two sample emails, where it correctly predicted one as spam and the other as non-spam.

## Libraries Used
- `pandas`: For data manipulation
- `scikit-learn`: For machine learning models and text vectorization

## How to Use
1. Ensure the required libraries are installed:
   ```bash
   pip install pandas scikit-learn
   ```
2. Load the dataset and run the script.
3. The trained model can predict whether a given message is spam or not.
