# Sentiment Analysis on Social Media Data using NLTK Vader

## 📌 Overview

This project performs **sentiment analysis** on social media data using **NLTK's Vader (Valence Aware Dictionary and sEntiment Reasoner)**. The goal is to classify text into **positive, negative, or neutral sentiment** by leveraging Vader's lexicon-based approach.

## 🚀 Features

- **Preprocessing**: Cleans raw social media text (removes URLs, mentions, hashtags, and special characters).
- **Sentiment Scoring**: Uses Vader's `SentimentIntensityAnalyzer` to classify sentiments.
- **Data Visualization**: Displays sentiment distribution through plots.
- **Custom Analysis**: Allows users to input their own text for sentiment evaluation.

## 🛠️ Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/sentiment-analysis-nltk.git
   cd sentiment-analysis-nltk
   ```

## 📂 Dataset

- You can use **Twitter API, Facebook API, or any dataset** containing social media comments.
- Example datasets: Kaggle's **Twitter Sentiment Analysis** dataset.

## 🏗️ Usage

1. **Run the script**:
   ```bash
   python sentiment_analysis.py
   ```
2. **Test with custom input**:
   ```python
   from vaderSentiment.vaderSentiment import SentimentIntensityAnalyzer

   analyzer = SentimentIntensityAnalyzer()
   text = "I love this product! It's amazing."
   sentiment_score = analyzer.polarity_scores(text)
   print(sentiment_score)
   ```

## 📊 Sample Output

Example of Vader's sentiment score:

```json
{'neg': 0.0, 'neu': 0.3, 'pos': 0.7, 'compound': 0.85}
```

- `compound` score determines final sentiment:
  - **Positive**: `compound > 0.05`
  - **Neutral**: `-0.05 <= compound <= 0.05`
  - **Negative**: `compound < -0.05`

## 📈 Visualization

- The script provides bar charts and pie charts for sentiment distribution using **Matplotlib & Seaborn**.

## 📜 Dependencies

- Python 3.x
- `nltk`
- `vaderSentiment`
- `pandas`
- `matplotlib`
- `seaborn`

## 🤝 Contribution

Feel free to **fork** this repository, submit issues, or create pull requests!

## 🔗 Connect

- LinkedIn: Sundaresan C ([https://www.linkedin.com/in/sundaresan-c-55991b236/])
- GitHub: Sundaresan C ([https://github.com/SundaresanC])

