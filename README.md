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

## Technical environment
<li>Data extraction: Web Scraping (Javascript), Data Parsing (Cortext);
<li>Data Wrangling: Time Series, Feature Engineering, deleting duplicates and missing values;
<li>Text Mining: Text cleaning and pre-processing (NLKT), implementing regular expressions and extended stop-words list, NLP (Spacy), Terms extraction, Topic Modeling (Gensim);
<li>Supervised Learning: Text classification (Fasttext), Predictive Modeling, Model Cross-Validation, Hyperparameter optimization;
<li>Data Visualization: Distributions, Timeline word usage (Plotly), Wordclouds, Network mapping (Gephi).
  

# Installation guide
 
<code>data_wrangling.ipynb</code>: Python code with data preprocessing and features engineering
  
<code>data_cleaning.ipynb</code>: Python code with text cleaning 
 
<code>network_shaping_ai.gephi</code>: output network dataframe 
  
<code>requirements.txt</code>: required libraries and packages

  
## Preliminary results
Extraction of the topics and main terms on all corpora through network mapping, text classification model testing - work in progress.
The network represents the links (co-occurrence in the text) between the terms extracted from all corpora. The node's colors are allocated by the Louvain Method of community detection. Group labels are manually assigned based on the main topic of the words in the community.

## Main challenges
<li>Working with big text data: optimization of the analysis, experiment with ram and data pre-processing techniques;
<li>Text data preparation for the analysis: cleaning data using additional stop-words, regular expressions, implementation of the lemmatization.

  
