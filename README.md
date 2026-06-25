# Steam Games Analysis using NLP and Machine Learning

## Project Overview

This project explores the Steam gaming ecosystem through data collected from the Steam Web API. By combining Natural Language Processing, data visualization, and machine learning techniques, we analyze game descriptions, user reviews, pricing trends, platform support, and player refund behavior.

The objective is to extract meaningful insights from both structured and unstructured data while demonstrating practical applications of data science and machine learning methods.

---

## Dataset

The dataset was created using the Steam Web API and contains information such as:

- Game titles
- Genres
- Prices
- Platform availability
- User reviews
- Playtime statistics
- Review metadata
- Refund-related information

After collection, the data was cleaned and preprocessed to prepare it for analysis and modeling.

---

## Natural Language Processing

### TF-IDF Analysis

Term Frequency-Inverse Document Frequency (TF-IDF) was used to identify the most representative words for different game genres.

This analysis highlights the vocabulary that distinguishes genres and reveals how developers describe their games.

### N-Gram Analysis

Bigram and phrase frequency analysis was performed on user reviews to identify recurring topics and common complaints.

The results indicate that negative reviews are often associated with technical issues, bugs, crashes, and performance problems.

### Part-of-Speech Tagging

Part-of-Speech tagging was applied to game descriptions to examine the adjectives used by developers.

The analysis shows that developers across multiple genres frequently rely on similar descriptive terms to present their games as unique or innovative.

### Sentiment Analysis

Sentiment analysis was performed using:

- VADER Sentiment Analyzer
- AFINN sentiment lexicon

This allowed us to measure the overall positivity and negativity of player reviews and compare sentiment across different games and communities.

---

## Exploratory Data Analysis

Several visualizations were created to investigate relationships within the dataset.

### Price vs. Quality

The relationship between game price and review quality was analyzed.

The results suggest that extremely low-priced games often carry a higher risk of receiving mediocre ratings, although price alone is not a reliable indicator of quality.

### Platform Support

Platform availability was compared across different developer categories.

Interestingly, indie developers were found to provide broader multiplatform support than expected.

### Review Trends

Review distributions and sentiment scores were examined to better understand player satisfaction and community behavior.

---

## Machine Learning

A supervised learning model was developed to predict whether a player refunded a game based on information extracted from their review.

Features included:

- Review sentiment
- Review length
- Playtime
- Number of votes
- Whether the game was received for free

The objective was to determine whether player behavior and review characteristics can be used to predict refund decisions.

Model performance was evaluated using standard classification metrics and confusion matrices.

---

## Technologies Used

- Python
- Pandas
- NumPy
- NLTK
- Scikit-learn
- Plotly
- Matplotlib
- Requests
- BeautifulSoup
- Steam Web API

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/steam-games-analysis.git
cd steam-games-analysis
```

Install the required dependencies:

```bash
pip install pandas numpy nltk scikit-learn plotly matplotlib requests beautifulsoup4 afinn
```

Download the required NLTK resources:

```python
import nltk

nltk.download("punkt")
nltk.download("stopwords")
nltk.download("averaged_perceptron_tagger")
nltk.download("vader_lexicon")
```

---

## Usage

1. Obtain a Steam Web API key.
2. Configure the API key in the notebook.
3. Run the notebook cells sequentially.
4. Generate datasets, visualizations, and machine learning results.
5. Explore the findings presented throughout the analysis.

---

## Key Findings

- Technical problems are among the most common causes of negative reviews.
- Different genres exhibit distinct vocabularies that can be identified through TF-IDF analysis.
- Developers often use similar descriptive language regardless of genre.
- Indie developers frequently offer stronger multiplatform support than larger studios.
- Review sentiment provides useful information for predicting refund behavior.
- Very low-priced games tend to show greater variability in quality and player satisfaction.

---

## Authors

**Emanuel Aenoaei**  
**Julia Căpitănescu**  