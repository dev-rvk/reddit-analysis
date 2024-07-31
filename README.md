# Indepth analysis of `r/subredditoftheday`

Dataset: [link](https://www.kaggle.com/code/mathurinache/sub-reddit-of-the-day-posts-analysis/input)

This project aims to analyze the sentiment of comments on various subreddits featured in "Subreddit of the Day."

## Method

1. Data Collection: Extracted data from the "Subreddit of the Day" posts.
Focused on comments across various subreddits.

2. Data Cleaning: Removed missing values from the dataset.
Extracted subreddit names from titles using regular expressions.

3. Sentiment Analysis: 
   - Used TextBlob to calculate sentiment polarity for each comment.
   - Classified sentiments into three categories: Positive, Neutral, and Negative based on polarity scores:
   - Positive: Polarity > 0.1
Neutral: -0.1 <= Polarity <= 0.1
Negative: Polarity < -0.1
Data Visualization:

Visualized the distribution of sentiment categories using bar plots.

## Findings

1. **Sentiment analysis of comments**: The majority of comments across the analyzed subreddits have a positive sentiment followed by neutral.

2. **Plotting Sentiments of sub-reddits on the basis of score**:
  The most number of Positive comments are in medium range of score (upvotes) followed by low range.

3. **Finding correlation between Score and Sentiment**: Correlation between sentiment and score: -0.07 i.e -ve means that positive comments tend to have lower score.

    Potential Reasons:
   - **Engagement with Criticism**: Users might find critical comments more engaging, leading to more upvotes.
   - **Issue Highlighting**: Negative comments may highlight issues or problems more effectively, leading to more upvotes.

4. **Top Subreddit Based on Engaggement**: 
    ```plaintext                       
    subreddit                       EngagementScore                       
    /r/FragileWhiteRedditor          0.445013
    /r/wallstreetbets                0.444708
    /r/Dota2                         0.334715
    /r/ThanosDidNothingWrong         0.294853
    /r/Pokemon                       0.289744
    ```

5. **Performed Analysis of top words used in the top 10 most commented posts**  
6. **Performed analysis of Posting Patterns as per Month (over a span of a year)**
