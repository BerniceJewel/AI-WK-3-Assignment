Amazon Reviews Analysis with Sentiment Analysis
This project combines Named Entity Recognition (NER) and Sentiment Analysis on Amazon reviews to extract product names, brands, and analyze review sentiments.

Project Summary
This project analyzes Amazon product reviews using natural language processing techniques to:

Extract and identify products and brands mentioned in reviews
Analyze the sentiment of reviews using a rule-based approach
Generate insights about product and brand perceptions
Visualize sentiment patterns across reviewers
The analysis pipeline includes comprehensive data cleaning, entity recognition, and sentiment analysis, providing valuable insights into customer opinions and product performance.

Project Structure
analyze_reviews_with_sentiment.ipynb - Main notebook with analysis and sentiment analysis
amazon_reviews.csv - Dataset
cleaned_amazon_reviews.csv - Cleaned dataset (generated after running the notebook)
Setup
Install the required dependencies:
pip install spacy pandas matplotlib seaborn
python -m spacy download en_core_web_sm
Make sure you have the amazon_reviews.csv file in your directory.
Features
The notebook includes:

1. Data Cleaning and Preprocessing
Removal of duplicate reviews
Handling of missing values
Text cleaning (lowercase, URL removal, special character removal)
Removal of very short reviews
DateTime conversion
Review length analysis
Data quality statistics
2. Named Entity Recognition
Product name extraction
Brand identification
Entity relationship analysis
Visualization of entity frequencies
3. Sentiment Analysis
Rule-based sentiment scoring
Positive/negative word detection
Negation handling
Sentiment score calculation (-1 to 1)
Sentiment categorization (Positive, Negative, Neutral)
4. Visualization
Entity frequency plots
Sentiment distribution pie chart
Reviewer sentiment analysis
Example reviews for each sentiment category
Data Cleaning Details
The data cleaning process includes:

Duplicate Removal: Ensures each review is unique
Missing Value Handling:
Fills missing reviewer names with 'Anonymous'
Removes rows with missing review text
Text Cleaning:
Converts to lowercase
Removes URLs and special characters
Removes numbers
Trims whitespace
Quality Filters:
Removes very short reviews (< 10 characters)
Feature Engineering:
Adds review length analysis
Converts timestamps to datetime format
Output
The notebook generates:

Cleaned dataset (cleaned_amazon_reviews.csv)
Distribution of review sentiments
Example reviews for each sentiment category
Reviewer-level sentiment analysis
Visualizations of sentiment distribution
Dependencies
Python 3.x
pandas
spacy
matplotlib
seaborn
re (built-in)
datetime (built-in)
collections (built-in)
