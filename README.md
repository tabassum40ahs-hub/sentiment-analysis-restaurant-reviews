# 📌 Project Overview

This project performs sentiment analysis on McDonald's customer reviews using Natural Language Processing (NLP) and Machine Learning techniques.

The objective is to automatically classify customer reviews as Positive or Negative based on the text content.

The project compares traditional NLP approaches and transformer-based models to understand how different techniques perform on restaurant review sentiment classification.

# 📊 Dataset

The dataset consists of McDonald's restaurant customer reviews.

Each review is labeled with a sentiment:

Positive

Negative

Basic text preprocessing steps were applied before modeling:

Lowercasing text

Removing punctuation

Stopword removal

Tokenization


# ⚙️ Models Implemented

The following approaches were implemented and compared:

TF-IDF + Logistic Regression

A traditional NLP approach where text is converted into numerical features using TF-IDF vectorization, followed by a Logistic Regression classifier.

Word2Vec + Logistic Regression

Word embeddings were generated using Word2Vec to capture semantic relationships between words before training the classifier.

DistilBERT Transformer Model

A pretrained transformer model (DistilBERT) was used for sentiment classification using contextual embeddings.


# 📈 Model Evaluation

The models were evaluated using:

Accuracy

Confusion Matrix

Cross Validation

Additional testing was performed on confusing or mixed-sentiment reviews to evaluate model robustness.



# 🔍 Key Insights

TF-IDF + Logistic Regression performed best on the dataset in terms of overall accuracy.

Word2Vec underperformed, likely due to the limited dataset size.

When tested on simple reviews, most models predicted the sentiment correctly.

For confusing or mixed-sentiment reviews, traditional models sometimes struggled.

DistilBERT handled confusing reviews better, since transformer models capture contextual meaning more effectively.

Example confusing review tested:

"The burger was tasty but the service was extremely slow."

Traditional models showed uncertainty in classification, while DistilBERT handled contextual sentiment more effectively.



# 🛠 Tech Stack

Python

Pandas

NumPy

Scikit-learn

Gensim

HuggingFace Transformers

Matplotlib

Seaborn

# 💡 Future Improvements

Expand dataset with larger review collection

Improve Word2Vec embeddings with more training data

Fine-tune transformer models for better performance

Deploy the model as a web application

# 👩‍💻 Author

Tabassum Shaikh
