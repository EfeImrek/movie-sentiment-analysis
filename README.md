# 🎬 Movie Sentiment Analysis  
**Course:** DSA 210 - Introduction to Data Science  
**Term:** Fall 2025–2026  
**Author:** [Your Name]  

---

## 🎯 Project Motivation  
This project aims to analyze movie reviews and determine whether they express **positive** or **negative** emotions using data science and machine learning techniques.  
The main goal is to explore public sentiment around movies and build a classifier that can automatically predict the tone of a review.

---

## 📊 Data Sources  
- **Main dataset:** IMDb Movie Reviews Dataset (from Kaggle)  
  → Contains thousands of labeled movie reviews.  
- **Additional dataset:** IMDb ratings or Google Trends data.  
  → Used to enrich the dataset and compare sentiment with popularity.

---

## 🧪 Methodology  

### 1. Data Cleaning  
- Convert all text to lowercase  
- Remove punctuation, stopwords, and special symbols  
- Tokenize and lemmatize the text  

### 2. Exploratory Data Analysis (EDA)  
- Word frequency distributions  
- Word clouds for visualizing common words  
- Relationship between review length and sentiment  

### 3. Hypothesis Testing  
- Are positive reviews longer than negative ones?  
- Does IMDb rating correlate with review sentiment?  

### 4. Machine Learning  
- Models used: Logistic Regression, Naive Bayes, and Support Vector Machine (SVM)  
- Evaluation metrics: Accuracy, Precision, Recall, and F1-score  

---

## 📈 Expected Results  
- The classifier achieves around **80% accuracy** in predicting review sentiment  
- Positive and negative reviews show distinct linguistic patterns  
- Sentiment polarity generally aligns with IMDb movie ratings  

---

## ⚠️ Limitations and Future Work  
- Dataset is in English, so results may not generalize to other languages  
- Class imbalance (e.g., more positive than negative reviews) may affect model accuracy  
- Future improvements: include Turkish reviews or apply deep learning models such as LSTM or BERT  

---

## 🧰 Technologies Used  
- **Language:** Python 3.11  
- **Libraries:** pandas, numpy, matplotlib, seaborn, scikit-learn, nltk, wordcloud  

---

## 📦 Installation  
To install all dependencies, run the following command in your terminal:

```bash
pip install -r requirements.txt
