# Multilingual Document Retrieval System

## Project Overview

This project aims to develop a high-performance multilingual document retrieval system that processes a corpus of over 250,000 documents in seven languages. It retrieves the top 10 most relevant documents per query while optimizing both speed and accuracy. The final model was tested and submitted on Kaggle for evaluation.

## Approach

We implemented two primary retrieval models:
- TF-IDF: A baseline method ranking documents based on term frequency and inverse document frequency.
- BM25: An improved model that adjusts for term saturation and document length to enhance retrieval accuracy.

## Methodology

### 1. Preprocessing
- Language-specific tokenization and stopword removal.
- Text normalization by lowercasing and stemming if applicable.
- Corpus partitioning by language.

### 2. Retrieval Models
- TF-IDF: Constructed sparse matrices for efficient query-document matching.
- BM2: Tuned hyperparameters (e.g., `k1` for term saturation) to optimize performance.

### 3. Evaluation
- Performance assessed using Recall@10 metric.
- TF-IDF Recall@10: `0.592`  
- BM25 Recall@10: `0.730` 

### 4. Alternative Approaches
- Experimented with Sentence-BERT (paraphrase-multilingual-MiniLM-L12-v2) for semantic retrieval.
- Achieved lower performance (Recall@10 = 0.26) due to document length limitations.

## Authors

This work was carried out by Youssef Belghmi, Hamza Morchid, and Amine Belghmi, Master Data Science students at EPFL, as part of the Distributed Information Systems (CS-423) course project.
