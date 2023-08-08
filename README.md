# Sentiment Analysis of Tweets Directed at @Apple Before and After Quarterly Results

This project performs sentiment analysis on tweets directed at Apple before and after its quarterly results announcement. It aims to explore how sentiment changed before and after the announcement, providing insights into public perceptions.

## Prerequisites

Make sure you have the required R packages installed:

- `tm` for text mining and preprocessing
- `syuzhet` for sentiment analysis
- `lubridate` for handling dates
- `ggplot2`, `scales`, `reshape2`, and `dplyr` for data visualization

## Data Preparation

1. Import the tweet data for Apple before its quarterly results from the 'apple_pre_earnings.csv' CSV file.
2. Change the character encoding of the text column to UTF-8 for proper text processing.
3. Convert the data into a corpus using the `tm` package to enable text mining operations.

## Data Cleaning

1. Convert all text to lowercase using `tm_map`.
2. Remove punctuation, numbers, and common English stopwords.
3. Remove URLs, mentions, and specific words like 'aapl' and 'apple'.
4. Replace 'stocks' with 'stock' to avoid double counting.
5. Strip extra whitespace from the text.

## Term-Document Matrix (TDM)

1. Convert the cleaned corpus into a Term-Document Matrix (TDM) to analyze word frequencies.
2. Display the first 10 words from the TDM for a quick overview.

## Bar Plot and Word Cloud

1. Generate a bar plot of word frequencies to visualize the most frequent words.
2. Filter out words with a frequency less than 25 to focus on significant words.
3. Create a word cloud for a visually appealing representation of word frequencies.

## Sentiment Analysis

1. Import the tweet data for Apple after its quarterly results from the 'apple_post_earnings.csv' CSV file.
2. Perform sentiment analysis using the `syuzhet` package to obtain sentiment scores.
3. Plot a bar plot of sentiment scores for tweets directed at Apple before the announcement.
4. Plot a bar plot of sentiment scores for tweets directed at Apple after the announcement.

## Conclusion

This analysis reveals that after Apple published its quarterly earnings, there was a decrease in negative emotions and an increase in positive emotions in the tweets directed at Apple.

## Instructions

1. Ensure the required CSV files are in the same directory as the R script.
2. Install the necessary R packages using `install.packages(c("tm", "syuzhet", "lubridate", "ggplot2", "scales", "reshape2", "dplyr"))`.
3. Run the R script step by step to perform the analysis.

Feel free to modify the code and adapt the analysis to suit your needs.

---

*Note: This project is for educational purposes and provides a general overview. Real-world analysis might require additional considerations.*
