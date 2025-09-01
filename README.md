Twitter Sentiment Analysis
A Python project that performs sentiment analysis on Twitter data, classifying tweets into positive, negative, or neutral categories using various machine learning and deep learning models.

This repository demonstrates the process of text preprocessing, feature extraction (TF-IDF), and model training for a multi-class classification task.

Features
Text Preprocessing: Cleans raw tweet data by removing URLs, mentions, hashtags, special characters, and stop words.

Feature Extraction: Uses TF-IDF to convert cleaned text into a numerical format suitable for machine learning.

Model Comparison: Implements and evaluates several different classification models to compare their performance.

Models Implemented
This project trains and compares the following models:

Traditional Machine Learning:

Multinomial Naive Bayes

Complement Naive Bayes (with hyperparameter tuning via GridSearchCV)

Deep Learning (using TensorFlow/Keras):

Simple Recurrent Neural Network (RNN)

Long Short-Term Memory (LSTM)

Bidirectional LSTM (Bi-LSTM)

Dataset
This project uses the "Twitter Data" dataset, which can be found on Kaggle.

Source: Kaggle - Twitter Sentiment Analysis

Important: To run this project, please download the Twitter_Data.csv file from the link above and place it in the root directory of this project.

Getting Started
Follow these instructions to get a copy of the project up and running on your local machine.

Prerequisites
Python 3.9 or higher

pip (Python package installer)

Installation
Clone the repository:

git clone [https://github.com/lokeshreddyyaswamy/Sentiment_Analysis.git](https://github.com/lokeshreddyyaswamy/Sentiment_Analysis.git)
cd Sentiment_Analysis

Create and activate a virtual environment (recommended):

# For macOS/Linux
python3 -m venv venv
source venv/bin/activate

# For Windows
python -m venv venv
.\venv\Scripts\activate

Install the required packages:

pip install -r requirements.txt

Download NLTK data:
Run the following commands in a Python interpreter to download the necessary NLTK models:

import nltk
nltk.download('stopwords')
nltk.download('punkt')
nltk.download('wordnet')

Usage
After setting up the environment and placing Twitter_Data.csv in the root folder, you need to update the file path in the script.

Open sentiment_analysis.py.

Change this line:

df = pd.read_csv('/content/Twitter_Data.csv')

to this:

df = pd.read_csv('Twitter_Data.csv')

Run the script from your terminal:

python sentiment_analysis.py

The script will then preprocess the data, train each model, and print the accuracy and classification report for each one.

License
This project is licensed under the MIT License - see the LICENSE file for details.
