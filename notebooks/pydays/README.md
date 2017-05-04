## PyDays Vienna

This directory contains the Jupyter Notebook which will be followed during the workshop for PyDays Vienna 2017.

It largely follows the structure of the [News Classification](https://github.com/RaRe-Technologies/gensim/blob/develop/docs/notebooks/gensim_news_classification.ipynb) notebook, with the major difference being in the pre-processing done by spaCy instead of NLTK.

### Requirements

```
- Jupyter
- Gensim Version (>=0.13.1 would be preferred since we will be using topic coherence briefly)
- matplotlib
- spaCy
- pyLDAVis
```

In case the user finds it difficult to download any of the above, there will be a Jupyter Notebook with all the cells already run, so you can just follow the same.


### Setup

- Start by cloning the repo using

`git clone https://github.com/bhargavvader/personal`

- Go into the `notebooks/pydays` directory

- Install `virtualenv` using

`pip install virtualenv`

- Start the environment with

`virtualenv venv`

- Download requirements with -

`pip install -r REQUIREMENTS.txt`

And you should be good to go!