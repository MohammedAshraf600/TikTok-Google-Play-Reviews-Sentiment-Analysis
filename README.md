# 📱 TikTok Google Play Reviews – Sentiment Analysis

## 📌 Project Overview
This project performs **sentiment analysis on TikTok reviews from Google Play Store** using **Natural Language Processing (NLP)** techniques.  
The workflow includes **data cleaning, text preprocessing, visualization, and sentiment scoring** to understand user opinions and overall sentiment trends.

---

## 🎯 Objectives
- Analyze user reviews of the TikTok app
- Clean and preprocess raw text data
- Visualize review distributions and frequent words
- Perform sentiment analysis (Positive / Negative / Neutral)
- Identify the dominant sentiment in user reviews

---

## 📂 Dataset
**Source:** Google Play Store Reviews  
**File:** `tiktok_google_play_reviews.csv`

### Selected Columns
| Column | Description |
|------|------------|
| content | User review text |
| score | Rating (1–5 stars) |

---

## 🧹 Data Preprocessing
- Removed unnecessary columns
- Dropped null values from `content`
- Converted text to lowercase
- Removed:
  - URLs
  - HTML tags
  - Punctuation
  - Numbers
  - Stopwords
- Applied **Porter Stemming**
  - Example:  
    - `running → run`  
    - `beautifully → beauti`

---

## 🧠 Text Cleaning Pipeline
Steps applied to each review:
1. Lowercasing
2. Regex-based cleaning
3. Stopword removal
4. Tokenization
5. Stemming
6. Rejoining cleaned tokens

---

## 📊 Exploratory Data Analysis (EDA)

### ⭐ Rating Distribution
- Visualized using an **interactive pie chart**
- Shows user rating behavior (1–5 stars)

### ☁️ Word Clouds
Generated word clouds for:
- All reviews
- Positive reviews
- Negative reviews  

These visualizations highlight the most frequent terms used by users.

---

## 😊 Sentiment Analysis
Used **NLTK – VADER SentimentIntensityAnalyzer** to extract:
- Positive score
- Negative score
- Neutral score

### Sentiment Features
| Feature | Description |
|------|------------|
| positive | Positive sentiment score |
| negative | Negative sentiment score |
| neutral | Neutral sentiment score |

---

## 📈 Overall Sentiment Results
**Aggregated sentiment scores:**
- **Positive:** 196,353
- **Negative:** 16,512
- **Neutral:** 244,169

### ✅ Final Conclusion
> **Neutral sentiment is dominant**, indicating that most users provide informational or emotion-neutral feedback rather than strong opinions.

---

## 🛠️ Tools & Libraries
- Python
- Pandas
- Matplotlib
- Plotly
- NLTK
- WordCloud
- Regular Expressions (re)
