# Question Answer Feedback

This is a project that uses GloVe embeddings and cosine similarity to classify feedback on Amazon question and answer datasets.

## Installation

To run this project, you will need the following Python packages:

    pandas
    numpy
    scikit-learn
    gensim

You can install these packages using pip:  ```pip install -r requirements.txt```

You will also need to download the pre-trained GloVe embeddings from the Stanford website. We recommend using the 300-dimensional embeddings trained on the Common Crawl dataset.


## Usage

To use this project, you will need to download an Amazon question and answer dataset. You can find these datasets on the Amazon product data website. Once you have downloaded the dataset, you can preprocess it using the preprocess.py script in the scripts folder. This script will clean the data and split it into training and testing sets.

Next, you can use the train.py script to train a classifier on the training set. This script will generate word embeddings for each question and answer using the GloVe embeddings, and then calculate the cosine similarity between each question and answer pair. It will then use these similarity scores to train a classifier using the scikit-learn library.

Finally, you can use the test.py script to evaluate the performance of the classifier on the testing set. This script will generate word embeddings and similarity scores for each question and answer pair in the testing set, and then use the trained classifier to predict the feedback for each pair.
 
