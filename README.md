# NLP_Text_Summary_Generator
This Python project implements a text summarization algorithm using _Natural Language Processing (NLP)_ techniques. The algorithm aims to generate a summary of a given text document by extracting the most important sentences.

## How it works
1. The input text document is read and split into individual sentences.
2. Stop words (common words that do not carry much meaning) are removed from the sentences.
3. A similarity matrix is built, which represents the similarity between each pair of sentences in the document.
4. The similarity matrix is used to create a graph, where each sentence is a node and the similarity score between sentences is an edge.
5. The sentences are ranked based on their importance using the PageRank algorithm.
6. The top-ranked sentences are selected to form the summary.
## Dependencies
This project requires the following dependencies:

* nltk
* numpy
* networkx
  
You can install these dependencies using pip:
```
pip install nltk numpy networkx
```
## Usage
To generate a summary, follow these steps:

Import the necessary libraries:
```python
import nltk
from nltk.corpus import stopwords
from nltk.cluster.util import cosine_distance
import numpy as np
import networkx as nx
```
Define the functions `read_article`, `sentence_similarity`, `build_similarity_matrix`, and `generate_summary` as provided in the code.

Call the `generate_summary` function with the path to the text file and the desired number of sentences in the summary. For example:
```python
generate_summary("Coding.txt", 2)
```
This will generate a summary of the text document `"Coding.txt"` containing 2 sentences.

Note: The input text document should be in plain text format.

## Acknowledgments
This project was inspired by the field of NLP and its applications in text summarization. It incorporates various techniques and algorithms to achieve the goal of generating a summary from a given text document.

## Contact
uditsathe@gmail.com .
