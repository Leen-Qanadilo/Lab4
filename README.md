# Lab4

Lab 4 – Goodreads Reviews Feature Engineering (Gold Layer v2)

This notebook builds an advanced feature layer for the Goodreads reviews
dataset using Apache Spark and Azure Data Lake Storage (ADLS). It cleans
the review text, adds multiple NLP features (sentiment, TF-IDF,
embeddings, readability, etc.), and stores everything as Delta tables in
the Gold / feature_v2 layer.

------------------------------------------------------------------------

1. Prerequisites

-   Environment
    -   Azure Databricks or Synapse with Spark
    -   Python 3.x, Spark 3.x
-   Python libraries
    -   nltk
    -   sentence-transformers
    -   textstat
    -   textblob
    -   numpy, pandas, scikit-learn
    -   pyspark
-   Storage
    -   ADLS Gen2 account: goodreadsreviews60106541
    -   Lakehouse container: lakehouse

------------------------------------------------------------------------

2. High-Level Pipeline

1.  Connect to ADLS and verify.
2.  Install/import libraries.
3.  Load dataset from Gold layer.
4.  Train/Validation/Test split.
5.  Text cleaning & basic statistics.
6.  Sentiment features using VADER.
7.  TF-IDF generation using Spark ML.
8.  BERT sentence embeddings.
9.  Readability & lexical richness metrics.
10. Final combined dataset writing.

------------------------------------------------------------------------

3. How to Run

1.  Open Lab4.ipynb.
2.  Set ADLS account key.
3.  Run notebook top‑to‑bottom.
4.  Verify Delta outputs under gold/feature_v2/.
