 Web Scrape Sentiment Analysis using VADER
This project performs **sentiment analysis** on a dataset of social media posts, using the **VADER Sentiment Analysis** tool. The dataset is processed in **Python** with the help of `pandas` for data handling and `vaderSentiment` for sentiment analysis. The final dataset includes the original data with an additional column indicating the sentiment (Positive, Neutral, Negative) of each post based on its text content.

 Project Overview

1. Load Data: The dataset is loaded from a CSV file containing web-scraped data with post text.
2. Sentiment Analysis: VADER sentiment analysis is applied to the `text` column of the dataset to determine the sentiment of each post.
3. Save Results: The sentiment values are added as a new column and saved to a new CSV file.

 Dependencies

- pandas: For data manipulation and reading/writing CSV files.
- VADER SentimentIntensityAnalyzer**: For sentiment analysis, which is part of the `vaderSentiment` library.
  *textblob (optional): Used initially, though `VADER` is primarily used in this project.

You need to have Python installed on your system. 
The following Python packages are required:

1. **pandas**:
   ```bash
   pip install pandas
   The input file WEB SCRAPE.csv should contain a text column with social media post content.
   The processed output is saved as WEB SCRAPE_with_vader_sentiment.csv, with an additional Sentiment column indicating the sentiment of each post (Positive, Neutral, Negative)
   VADER (Valence Aware Dictionary and Sentiment Reasoner) is a tool specifically designed to handle sentiment analysis for social media text. It takes into account the intensity of positive and negative emotions, as well as neutral sentiment.
The compound score is used to categorize the sentiment:
Positive: Compound score >= 0.05
Negative: Compound score <= -0.05
Neutral: Compound score between -0.05 and 0.05
