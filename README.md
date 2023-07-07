# Sentiment-Analysis
 sentiment analysis using the VADER (Valence Aware Dictionary and Sentiment Reasoner) sentiment analysis tool from the Natural Language Toolkit (NLTK) library in Python. 
The NLTK library is imported, and the VADER lexicon is downloaded using nltk.download('vader_lexicon'). The VADER lexicon is a pre-trained sentiment analysis model included in NLTK.

The SentimentIntensityAnalyzer class from the nltk.sentiment module is imported. This class provides the functionality for sentiment analysis using the VADER model.

The SentimentIntensityAnalyzer object sia is initialized.

A list called reviews is defined, containing example product reviews. These reviews represent the input for sentiment analysis.

A for loop iterates over each review in the reviews list.

Within the loop, the polarity_scores() method of the SentimentIntensityAnalyzer object is used to calculate the sentiment scores for each review. The polarity_scores() method returns a dictionary containing four values: neg (negative), neu (neutral), pos (positive), and compound (compound sentiment score).

The sentiment scores are interpreted to determine the overall sentiment of each review. If the compound score is greater than or equal to 0.05, the sentiment is classified as 'Positive'. If the compound score is less than or equal to -0.05, the sentiment is classified as 'Negative'. Otherwise, it is classified as 'Neutral'.

The review text and the assigned sentiment label are printed using print() statements. The sentiment label is either 'Positive', 'Negative', or 'Neutral' based on the compound score.
