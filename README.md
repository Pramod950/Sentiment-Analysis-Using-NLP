# Sentiment-Analysis-Using-NLP

## Project Overview

This project performs Sentiment Analysis on movie reviews by classifying them as Positive or Negative. The performance of a traditional Machine Learning model (TF-IDF + Logistic Regression) is compared with a Deep Learning model (LSTM).

## Dataset Information

* Dataset Type: Movie Reviews
* Task: Binary Sentiment Classification
* Classes:
  * Positive (1)
  * Negative (0)
* Train-Test Split:
  * Training Data: 80%
  * Testing Data: 20%
* Validation Split: 20% of Training Data

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* TensorFlow / Keras
* Matplotlib
* Regular Expressions (Regex)

## Text Preprocessing

* Removed HTML tags
* Converted text to lowercase
* Removed special characters and numbers
* Removed extra spaces

## Feature Engineering

### TF-IDF Vectorization

* Maximum Features: 5000
* N-gram Range: (1,1) - Unigrams

### Tokenization for LSTM

* Vocabulary Size: 5000 words
* Maximum Sequence Length: 100
* Longer sequences were truncated
* Shorter sequences were padded

## Model 1: TF-IDF + Logistic Regression

### Performance

* Accuracy: 90%
* Precision: 0.92
* Recall: 0.90
* F1-Score: 0.90

## Model 2: LSTM Neural Network

### Architecture

* Embedding Layer (5000, 128)
* LSTM Layer (64 Units)
* Dense Layer (32 Units, ReLU)
* Dropout Layer (0.2)
* Output Layer (Sigmoid)

### Training Configuration

* Loss Function: Binary Crossentropy
* Optimizer: Adam

### Performance

* Accuracy: 85%
* Precision: 0.86
* Recall: 0.85
* F1-Score: 0.85

## Model Comparison

| Model                        | Accuracy |
| ---------------------------- | -------- |
| TF-IDF + Logistic Regression | 90%      |
| LSTM Neural Network          | 85%      |

## Key Insights

* TF-IDF + Logistic Regression achieved the highest accuracy.
* Text preprocessing improved model performance.
* LSTM captured sequence information but required more data for better results.
* Traditional Machine Learning performed better than Deep Learning on this small dataset.

## Skills Demonstrated

* Natural Language Processing (NLP)
* Text Preprocessing
* TF-IDF Vectorization
* Logistic Regression
* Deep Learning
* LSTM Networks
* Sentiment Analysis
* Model Evaluation
* TensorFlow/Keras
* Scikit-learn

## Conclusion

The TF-IDF + Logistic Regression model achieved the best performance with 90% accuracy, outperforming the LSTM model (85%) on this dataset.
