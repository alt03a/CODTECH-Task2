# CODTECH-Task2

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: SK ALTAB HOSSEN

*INTERN ID*:CT04DR1863

*DOMAIN*:MACHINE LEARNING

*DURATION*: 4 WEEKS

*MENTOR*:NEELA SANTOSH

##Task 2: Sentiment Analysis with NLP
Project Description

Title: Customer Review Sentiment Analysis using TF-IDF and Logistic Regression

Introduction Sentiment Analysis, also known as opinion mining, is a subfield of Natural Language Processing (NLP) that involves determining the emotional tone behind a body of text. It is widely used by businesses to understand customer feedback on products and services. This project focuses on building a machine learning model capable of classifying customer reviews into positive, negative, or neutral sentiments.

Methodology The project pipeline follows standard NLP practices:

Data Preprocessing: Raw text data is noisy and unstructured. I implemented a preprocessing function to clean the data. This involved:

Lowercasing: Converting all text to lowercase to ensure uniformity (e.g., "Good" and "good" are treated as the same word).

Noise Removal: Using Regular Expressions (Regex) to remove special characters, punctuation, and numbers that do not contribute to sentiment.

Stopword Removal: Filtering out common words like "is," "the," and "and" using the NLTK library. These words appear frequently but carry little semantic meaning regarding sentiment.

Feature Extraction (TF-IDF): Machine learning models cannot process raw text; they require numerical input. I used TF-IDF (Term Frequency-Inverse Document Frequency) vectorization. This technique transforms the text into a matrix of numbers. It scores words based on their frequency in a document but penalizes words that appear frequently across all documents. This ensures that unique, sentiment-rich words (like "terrible" or "fantastic") carry more weight than generic words.

Model Training: I selected Logistic Regression for the classification task. Despite its name, Logistic Regression is a linear classifier that estimates the probability of a sample belonging to a particular class. It is highly effective for binary and multi-class text classification problems, offering a good balance between speed and accuracy.

Evaluation The model was evaluated using accuracy score, a classification report (Precision, Recall, F1-Score), and a Confusion Matrix. The Confusion Matrix provided a visual breakdown of where the model succeeded and where it was confused (e.g., classifying a negative review as neutral). The results showed that the TF-IDF and Logistic Regression combination is a robust baseline for sentiment analysis tasks.

#OUTPUT
