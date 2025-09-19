# Twitter-Emotion-Classifier
**Introduction
This project implements a machine learning solution to classify emotions or feelings from text data. The goal is to train various models to accurately predict the emotion label associated with a given text. The project uses a dataset split into training, validation, and testing sets.

**Dataset
The project uses three separate CSV files: training.csv, validation.csv, and test.csv. Each file contains two columns:

text: The input text containing an emotion or feeling.

label: The corresponding numerical label for the emotion.


**Methodology
The machine learning pipeline consists of several key steps:

1. Data Pre-processing
The text data is cleaned to improve model performance. This involves several transformations, including:

Removing special characters and numbers.

Tokenization of each word.

Removing English stop words.

Lemmatization to reduce words to their base or root form.

2. Feature Extraction
The pre-processed text data is converted into a numerical format using the TfidfVectorizer. This technique transforms text into a matrix of TF-IDF features, with a maximum of 5,000 features considered.

3. Model Training and Evaluation
Several classification models were trained and evaluated on the data to determine the best-performing approach. The models tested include:

Logistic Regression: Multiple models were evaluated by tuning hyperparameters, with the best model achieving an accuracy of 87.75%.

Support Vector Machines (SVM): Various linear kernel SVM models were tested, with the most effective one reaching an accuracy of 87.625%.

Random Forest Classifier: Hyperparameters were tuned to find the optimal model, which obtained an accuracy of 87.958%.

Long Short-Term Memory (LSTM): A neural network approach was also implemented and evaluated, achieving a validation accuracy of 86.35%.


**Dependencies
The following Python libraries are required to run this project:

pandas

scikit-learn

nltk

re

matplotlib

wordcloud

keras

tensorflow
