# 🎬 IMDb Review Sentiment Classification

## 💼 Business Use Case

Customer reviews contain useful signals about how an audience perceives a product, but manually reading thousands of comments is difficult to scale. This project explores how a sentiment classifier can help product, marketing, or content teams sort positive and negative feedback, monitor changes in perception, and focus human review on the comments that deserve closer attention.

## 🎯 Principal Objective

The objective is to build a clear NLP baseline that predicts whether an IMDb review expresses positive or negative sentiment. The notebook covers the complete workflow, from label preparation and train-test splitting to text vectorization, neural-network training, and evaluation on unseen reviews.

The model intentionally uses a relatively simple multi-hot text representation. This keeps the pipeline easy to understand and provides a useful benchmark before moving to richer representations or more complex language models.

## 🔍 Key Takeaways

The feed-forward neural network achieves approximately **87% test accuracy**, showing that a compact model can already capture meaningful sentiment signals from review text. At the same time, the experiment makes the limitations of a bag-of-tokens representation clear: word order, context, and semantic relationships are lost.

From a business perspective, this type of model is most useful as a triage and monitoring tool rather than a fully autonomous decision system. Before deployment, the evaluation should go beyond accuracy and consider precision, recall, F1 score, error patterns, and the business cost of missing strongly negative feedback.

## 💻 Explore the Notebook

The [notebook](https://github.com/saels/movie-sentiment-classification/blob/83b079c096d00700d70ddca750dfec14b64c8ba4/Movie_sentiment_classification.ipynb) contains the full preprocessing, vectorization, model architecture, training, and evaluation workflow. Check the code for the implementation details and for a closer look at how this baseline can be extended with richer text representations and deeper error analysis.
