## Workshop

This directory contains the Jupyter Notebooks which will be followed during the workshop/tutorial.

The computational social science tutorial will walk us through networks and text analysis - this is just the tip of the iceberg, and there is a lot more which would constitute computational social science, but we have to start somewhere. Hopefully this should give you an idea of the kinds of methods used.

### Requirements for Tutorial

```
- Jupyter
- Gensim 
- matplotlib
- spaCy
- pandas
- numpy
- networkx
- seaborn
```


### Setup

The setup instructions are if you are using virtualenv for your environment: you can use any environment to do this, or even on your local (though it isn't recommended). Basically, you would want to be able to run the jupyter notebook in the directory, install the packages, and start running the cells. The instructions below will help you through one way of making that happen.

- Start by cloning the repo using

`git clone https://github.com/bhargavvader/personal`

- Go into the `notebooks/computational_social_science` directory

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

If you are using anaconda as your virtual environment, running `conda install gensim` and `conda install spacy` should also do the trick.

Alternatively, you can look up which of the libraries you would still need to download and go ahead and just download those.

### Downloading spaCy language model

The tutorial will be using the spaCy English language model, so we will be needing to download it first.
This [link](https://spacy.io/usage/models) contains instructions to download this model.
All we really have to do is run `python -m spacy download en` after we finish all our libary installations.
