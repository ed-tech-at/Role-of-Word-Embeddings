# The Role of Word Embeddings

## Local Installation
To experiment with word embeddings locally, the dataset Gensim could be used with Python 3. 

Python 3 can be installed from https://www.python.org/

There is currently a bug in the Gensim module. To fix it, an older version of scipy could be used. See https://stackoverflow.com/q/78279136

```
pip install scipy==1.12
pip install gensim
```

## Run Examples Locally

`python3`

```
import gensim.downloader as api
dataset = api.load('glove-wiki-gigaword-300')

dataset.most_similar_cosmul(positive=["warm", "winter"], negative=["summer"])

dataset.most_similar_cosmul(positive=["boat", "road"], negative=["sea"])
```