# Language Detection Using Multinomial Naive Bayes

This repository contains a complete implementation of a language detection system using a Multinomial Naive Bayes classifier. The project leverages natural language processing (NLP) techniques to classify text snippets into one of 22 languages based on their written content.

## Project Overview

Language detection is a fundamental task in NLP with applications in multilingual search engines, content filtering, and automatic translation. This project demonstrates a straightforward yet effective approach using classical machine learning methods without requiring deep learning.

The dataset consists of 22,000 text samples spanning 22 distinct languages including English, Spanish, Chinese, Hindi, Arabic, French, and more. Each sample is a short text labeled by its language.

## Features

- **Data Loading and Preprocessing:** Reads a CSV file containing text and corresponding language labels.
- **Feature Extraction:** Utilizes `CountVectorizer` to convert text data into numerical feature vectors using the bag-of-words model.
- **Model Training:** Applies `MultinomialNB` classifier from scikit-learn to learn from the training data.
- **Evaluation:** Measures model accuracy on a held-out test set, achieving approximately 95% accuracy.
- **Prediction Interface:** Allows user input of text to predict its language dynamically.

## Dataset

- The data file `language.csv` contains 22,000 rows.
- Two columns: `Text` (text snippet) and `language` (language label).
- Balanced dataset with 1000 samples per language for 22 languages.

## Technologies Used

- Python 3
- Pandas for data handling
- NumPy for numerical operations
- scikit-learn for machine learning (feature extraction, model training, evaluation)
- Jupyter Notebook or any Python IDE for development and testing

## How to Use

1. Clone the repository.
2. Place `language.csv` in the root directory or update the path in the script.
3. Run the script or notebook to train and evaluate the model.
4. Input custom text when prompted to get language prediction.

## Results

- The Multinomial Naive Bayes model achieved around **95.3% accuracy** on the test set.
- The model efficiently distinguishes between multiple languages using simple word count features.

---
