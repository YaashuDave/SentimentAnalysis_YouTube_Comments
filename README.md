
# SentimentAnalysis_YouTube_Comments
Automated sentiment analysis system using NLP, web scraping, YouTube API, and Hugging Face. Classifies user comments into positive, negative, or neutral, empowering businesses and content creators with valuable insights for informed decisions, improved satisfaction, and enhanced engagement.

# Overview
This project conducts sentiment analysis on YouTube comments for a specific video using three Python packages: "Vader Lexicon Sentiment Analyser,"  and the "Roberto model" from Hugging Face Transformers. The analysis provides insights into the sentiments expressed by users, utilizing the YouTube Data API for comment retrieval.

# How it works
1)YouTube Data API: Scrapes comments from a targeted video using the YouTube Data API available on the Google Developers Console.<br>
2)NLTK Library: Implements the Natural Language Toolkit (NLTK) for sentiment analysis.<br>
3)VADER Lexicon: Utilizes VADER, a lexicon and rule-based sentiment analysis tool tailored for social media expressions.<br>
4)Hugging Face Transformers - Roberto Model: Incorporates the Roberto model for advanced sentiment analysis using transformer-based techniques.<br>

# Scoring for Vader model
The sentiment analysis involves assigning compound scores to words, with labels determined by specific relations for VADER. The Roberto model leverages transformer-based techniques for a nuanced understanding of sentiments. This is done as Vader Model is not that accurate as compared to Roberto. Vader Model cannot understand sarcasm.<br><br>
Weakly Positive sentiment: compound score <= 0.3<br>
Positive sentiment: compound score >= 0.3 and <= 0.6<br>
Strongly Positive sentiment: compound score >= 0.6<br>
Neutral sentiment: compound score = 0<br>
Weakly Negative sentiment: compound score <= 0 and > -0.3<br>
Negative sentiment: compound score <= -0.3 and > -0.6<br>
Strongly Negative sentiment: compound score <= -0.6<br>

# Scoring for Roberto model
For Roberto Model it is Normal Scoring that is positive, negative and neutral as it is very accurate.

# Usage
1)Clone the repository.<br>
2)Install the required packages(already written in notebook).<br>
3)Obtain API credentials from the Google Developers Console for YouTube Data API.<br>
4)Replace the placeholder API key in the code with your credentials and replace videoid=" " with any url of YouTube video.<br>
5)Run the script to perform sentiment analysis on YouTube comments.<br>

# Outputs by Vader:
![output1](https://github.com/YaashuDave/SentimentAnalysis_YouTube_Comments/assets/107920191/1e019008-7a06-4fe8-b9d1-acc9ed066ff3) <br>
![output2](https://github.com/YaashuDave/SentimentAnalysis_YouTube_Comments/assets/107920191/fb6ed6d4-d894-4ce4-8515-35afcd9d99cc)
![output3](https://github.com/YaashuDave/SentimentAnalysis_YouTube_Comments/assets/107920191/25c6f310-34f0-4cca-98ea-e80c00321b80)
![output4](https://github.com/YaashuDave/SentimentAnalysis_YouTube_Comments/assets/107920191/e41b9732-5ab5-48c9-af82-6f3af7fbeb0f)
![output5](https://github.com/YaashuDave/SentimentAnalysis_YouTube_Comments/assets/107920191/ca548862-b964-4f1d-ae45-2f3259a77883)

# Outputs by Roberto:
![output6](https://github.com/YaashuDave/SentimentAnalysis_YouTube_Comments/assets/107920191/0f97d58c-9fe3-46c3-a82e-6feda2811449)
![output7](https://github.com/YaashuDave/SentimentAnalysis_YouTube_Comments/assets/107920191/586dbb51-262b-4df3-9f2f-66f0c24bcaeb)
![output8](https://github.com/YaashuDave/SentimentAnalysis_YouTube_Comments/assets/107920191/38362b02-d147-41ad-bf81-0f22f77586ec)

# Contributer
  YAASHU DAVE
