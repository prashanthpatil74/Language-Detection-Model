🌐 Language Detection Model
This project provides a machine learning-based solution for automatic language identification. It aims to determine the language of any input text using traditional Natural Language Processing (NLP) techniques and statistical classifiers. The system is lightweight, interpretable, and easily extendable, making it suitable for both educational purposes and practical use.

🎯 Purpose
Language detection is a critical feature in many multilingual applications, such as:

Text preprocessing in NLP pipelines

Content moderation

Language-specific search engines

Chatbots and voice assistants

Email or message routing based on locale

This repository demonstrates how to build such a model from scratch using open-source tools.

⚙️ How It Works
Data Preparation
A labeled dataset of text samples in different languages is used for training. Each row contains a short sentence and its corresponding language label.

Text Vectorization
Text samples are converted into a numerical format using CountVectorizer or TF-IDF Vectorizer. This turns raw text into a matrix of token counts or weighted frequencies.

Model Training
A Multinomial Naive Bayes classifier is trained on the vectorized data. This algorithm is well-suited for text classification tasks and performs well even with smaller datasets.

Prediction
For a given input string, the model predicts the language by transforming the text using the same vectorizer and passing it through the trained classifier.

📊 Supported Languages
The base model supports detection of several major languages, such as:

English

French

Spanish

German

Italian

Portuguese

Dutch

Russian

Chinese

Japanese

