# 🧠 Suicidal Thoughts Classification with Machine Learning

This repository contains the implementation of the project *Utilizing Machine Learning Models to Classify Suicidal Thoughts Using Data from Twitter/X*. The project aims to detect suicidal tendencies based on data from the **Twitter/X** social media platform using various *Natural Language Processing (NLP)* techniques and *Machine Learning* models.

## 🌟 Background

Every year, approximately 703,000 people worldwide end their lives, making suicide the fourth leading cause of death among individuals aged 15-29 years. In Indonesia, 6,544 suicide-related deaths were recorded in 2019. By leveraging data from Twitter/X, this project aims to enable early detection of suicidal thoughts and direct individuals to support services such as suicide hotlines or psychologists.

## 🔍 Methodology

### 1. Data Collection 📊
The dataset was collected by scraping Twitter/X using Python. Keywords like "capek hidup" (tired of life), "depresi" (depression), and "nyerah" (give up) were used to gather approximately 3,000 tweets in CSV format.

### 2. Data Preprocessing 🛠️
The preprocessing steps included cleaning and transforming the data:
- **Data Cleaning**: Removing irrelevant elements like mentions, hashtags, and URLs.
- **Normalization**: Converting informal or abbreviated words into their formal forms.
- **Spell Correction**: Fixing spelling errors.
- **Stopword Deletion**: Removing insignificant words.
- **Tokenization & Lemmatization**: Splitting text into smaller units and converting them into their root forms.
- **Labeling**: Using the *DistilBERT* model to label tweets as *neutral*, *positive*, or *negative*.

### 3. Fine-Tuning and Modelling 🤖
The models used were:
- **Random Forest** 🌳
- **Support Vector Machine (SVM)** 📈
- **IndoBERT** 📚

### 4. Validation and Evaluation 📉
The models were tested to achieve the following accuracies:
- **SVM**: 84.8%
- **Random Forest**: 84%
- **IndoBERT**: 87%

## 🚀 Implementation
The process and experiments can be accessed in this Repository

## 📈 Analysis
The **IndoBERT** model outperformed others with an accuracy of 87%, demonstrating its superior ability to understand complex textual contexts.

## ✅ Strengths
- Focuses on mental health issues for social media users.
- Uses original data.
- Implements *state-of-the-art* NLP models like IndoBERT.

## ❌ Limitations
- The dataset consists of only 3,000 tweets, causing the model to be biased towards negative data.
- No deployment as a web application has been implemented yet.

## 🏁 Conclusion
This project demonstrates that the IndoBERT method is effective in detecting suicidal tendencies in tweets. With additional data and better dataset balancing, the model's accuracy could be further improved.

---


