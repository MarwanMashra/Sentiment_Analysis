# Sentiment Analysis

This is a sentiment analysis for Amazon food reviews using Bert, embeddings and other NLP approaches. This project was done in the context of a class on NLP during the master of AI at the university of Paris-Saclay.

## Dataset

The project is based on the Amazon food review from customers dataset. The dataset comes from a Kaggle competition. It can be downloaded from <a href="https://www.kaggle.com/snap/amazon-fine-food-reviews/download" > here </a>(254MB).

## Task

This is a multi-class classification. Reviews should be classified into three classes <b>Negative</b>, <b>Positive</b>, <b>Neutral</b>.

## Used approaches

- Simple vectorization approaches: CountVectorizer and Tf-idf with Scikit-learn.
- Different Pretrained Word Embeddings: Glove, Word2Vec and FastText with Gensim.
- Different visualization approaches: PCA, t-SNE
- Bert embeddings (DistilBERT) with Transformers - Hugging Face.
- Fine-tuned Bert with pyTorch.

## Results

| Method                                   | F1 macro avg. |
| ---------------------------------------- | :-----------: |
| Glove embeddings + SGD                   |     0.46      |
| DistilBERT embeddings + SGD              |     0.566     |
| DistilBERT embeddings + Logistic + stack |     0.69      |
| DistliBERT Fine-tuned                    |     0.75      |
