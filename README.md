# 📧 AI-Powered Email Phishing Detection using NLP & Machine Learning

## 🔐 About the Project

AI-Powered Email Phishing Detection is a cybersecurity project designed to identify whether an email is **Phishing** or **Legitimate** using Natural Language Processing (NLP) and Machine Learning.

The system analyzes email content and identifies patterns that can help detect potentially suspicious emails.

---

## 🎯 Objective

The main objective of this project is to build a system that can help users identify potentially malicious phishing emails before interacting with them.

The system classifies emails into:

- 🚨 **Phishing**
- ✅ **Legitimate**

---

## 🧠 How It Works

```text
Email Input
     ↓
Text Preprocessing
     ↓
NLP Processing
     ↓
TF-IDF Feature Extraction
     ↓
Machine Learning Model
     ↓
Prediction
     ↓
Phishing / Legitimate
Legitimate
🔎Features

The system can analyze email information such as:

Email subject
Email body
Suspicious keywords
Urgent language
Login or verification requests
Textual patterns commonly found in phishing emails

Examples of suspicious phrases include:

"Urgent"
"Verify your account"
"Click here"
"Login immediately"
"Your account will be blocked"

These indicators alone do not prove that an email is malicious. The machine-learning model uses patterns learned from the dataset to make the classification.

🧹 NLP Preprocessing

Before classification, the email text goes through several preprocessing steps:

HTML removal
Converting text to lowercase
Removing punctuation
Removing stopwords
Tokenization
Lemmatization
📊 TF-IDF

TF-IDF (Term Frequency-Inverse Document Frequency) is used to convert email text into numerical features that can be processed by the machine-learning model.

It helps represent the importance of words within the email dataset.

🤖 Machine Learning

Machine-learning techniques are used to classify emails based on patterns learned from previously labelled email data.

The trained model predicts whether a new email is:

Phishing or Legitimate

🖥️ Web Application

A simple web interface is developed using Flask.

Users can enter email content and receive a classification result from the trained model.

🛠️ Technologies Used
Technology	Purpose
Python	Main programming language
Scikit-learn	Machine Learning
Pandas	Data processing
NumPy	Numerical operations
NLTK	NLP processing
TF-IDF	Text feature extraction
Flask	Web application
HTML	Frontend
CSS	Styling
📁 Project Structure
AI-Email-Phishing-Detection/
│
├── README.md
├── app.py
├── requirements.txt
│
├── templates/
│   └── index.html
│
├── static/
│   └── style.css
│
└── model/
    ├── phishing_model.pkl
    └── vectorizer.pkl
🚀 Future Improvements
Gmail API integration
Real-time email analysis
Phishing confidence score
Suspicious URL analysis
Sender-domain analysis
Attachment analysis
Security dashboard
Automatic phishing/safe email labelling
