# 📰 Fake News Detector

A Fake News Detection app built using Python, NLP, and ML, with an interactive Gradio interface. Paste any news article to check if it's REAL or FAKE.

Features

Detects whether a news article is real or fake.

Uses TF-IDF vectorization and PassiveAggressiveClassifier.

Cleans and preprocesses text (removes punctuation, numbers, stopwords, etc.).

Simple Gradio interface for user-friendly interaction.

Installation

Clone the repository:

git clone https://github.com/<your-username>/fake-news-detector.git
cd fake-news-detector


Install required libraries:

pip install nltk gradio scikit-learn pandas numpy


Download NLTK stopwords:

import nltk
nltk.download('stopwords')

Usage

Upload Fake.csv and True.csv datasets (news articles labeled fake/real).

Run the script to train the model:

python fake_news_detector.py


Launch the Gradio interface:

Paste a news article into the textbox.

Click Submit to see if the news is REAL or FAKE.

How It Works

Data Preprocessing: Combines title and text, cleans text (lowercase, remove punctuation/stopwords/URLs).

Dataset Balancing: Downsamples the real news to match fake news samples.

TF-IDF Vectorization: Converts text into numerical features.

Model Training: Uses PassiveAggressiveClassifier for binary classification.

Prediction: Cleaned text is vectorized and fed to the model for prediction.

Technologies Used

Python

NLTK
 for text preprocessing

Scikit-learn
 for ML

Gradio
 for interactive UI

Pandas & NumPy
 for data handling

Author

Keerthi Sri
