<div align="center">
<h1 align="center">📊 Twitter Sentiment Analysis 📊</h1>
<p align="center">
Classifying tweets into positive, negative, or neutral categories using Machine Learning and Deep Learning.
</p>
</div>

<div align="center">

</div>

This repository contains a Python project that performs sentiment analysis on Twitter data. It demonstrates the complete workflow from raw text preprocessing to training and evaluating various classification models.

✨ Features
🧹 Text Preprocessing: Cleans raw tweet data by removing URLs, mentions, hashtags, special characters, and stopwords.

🔢 Feature Extraction: Uses TF-IDF to convert cleaned text into a numerical format suitable for machine learning.

🤖 Model Comparison: Implements and evaluates several different classification models to compare their performance.

🚀 Models Implemented & Performance
This project trains and compares the following models. The accuracy scores below are based on the test set and may vary slightly on different runs.

Model

Test Accuracy

Multinomial Naive Bayes

~90.6%

Complement Naive Bayes

~90.6%

Simple RNN

~95.3%

LSTM

~95.7%

Bidirectional LSTM

~95.8%

💾 Dataset
This project uses the "Twitter Data" dataset, which can be found on Kaggle.

Source: Kaggle - Twitter Sentiment Analysis

Important: To run this project, please download the Twitter_Data.csv file from the link above and place it in the root directory of this project.

⚙️ Getting Started
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
Run the following command in your terminal to download the necessary NLTK models:

python -c "import nltk; nltk.download('stopwords'); nltk.download('punkt'); nltk.download('wordnet')"

▶️ Usage
After setting up the environment and placing Twitter_Data.csv in the root folder, you need to update the file path in the script.

Open sentiment_analysis.py.

Change this line:

df = pd.read_csv('/content/Twitter_Data.csv')

to this:

df = pd.read_csv('Twitter_Data.csv')

Run the script from your terminal:

python sentiment_analysis.py

The script will then preprocess the data, train each model, and print the accuracy and classification report for each one.

📄 License
This project is licensed under the MIT License - see the LICENSE file for details.
