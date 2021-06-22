# SHAPING_AI
Code developed during the internship at Sciences Po médialab project 'Shaping 21st Century AI. Controversies and Closure in Media, Policy, and Research'

## Overview
The international project 'Shaping 21st Century AI. Controversies and Closure in Media, Policy, and Research' investigates the development of Artificial Intelligence (AI) as a socio-technical phenomenon. The project’s task aims at detecting criticism and promises around AI in the French media.

## Research Questions 
<li>How is AI presented in the press?
<li>Are there specific epochs of AI discourses?
<li>Can we identify promises and critics? How do they evolve through time? How do they map one on top of the other?

## Data
<li>Source: Europresse database
<li>Media: ≈ 500 national and regional French media in the French language 
<li>Timeline: a period of 10 years (from 2011 to 2021)
<li>Corpus: 47 162 articles after pre-processing
<li>Terms: 8010 unique nouns detected
<li>Network: 3742 nodes and 92956edges

## Objectives 
<li>Mapping the AI discourses and their evolution over time;
<li>Detecting arguments about AI promises and criticisms;
<li>Highlighting the roles of human and technical/calculation objects in AI debates.

## Expected results
Creating text classification model: extraction of the critique and promises corpora, comparison of the terms and topics around them. Epoch detection and visualization of AI discourse timeline.

## Digital Sciences methods
<li>Data: Data wrangling, Time Series, Feature Selection;
<li>Supervised Learning: Text classification, Predictive Modeling, Model Cross-Validation, and Hyperparameter optimization;
<li>Visualization: Interactive graphs, Network analysis;
<li>Text mining: NLP, Terms extraction, Topic Modeling;
<li>Web scraping: Javascript.

## Technical environment
### Programming in Python
#### Working with Data
<li>Pandas, random: Data wrangling and feature engineering, time series transformation, deleting duplicates and missing values, exploratory data analysis <li>Plotly, Seaborn, matplotlib, pyLDAvis: data visualization, timeline word usage, word clouds, LDA 

#### Working with Text
<li>Gensim: topic modeling, LDA model
<li>NLKT: Text cleaning and pre-processing: implementing regular expressions and extended stop-words list
<li>Spacy: advanced Natural Language Processing, lemmatization, tokenization, and entities extraction
<li>Fasttext: supervised text classification

### Additional tools
<li>Web-scraping for Data extraction
<li>Artoo.js - client-side scraping companion and bookmarklet injecting JavaScript code in a web page in order to provide scraping utilities
<li>Data Parsing and Terms Extraction
<li>Cortext - tool to explore and analyze semantics dynamics in the corpus of texts.

#### Visualization
<li>Rawgraphs - tool for scaffolding complex visualizations online
<li>Gephi - an open-source network analysis and visualization software package written in Java on the NetBeans platform
  
## Preliminary results
Extraction of the topics and main terms on all corpora through network mapping, text classification model testing - work in progress.
The network represents the links (co-occurrence in the text) between the terms extracted from all corpora. The node's colors are allocated by the Louvain Method of community detection. Group labels are manually assigned based on the main topic of the words in the community.

   
## Main challenges
<li>Working with big text data: optimization of the analysis, experiment with ram and data pre-processing techniques;
<li>Text data preparation for the analysis: cleaning data using additional stop-words, regular expressions, implementation of the lemmatization.

