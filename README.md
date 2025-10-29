# Movie-Reviews-Sentiment-Analysis

## *Project Idea*

This project aims to analyze public movie reviews and determine whether the sentiment expressed in each review is **positive**, **negative**, or **neutral**.  
The main hypothesis is that textual patterns in user-generated reviews can accurately predict the sentiment of a viewer’s experience.  

By applying **Natural Language Processing (NLP)** techniques to a large corpus of movie reviews, the study explores how linguistic features such as word frequency, emotion-related terms, and sentence structure influence sentiment classification.

---

## *Description of Dataset*

The project will utilize a publicly available dataset and additional metadata:

### *IMDb Movie Reviews Dataset*  
- **Source:** [IMDb Dataset on Kaggle](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews)  
- **Size:** 50,000 labeled movie reviews (balanced: 25k positive, 25k negative)  
- **Format:** CSV file containing two columns — *review* (text) and *sentiment* (label)  
- **Purpose:** Base dataset for training and testing the sentiment classification model  

### *Enrichment Dataset (Movie Metadata)*  
- **Source:** [TMDB Open API](https://developer.themoviedb.org/reference/intro/getting-started)  
- **Features Added:** Movie genre, release year, and average audience rating  
- **Purpose:** To analyze whether external factors such as genre or release period correlate with sentiment polarity  

---

## *Plan*

### *Data Collection*
- Import IMDb dataset from Kaggle.  
- Use TMDB API to retrieve metadata for corresponding films.  
- Merge the two datasets on movie title and release year.  

### *Data Preprocessing*
- Clean the text (remove punctuation, stopwords, and special characters).  
- Apply tokenization and lemmatization using NLTK.  
- Encode sentiment labels numerically for model training.  

### *Exploratory Data Analysis (EDA)*
- Visualize word frequency distributions using word clouds.  
- Examine sentiment proportions by genre and release year.  
- Compute correlations between ratings and review sentiment.  

### *Modeling*
- Apply machine learning methods for classification:  
  - Logistic Regression  
  - Support Vector Machines (SVM)  
  - Random Forest  
- Evaluate models using accuracy, precision, recall, and F1 score.  
- Optionally, test deep learning models (e.g., LSTM).  

### *Visualization and Presentation*
- Plot confusion matrices for model comparisons.  
- Visualize average sentiment by movie genre.  
- Present insights on patterns found in emotional language.  

---

## *Tools and Technologies*
- **Python** – Core language for data analysis  
- **Pandas & NumPy** – Data handling and preprocessing  
- **NLTK & Scikit-learn** – NLP and machine learning  
- **Matplotlib & Seaborn** – Visualization  
- **Jupyter Notebooks** – Documentation and reproducibility  

---

## *Expected Outcomes*
- A machine learning model capable of classifying movie reviews by sentiment  
- Identification of key linguistic features linked with positive or negative opinions  
- Insights into how genre or release year influences audience reactions  
- Visual tools summarizing sentiment trends across thousands of reviews  

---

## *Potential Challenges*
- Ambiguity in review language (e.g., sarcasm or mixed emotions)  
- Balancing data and avoiding overfitting  
- Handling long and unstructured text  
- Computational cost of deep learning models on large text data  

---

## *Ethical Considerations*
- All data sources are publicly available and anonymized.  
- No personal or sensitive user data is included.  
- Project follows ethical guidelines for data collection and AI usage.  

---

## *AI Usage Statement*
Parts of this README and project plan were prepared with assistance from **ChatGPT (GPT-5)**.  
All generated content was reviewed, verified, and edited by the author to ensure academic integrity and compliance with course requirements.

---

## *References*
- [IMDb Dataset on Kaggle](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews)  
- [TMDB Open API](https://developer.themoviedb.org/reference/intro/getting-started)  
- [NLTK Documentation](https://www.nltk.org/)  
- [Scikit-learn Documentation](https://scikit-learn.org/stable/)  
