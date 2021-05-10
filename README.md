# sentiment_analysis_reddit
An analysis of various applications of the sentiment analysis tool using a Reddit corpus

# Aims of project
The focus of this research is to utilize the natural language processing tool of sentiment analysis in order to assess the attitude and positivity of people’s text for a number of subreddits on Reddit. Sentiment analysis is used to extract a person's opinion and attitude towards a given topic. The results of this analysis is seen as a positive, neutral or negative percentage.

This report will utilise sentiment analysis in a number of different manors. The first use case is to assess the positivity of a series of countries by collecting text data from the specific country’s main subreddits. This positivity results for the post titles will be compared to united nations world happiness report. Further sentiment analysis will be undertaken on the main Irish subreddit r/Ireland to assess the positivity of posts over the last year and identify whether a correlation exists between COVID-19 and the positivity of post titles. A final test will be carried out to assess the attitude held by users of the subreddit r/Ireland towards the four major Irish political parties. 
A brief overview of how sentiment analysis works and the benefits it can bring to a wide number of fields will be discussed below.

# Overview of sentiment analysis
Sentiment analysis (SA) is a continuously growing theme within the area of text mining and natural language processing and information retrieval (Zhang et al., 2018). It can be considered as a method for extracting the subjectivity and sentiment from a corpus. Sentiment analysis is also referred to as opinion mining as it collects information regarding a person's opinion and attitudes for a given topic. The most frequent use of sentiment analysis is to analyse reviews; however, it has also been used to obtain opinions from social media posts and identify the polarity of these opinions (Medhat et al, 2014). The extraction of opinions has far reaching uses as opinions of others have a major impact on our own (Zhang et al., 2018).
The benefits of Sentiment analysis can be seen when it is used for market analysis, identifying potential stock fluctuations and to assess political support (Hutto & Gilbert,  2015). SA can also be used as a cost-effective marketing tool to obtain the opinions of brands based on user’s social media posts, instead of the traditional more expensive tools of surveys or focus groups (Zhang et al., 2018).

# Sentiment Analysis Process 
Sentiment analysis is a classification process involving three parts including the document level, sentence level and aspect level. The document level attempts to classify the entire document as a single entity and identify if the opinion is positive or negative. The sentence level conducts the same process considering each sentence individually. The Sentiment analysis process begins by assessing if the sentence is objective or subjective. A subjective sentence will be analysed by the subject level to assess if the opinion is negative or positive. Finally, the aspect level identifies opinions for individual aspects of entities. This is beneficial as It is possible for a review of a given entity to have a contrasting opinion for various aspects e.g. “The movie was poor overall, but the score was fantastic.”
The data used to train sentiment analysis is of great importance this means that choosing the correct domain data is pertinent to the success of the classification. This may require curating a specific lexicon for different  domains such as review sites where the language would typically be quite formal, or a more informal lexicon may be used for social media posts (Hutto & Gilbert,  2015). 
Feature selection plays an important role in sentiment analysis. A number of feature extraction tools include term frequency, Parts of Speech (POS) tagging, Opinion words/phrases and negation. Term frequency is used to identify how often a word appears in a corpus. POS tagging identifies the adjectives in the sentence to provide an insight into the sentiment of an entity. Opinion words and phrases can simply refer to adjectives such as “poor”, “Okay” and “great” or phrases such as “ I couldn't put this book down”. Negations are used to contradict adjectives such as “not bad”, which would refer to “good”.
Typically, sentiment analysis tools are produced by training both supervised and unsupervised machine learning models, using a sentiment lexicon containing lists of adjectives including both synonyms and antonyms as well as phrases (Medhat et al, 2014).


# Tools used for analysis of sentiment of internet language 
A number of tools were used in this analysis to both collect, process and identify sentiment within the text data.

## Vader Sentiment Analysis lexicon
A vast majority of the data to be analysed by sentiment analysis tools is related to social media, which brings up a series of linguistic issues due to the manner of which people express themselves on social media. These differences can be observed in the use of abbreviations and phrases. Traditional sentiment analysis tools often suffer at classifying the sentiment correctly due to their lack of knowledge on particular domains. 
Valence Aware Dictionary for sEntiment Reasoning (VADER) is a rule-based sentiment analysis tool which is capable of generalising well to a wide variety of domains. Vader is composed of a large sentiment lexicon that focuses on the domains of microblogs, such as Facebook and Twitter. Vader performs especially well  at classifying sentiment of these microblogs and is able to exceed the performance of humans when attempting to assess whether a tweet is positive, negative or neutral (Hutto & Gilbert,  2015).
## NLTK
NLTK, is one of the most prominent natural language processing tools used for the Python programming language. It is composed of a number of natural language processing tools including classification, tokenization, Parts of Speech tagging and stemming. NLTK also contains access to over, 50 inbuilt corpora and lexicon (Nltk.org, 2021).
## Spacy 
 Spacy is another major natural language processing tool that is open source. It focuses on the processing of very large corpora. It is available in over 70 languages and can undertake NLP tasks such as named entity recognition, text classification, lemmatization and dependency parsing. Spacy is focused on the development of software used for production while NLTK is geared towards research and education (Spacy.io, 2021).
## PRAW
Python Reddit API Wrapper (PRAW) is a Python library that can be used to scrape large amounts of text-based content from the Reddit API. PRAW allows access to posts titles and comments. It also collects metadata including the creation date, and number of up votes for each post (Boe, 2021).

# References 
- Boe, B. (2021). praw-dev/praw. [online] Available at: https://github.com/praw-dev/praw [Accessed 25 February 2021].

- Hutto, C.J. & Gilbert, Eric. (2015). VADER: A Parsimonious Rule-based Model for Sentiment Analysis of Social Media Text. Proceedings of the 8th International Conference on Weblogs and Social Media, ICWSM 2014.

- Medhat, W. & Hassan, A. & Korashy, H. (2014)Sentiment analysis algorithms and applications: A survey,Ain Shams Engineering Journal, Volume 5, Issue 4,2014,Pages 1093-1113,ISSN 2090-4479, https://doi.org/10.1016/j.asej.2014.04.011.

- Nltk.org. (2021). Natural Language Toolkit — NLTK 3.5 documentation. [online] Available at: https://www.nltk.org [Accessed 25 February 2021].

- Spacy.io. (2021). Facts & Figures [online] Available at: https://spacy.io/usage/facts-figures [Accessed 25 February 2021].

- Zhang, L. & Wang, S. & Liu, B. (2018). Deep Learning for Sentiment Analysis : A Survey. Wiley Interdisciplinary Reviews: Data Mining and Knowledge Discovery. 8. 10.1002/widm.1253.

