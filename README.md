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
- SCRIPTS.ipynb: source code for project
- DATA.csv: initial and analyzed data
- OUTPUT: figures and tables generated from scripts
- REFERENCES: sources used throughout project

## Reproducing results
