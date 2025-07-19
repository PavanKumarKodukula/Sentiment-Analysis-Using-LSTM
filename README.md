# Sentiment-Analysis-Using-LSTM

This project is a deep learning-based sentiment analysis model trained on a large dataset of tweets. It uses an LSTM (Long Short-Term Memory) network to classify tweets as Positive or Negative based on their textual content.

📌 Features
Preprocessing and cleaning of raw tweets (stopword removal, URL/mention cleanup, etc.)

Tokenization and padding using Keras

LSTM model for sentiment classification

Training with validation monitoring and learning rate reduction

Evaluation with accuracy, confusion matrix, and classification report

Visualization of training/validation loss and accuracy

Custom input prediction function

📁 Dataset
Dataset: Sentiment140

Link: https://www.kaggle.com/datasets/ferno2/training1600000processednoemoticoncsv

File used: training1600000processednoemoticon.csv

Format: Each row contains sentiment label, tweet ID, date, query, user, and tweet text

Labels:

0: Negative

4: Positive

🧠 Model Architecture
Embedding Layer (input_dim=10000, output_dim=128)

LSTM Layer (128 units)

Dropout (rate = 0.5)

Dense Output Layer with sigmoid activation for binary classification


🧪 Custom Prediction
You can test custom tweets using the following function:

def predict_sentiment(text):
    ...
    return "Positive" or "Negative"
Example:

predict_sentiment("I love this product!")  # Output: Positive
