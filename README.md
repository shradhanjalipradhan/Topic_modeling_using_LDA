
# Topic Modelling using LDA

## Overview
This project aims to uncover the underlying thematic structure in a collection of documents from the `20 newsgroups` dataset. We use Latent Dirichlet Allocation (LDA), a generative probabilistic model, to identify topics across the documents.

## Dataset
The dataset consists of newsgroup documents from the `20 newsgroups` collection, a popular dataset for experiments in text applications of machine learning techniques, such as text classification and text clustering.

## Preprocessing
We perform several preprocessing steps on the text data:
- **Tokenization**: Split the text into individual words.
- **Punctuation Removal**: Remove all punctuation from the words.
- **Lowercasing**: Convert all the words to lowercase to maintain consistency.
- **Stop Words Removal**: Exclude common words that do not contain important significance to be used in the model.
- **Stemming**: Reduce words to their root form.

## Feature Extraction
We convert the preprocessed text data into numerical vectors using two methods:
- **TF-IDF Vectorizer**: Transform the text into a matrix of TF-IDF features.
- **Count Vectorizer**: Create a bag-of-words representation of the text.

## Model Building
We apply Non-Negative Matrix Factorization (NMF) to identify topics within the documents. The number of topics is set to 5 as a starting point but can be adjusted according to the specific needs or results of the analysis.

## Results
For each topic, we display the top 10 words that are most representative of the topic. These words give us insight into the content and themes of the topics discovered by the LDA model.

## Scripts and Notebooks
The analysis is conducted in Python using libraries such as `sklearn` for machine learning, `nltk` for natural language processing, and other supporting libraries.

## Usage
To run the analysis, ensure that the following Python libraries are installed: `sklearn`, `nltk`, `pandas`, and others as required. The scripts can be run in a Python environment with the necessary libraries installed.

## Acknowledgements
This project is part of a broader effort to understand large collections of unstructured text data. The methods and approaches used here can be adapted to other text corpora and research questions.
