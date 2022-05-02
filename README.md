# HEB_google_maps_reviews
Python workflow to get common words and phrases from negative H-E-B store reviews

### Necessary Packages
import pandas as pd
import nltk
from collections import Counter
from nltk.corpus import stopwords
from nltk.collocations import *

# Define a function for generating cleanesed data frame from google maps review .csv
.csv files obtained from Outscraper tool, but can be done entirely in python if necessary. The Outscraper tool was used for the sake of saving time. See the link below.
https://app.outscraper.com/googleReviews

### Function applied to Dripping Springs and Waxahachie H-E-B stores

# Define function for generating common words list.
This function will generate a list of the most common words (ommiting stopwords) with a word count. 
Apply this function to the dataframes for each H-E-B store.

# Summary & Conclusions
The workflow above reads a .csv of google maps store reviews into a dataframe with the columns: date of review, review author, review text, and review rating (stars). A function is then applied to that new dataframe to get the most common words (ommiting stopwords) for a more efficient analysis of the review text.
