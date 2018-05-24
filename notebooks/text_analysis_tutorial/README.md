## Workshop

This directory contains the Jupyter Notebooks which will be followed during the workshop/tutorial.

It largely follows the structure of the [News Classification](https://github.com/RaRe-Technologies/gensim/blob/develop/docs/notebooks/gensim_news_classification.ipynb) notebook, with the major difference being in the pre-processing done by spaCy instead of NLTK.

The tutorial on Topic Modelling follows us through different topic models and how to visualise them and evaluate them, while the text analysis tutorial introduces users to a variety of text analysis approaches.

### Requirements for Topic Modelling

```
- Jupyter
- Gensim Version (>=0.13.1 would be preferred since we will be using topic coherence briefly)
- matplotlib
- spaCy
- pyLDAVis
```

In case the user finds it difficult to download any of the above, there will be a Jupyter Notebook with all the cells already run, so you can just follow the same.

### Requirements for Text Analysis

```
- Jupyter
- Gensim Version 
- matplotlib
- spaCy
- scikit-learn
- keras
```

### Setup

- Start by cloning the repo using

`git clone https://github.com/bhargavvader/personal`

- Go into the `notebooks/text_analysis_tutorial` directory

- Install `virtualenv` using

`pip install virtualenv`

- Start the environment with

```
virtualenv venv
source venv/bin/activate
```

- Download requirements with -

`pip install -r REQUIREMENTS.txt`

And you should be good to go!

Alternatively, if you are using anaconda as your virtual environment, running `conda install gensim` and `conda install spacy` should also do the trick.

### Text Analysis Tutorial

For the text analysis tutorial, you will be following the same instructions as above, but will need to run

`pip install -r REQUIREMENTS_1.txt`

Alternatively, you can look up which of the libraries you would still need to download and go ahead and just download those.

### Downloading spaCy language model

Both of the tutorials will be using the spaCy English language model, so we will be needing to download it first.
This [link](https://spacy.io/usage/models) contains instructions to download this model.
All we really have to do is run `python -m spacy download en` after we finish all our libary installations.