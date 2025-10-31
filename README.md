# Movie Reviews Sentiment Analysis

## Overview

This project explores how natural language processing (NLP) techniques can be applied to classify movie reviews based on sentiment.  
The main objective is to develop a model that automatically distinguishes between **positive**, **negative**, and **neutral** opinions expressed in text reviews.  

By analyzing a large dataset of user-generated movie reviews, this study seeks to understand how textual patterns, word choices, and tone reflect emotional attitudes toward films.

---

## Motivation

Millions of online users share their opinions about movies every day.  
These reviews influence audience decisions and provide valuable insights into collective perceptions of storytelling, performance, and direction.  

Through sentiment analysis, we can uncover linguistic trends associated with satisfaction or disappointment and visualize how viewers’ opinions vary across different genres or release periods.

---

## Data Sources

### IMDb Movie Reviews Dataset
- **Source:** [IMDb Dataset on Kaggle](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews)  
- **Content:** 50,000 labeled reviews (balanced between positive and negative)  
- **Structure:** Two columns — `review` (text) and `sentiment` (label)  
- **Purpose:** Primary dataset for model training and evaluation  

### TMDB Metadata Enrichment
- **Source:** [TMDB Open API](https://developer.themoviedb.org/reference/intro/getting-started)  
- **Additional Variables:** Genre, release year, and user rating  
- **Purpose:** To explore how movie characteristics correlate with audience sentiment  

---

## Methodology

### Data Preparation
1. Load IMDb data and clean text by removing punctuation, HTML tags, and special symbols.  
2. Tokenize and lemmatize text using [NLTK](https://www.nltk.org/).  
3. Merge movie metadata obtained from TMDB API.  
4. Encode sentiment labels for machine learning processing.  

### Exploratory Data Analysis
- Visualize most frequent words using word clouds.  
- Compare sentiment ratios by movie genre and release decade.  
- Explore relationships between average ratings and sentiment.  

### Modeling
- Apply multiple classification algorithms:
  - Logistic Regression  
  - Random Forest  
  - Support Vector Machine (SVM)  
- Evaluate model performance with accuracy, F1-score, and confusion matrices.  
- Optionally, experiment with a recurrent neural network (LSTM) for deeper text understanding.  

---

## Tools and Libraries

- **Python** — primary programming language  
- **Pandas, NumPy** — data manipulation and transformation  
- **NLTK, Scikit-learn** — NLP preprocessing and model training  
- **Matplotlib, Seaborn** — visualization of results  
- **Jupyter Notebook** — workflow documentation and reproducibility  

---

## Expected Outcomes

- A functional text classification model that predicts the polarity of a review.  
- Insights into linguistic and stylistic patterns typical of positive and negative feedback.  
- Comparative analysis of how movie characteristics (genre, release year) relate to sentiment.  
- Visual summaries demonstrating sentiment distribution and model accuracy.

---

## Limitations

- Text ambiguity (sarcasm or irony) may reduce classification accuracy.  
- Possible overfitting due to limited vocabulary diversity.  
- Computational complexity of deep learning methods for large-scale text data.  

---

## Ethical Considerations

All datasets used in this project are **publicly accessible** and contain **no personal information**.  
The analysis is limited to movie reviews and metadata for educational and research purposes.

---

## AI Usage Statement

Portions of this README and the initial project outline were generated with assistance from ChatGPT (GPT-5).  
The tool was used exclusively to improve the clarity, grammar, and organization of the text.  

All analytical decisions, dataset selection, and final wording were completed and verified by the author.  
The use of AI was limited to language support and did not involve automated code or data generation.  

This declaration is made to ensure full transparency and compliance with the course’s academic integrity policy.


---

## References

- [IMDb Movie Reviews Dataset on Kaggle](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews)  
- [TMDB API Documentation](https://developer.themoviedb.org/reference/intro/getting-started)  
- [NLTK Official Documentation](https://www.nltk.org/)  
- [Scikit-learn Documentation](https://scikit-learn.org/stable/)  
