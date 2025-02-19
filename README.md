# Twitter Airline Sentiment Analysis

## Project Overview
This project analyzes Twitter data to assess airline sentiment, identify the most common negative reasons for complaints, and compare sentiment trends across six major airlines. The dataset is sourced from Kaggle and consists of tweets from 2015 related to airline experiences. The analysis leverages R for data cleaning, visualization, and sentiment assessment.

## Objectives
1. Determine the main reasons for negative tweets.
2. Identify the airline with the worst rating for each negative reason.
3. Evaluate the overall sentiment (positive, negative, neutral) for each airline.
4. Find the top three negative reasons for each airline.
5. Analyze tweet frequency per airline.
6. Examine retweet patterns and their connection to negative sentiment.
7. Assess the correlation between tweet length and sentiment.

## Dataset
### Variables Kept
- **Airline**: Name of the airline.
- **Airline_sentiment**: Sentiment classification (Positive, Negative, Neutral).
- **Airline_sentiment_confidence**: Confidence level in sentiment classification.
- **Negativereason**: The main complaint for negative sentiment tweets.
- **Negativereason_confidence**: Confidence level in negative reason classification.
- **Retweet_count**: Number of retweets.
- **Text**: The tweet content.

### Variables Removed
- **Tweet_id**: Twitter user ID.
- **Airline_sentiment_gold & Negativereason_gold**: No data provided.
- **Tweet_coord, User_timezone, Tweet_location**: Inconsistent or irrelevant data.
- **Name**: Twitter user name.
- **Tweet_created**: Date/time of tweet posting (not necessary for analysis).

## Methodology
1. **Data Cleaning**:
   - Removed unnecessary variables.
   - Dropped N/A values in key columns.
   - Standardized column values (e.g., formatting text strings).

2. **Sentiment Analysis**:
   - Computed mean sentiment confidence scores per airline.
   - Identified airlines with the highest positive, neutral, and negative sentiment.

3. **Negative Reason Analysis**:
   - Examined the most frequent negative reasons.
   - Ranked airlines based on the worst-rated negative reasons.
   - Determined the top three negative reasons per airline.

4. **Visualization**:
   - **Tweet Volume Analysis**: Bar plots of tweet frequency per airline.
   - **Sentiment Breakdown**: Visualizing positive, neutral, and negative sentiment per airline.
   - **Negative Reason Trends**: Facet-wrapped bar graphs to show distribution per airline.
   - **Retweet Analysis**: Evaluating the most retweeted negative reasons.
   - **Text Length vs. Sentiment**: Density plots to check correlation between text length and sentiment.

## Key Findings
- **Most Negative Airline**: US Airways (highest mean negative sentiment confidence: 0.946).
- **Most Neutral Airline**: United (highest mean neutral sentiment confidence: 0.810).
- **Most Positive Airline**: Virgin America (highest mean positive sentiment confidence: 0.946).
- **Most Common Negative Reason**: "Customer Service Issues" (31.7% of negative tweets).
- **Most Frequent Airline in Tweets**: United Airlines (3,822 tweets).
- **Least Frequent Airline in Tweets**: Virgin America (504 tweets).
- **Top Negative Reasons by Airline**:
  - **American**: Customer Service Issues (40.1%)
  - **Delta**: Late Flight (28.2%)
  - **Southwest**: Customer Service Issues (33%)
  - **United**: Customer Service Issues (25.9%)
  - **US Airways**: Customer Service Issues (35.8%)
  - **Virgin America**: Customer Service Issues (33.1%)
- **Retweet Trends**:
  - 95% of tweets were not retweeted.
  - "Customer Service Issues" and "Can’t Tell" were the top reasons for retweets (~25%).
- **Text Length vs. Sentiment**:
  - Longer tweets were more likely to have negative sentiment.
  - Shorter tweets were more likely neutral or positive.

## Recommendations
1. **American Airlines**: Improve customer service (40.1% of complaints).
2. **Delta Airlines**: Reduce flight delays (28.2% of complaints).
3. **Southwest Airlines**: Enhance customer service (33% of complaints).
4. **United Airlines**: Address customer service issues (25.9% of complaints).
5. **US Airways**: Improve customer service experience (35.8% of complaints).
6. **Virgin America**: Improve flight booking and customer service.

## Tools & Resources
- **Programming Language**: R (ggplot2, dplyr)
- **Data Source**: Kaggle (Twitter Airline Sentiment Dataset)
- **References**:
  - Data visualization techniques with ggplot2.
  - R programming tutorials on sentiment analysis.
  - Kaggle discussions on Twitter sentiment analysis.

## Contributors
- **Author**: Mira Wadehra
- **Professor**: Houldsworth (MGSC-410-01)

## License
This project is for educational and analytical purposes. The dataset and code are shared under the respective terms of Kaggle and R open-source licensing.

