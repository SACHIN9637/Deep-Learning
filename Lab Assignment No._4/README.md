# NLP_Text_Classification

This repository implements a Spam Detection System using Natural Language Processing (NLP) and machine learning models like Logistic Regression and Naive Bayes. It classifies text messages as either spam or ham (not spam) using the SMS Spam Collection Dataset.

🔍 Features
Data preprocessing (lowercasing, tokenization, stopword removal, stemming, and lemmatization)

Feature extraction using CountVectorizer and TF-IDF Vectorizer

Classification using:

Logistic Regression

Multinomial Naive Bayes

Evaluation using accuracy, precision, recall, F1-score, and confusion matrix

Predicts spam/ham for custom input text

🗂 Dataset
The dataset used is SMS Spam Collection, which consists of over 5,000 labeled SMS messages.

Sample:

csv
Copy
Edit
label,message
ham,Ok lar... Joking wif u oni...
spam,Free entry in 2 a wkly comp to win FA Cup final tkts 21st May 2005...
🧰 Requirements
Install the dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Main Libraries Used:

pandas

nltk

scikit-learn

matplotlib

seaborn

⚙️ How It Works
1. Preprocessing
Convert to lowercase

Tokenize the text

Remove stopwords and non-alphabetic tokens

Apply stemming and lemmatization

Join tokens to form clean text

2. Vectorization
Transform text into numerical features using:

CountVectorizer

TfidfVectorizer

3. Model Training
Train using:

Logistic Regression

Multinomial Naive Bayes

4. Evaluation
Evaluate model performance using:

Accuracy

Precision

Recall

F1-score

Confusion Matrix (Visualized with Seaborn)
