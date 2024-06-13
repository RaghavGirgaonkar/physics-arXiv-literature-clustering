# Physics ArXiv Literature Clustering and Recommender
Clustering and Recommender system of Physics literature taken from the [Kaggle arXiv dataset](https://www.kaggle.com/datasets/Cornell-University/arxiv).

### Requirements
GitHub Large File System:  [git lfs](https://git-lfs.com)

Python 3.9+

Install required packages
``` pip install -r requirements```

### Create Dataset clustering model

1. Download ```arxiv-metadata-oai-snapshot.json``` from the [Kaggle arXiv dataset](https://www.kaggle.com/datasets/Cornell-University/arxiv) to the same directory.

2. Run ```clustering.ipynb``` to create dataset and encode text using Sentence Transformers models or TfidfVectorizer. 

### Get similar papers

After the dataset and models have been saved from running ```clustering.ipynb```, run ```recommend.ipynb``` and in the last cell enter the link to the arXiv paper (eg http://www.arxiv.org/abs/1602.03837). 
The number of similar papers to be recommended can be set using the ```num_papers``` variable. 

Output will be stored in ```output.txt```. A sample output file is provided.


### To Do

- Host Recommender on Website
- Try Gaussian Mixture Modeling
- Use more sophisticated embeddings
