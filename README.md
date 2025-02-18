# DSproject
The purpose of this project is to understand the relationship between Elon Musk's tweet sentiments and Tesla's stock price. Below is documentation for reproducability. 

## Software and Platform
This project used Python programming through Jupyter Notebook on Windows platform.

Required imports and libraries:
```
!pip install pyspellchecker
!pip install scattertext
!pip install nltk
!pip install -U kaleido

# Import Data Preprocessing and Wrangling libraries
import re
from tqdm.notebook import tqdm
import pandas as pd
import numpy as np
from datetime import datetime
import dateutil.parser

# Import NLP Libraries
import nltk
from spellchecker import SpellChecker
from nltk.sentiment.vader import SentimentIntensityAnalyzer as SIA

# Import Visualization Libraries
import plotly.offline as pyo
import plotly.express as px
import plotly.io as pio
import plotly.graph_objects as go
import matplotlib.pyplot as plt
from plotly.subplots import make_subplots
import seaborn as sns
import scattertext as st
from IPython.display import IFrame
from wordcloud import WordCloud, ImageColorGenerator
import matplotlib.pyplot as plt
from nltk.corpus import stopwords
import random
```

## Documentation
- LISCENCE.MD: proper citation for repository
- SCRIPTS folder: source code for project (for tweets, stock price, and analysis data)
- DATA folder: initial and combined data from tweets and stock price dataset
- OUTPUT: figures and tables generated from scripts
- REFERENCES: sources used throughout project

## Reproducing results
SCRIPTS:

1.Tweet_Sentiment_Analysis_&_EDA: Read in Musk tweets dataset imported from Kaggle and perform sentiment analysis and EDA. 

Output = new dataframe (Tweet Sentiment Data.csv), EDA graphs

2.Stock_Price_EDA: Read in Tesla stock prices from yfinance over same period of time as twitter dataset, and perform EDA.

Output = new dataframe (Tesla Stock.csv), EDA graphs

3.Data Analysis: This re-reads in Musk tweets and Tesla stock price dataframes, 1)processes and merges data into 1 dataframe (Merged Data.csv), 2)process merged dataframe for time-series analysis so both sets of data are stationary, and 3)performes multiple statistical analysis' to test relationship between sentiment of Musk's tweets and Tesla stock prices.

Output = new dataframe (Merged Data.csv), and statistical summaries of each test
