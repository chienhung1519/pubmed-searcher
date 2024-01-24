# Pubmed Searcher

## Overview
PubmedSearcher is a Python script that allows you to search for articles on PubMed, a popular database of biomedical literature. It provides a simple interface to search for articles based on a query and retrieve relevant information such as the article title, abstract, authors, DOI, and URL. PubmedSearcher is based on Pubmed API.

## Prerequisites
- Python 3.x
- requests library
- json library
- xml.etree.ElementTree or xml.etree.cElementTree library
- dataclasses library
- argparse library

## Usage

1. Download the `PubmedSearcher.py` file.
2. Initialize a PubmedSearcher instance and search.

```python
from PubmedSearcher import PubmedSearcher
searcher = PubmedSearcher()
articles = searcher.search("your_query_here", 20)
```

Replace `"your_query_here"` with your desired search query and `20` with the maximum number of articles to return.

3. Returned articles is a Article class with six attributes (pubmed_id, title, abstract, authors, doi, url).

```python
Article(pubmed_id=12345, title="Article title", abstract="Article abstract", authors="Author names", doi="Article doi", url="Article URL")
```