# spam-message-detection

This Python script is a demonstration of SMS spam detection using Natural Language Processing (NLP) and machine learning techniques. 
It explores a dataset of SMS messages, preprocesses the text data, engineers relevant features, builds and evaluates multiple classification models,
and provides a method to predict whether a given SMS message is spam or not.

## About the Code

This code performs the following tasks:

1. Data Loading and Exploration:
   - Loads an SMS dataset from a CSV file.
   - Explores the dataset's shape, columns, data types, and basic statistics.
   - Maps labels ('ham' and 'spam') to numerical values (0 and 1).

2. Data Visualization:
   - Uses matplotlib and seaborn to create visualizations.
   - Displays a countplot for spam vs. ham messages to visualize the class distribution.
   - Handles the imbalanced dataset by oversampling the minority class.

3. Feature Engineering:
   - Creates new features such as 'word_count,' 'contains_currency_symbol,' and 'contains_number' to enhance model performance.
   - Analyzes word count distributions for spam and ham messages.

4. Data Cleaning and Text Preprocessing:
   - Cleans the text data by removing special characters and numbers.
   - Converts text to lowercase, tokenizes messages, removes stopwords, and lemmatizes words.

5. Feature Extraction:
   - Utilizes TF-IDF vectorization to convert text data into numerical format.

6. Model Building and Evaluation:
   - Constructs machine learning models including Multinomial Naive Bayes, Decision Tree, Random Forest, and a Voting Classifier.
   - Evaluates model performance using the F1-Score metric and displays classification reports and confusion matrices.
   - Selects the Random Forest model for predictions based on performance.

7. Making Predictions:
   - Defines a function to predict whether a given text message is spam or ham using the selected model.
   - Demonstrates predictions on sample text messages.

## How to Use

1. Ensure you have Python 3.x installed on your system.

Navigate to the project directory:
cd your-repo

Install the required libraries, if not already installed, using:
pip install pandas 
pip install numpy 
pip install matplotlib 
pip install seaborn 
pip install nltk 
pip install scikit-learn

Download NLTK stopwords and wordnet data:
python

import nltk
nltk.download('stopwords')
nltk.download('wordnet')

Run the main Python script:
python spam_detection.py

Follow the code comments and output to understand the functionality and behavior of the code.

Dependencies : 
Python 3.x
Libraries: pandas, numpy, matplotlib, seaborn, nltk, scikit-learn
License

This code is provided under the MIT License. Feel free to use, modify, and distribute it as needed. Refer to the LICENSE file for more details.

Author: 
Ritu R Naik

Acknowledgments: 

This code uses the NLTK library for text preprocessing and scikit-learn for machine learning.
Enjoy exploring and experimenting with SMS spam detection!


