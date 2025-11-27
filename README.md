# Movie Dataset Analysis Project

## Overview
This project performs exploratory data analysis (EDA) and statistical hypothesis testing on the IMDb 5000 Movie Dataset. The goal is to identify patterns and relationships among movie-level variables such as IMDb score, budget, gross revenue, release year, and genre. This document represents the deliverable for **Milestone 1 (28 November)**. Machine learning, sentiment analysis, and metadata enrichment will be implemented in future milestones.

## Dataset
Source: Kaggle — IMDB 5000 Movie Dataset  
File used: `movie_metadata.csv`

Main columns used:
- movie_title  
- genres  
- title_year  
- budget  
- gross  
- imdb_score  

Note: Only movie-level metadata is used at this stage. Review-level sentiment data and TMDB enrichment will be added later.

## Project Structure
```
project-root/
│
├── data/
│   └── movie_metadata.csv
│
├── analysis/
│   └── eda_hypothesis_tests.ipynb  (or .py)
│
├── requirements.txt
└── README.md
```
## Analysis Notebook
You can view the full exploratory data analysis and hypothesis testing here:  
[EDA & Hypothesis Testing Notebook](analysis/eda_hypothesis_tests.ipynb)

## Setup & How to Run

### 1. Clone this repository
```bash
git clone https://github.com/EfeImrek/movie-sentiment-analysis.git
cd movie-sentiment-analysis
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Run the analysis
If using a Python script:
```bash
python analysis/eda_hypothesis_tests.py
```

If using Jupyter Notebook or Google Colab:
- Open `analysis/eda_hypothesis_tests.ipynb`
- Run all cells

## Exploratory Data Analysis (EDA)

The following analyses were conducted:

### IMDb Score Distribution
A histogram was plotted to observe how IMDb scores are distributed across the dataset.

### Budget Distribution
Budgets show heavy right skew with a long tail of extremely high-budget productions.

### Budget vs Gross Revenue
A scatterplot was used to examine whether higher budgets correlate with higher revenue.

### Number of Films per Year
A count plot was generated to detect trends in film production over the years.

### Genre Analysis
Genres were extracted from the `genres` column by taking the first listed genre (main_genre).  
A bar chart shows the distribution of main genres.

### Average IMDb Score by Genre
Mean IMDb scores were computed for each main genre.

### Correlation Heatmap
A heatmap of correlations among numerical variables (IMDb score, budget, gross, title_year) was generated.

## Hypothesis Testing

Three two-sample t-tests were conducted:

### H1 — Drama vs Action IMDb Scores
- **H0:** Mean IMDb scores are equal.  
- **H1:** Mean IMDb scores differ.  
- **Method:** Welch's t-test  
- **Result:** *(Insert your p-value)*  
- **Interpretation:** *(Reject / fail to reject H0)*  

### H2 — Pre-2000 vs Post-2000 IMDb Scores
- Films released before and after the year 2000 were compared.  
- **Result:** *(Insert p-value)*  
- **Interpretation:** *(Reject / fail to reject H0)*  

### H3 — High-Budget vs Low-Budget IMDb Scores
- The median budget was used as the threshold.  
- **Result:** *(Insert p-value)*  
- **Interpretation:** *(Reject / fail to reject H0)*  

## Key Findings Summary
- The most frequent primary genres are *(insert)*.  
- Budget and gross revenue show a positive but noisy correlation.  
- Depending on hypothesis outcomes, some genre or time-period groups may have significantly different IMDb scores.

(Replace placeholders with values from your outputs.)

## Limitations
- The dataset may include missing or inaccurate budget/gross values.  
- Genre information may include multiple genres; only the first was used as the primary genre.  
- Sentiment analysis and TMDB metadata are not yet included.

## Future Work
- Review-level sentiment analysis (IMDB 50K Dataset)  
- Metadata enrichment using the TMDB API  
- Regression or classification models (predict revenue or score)  
- Feature engineering and model tuning  
- Bias and fairness evaluation for ML models  

## Author
**Efe İmrek**  
GitHub: https://github.com/EfeImrek
