# Semantic and Keyword Search

## Overview

This project demonstrates the implementation of **Keyword Search** and **Semantic Search** techniques for information retrieval. It also explains the similarity and distance metrics used to compare text embeddings.

## Topics Covered

- Keyword Search
- Semantic Search
- Word Embeddings
- Cosine Similarity
- Dot Product
- Euclidean Distance

## Concepts

### Keyword Search
Keyword Search retrieves documents by matching the exact words or phrases present in the user's query. It relies on keyword occurrence rather than understanding the meaning of the text.

### Semantic Search
Semantic Search retrieves documents based on their meaning and context rather than exact keyword matching. It uses vector embeddings to identify semantically similar content.

### Cosine Similarity
Cosine Similarity measures the similarity between two vectors by calculating the cosine of the angle between them. Its value ranges from **-1 to 1**:
- **1** → Identical direction (highest similarity)
- **0** → No similarity
- **-1** → Opposite direction

### Dot Product
The Dot Product measures the relationship between two vectors by multiplying their corresponding components and summing the results. A **higher positive value** generally indicates greater similarity, while values close to **0** or **negative** indicate lower similarity.

### Euclidean Distance
Euclidean Distance measures the straight-line distance between two vectors in a vector space. Its value ranges from **0 to ∞**:
- **0** → Identical vectors
- **Smaller distance** → More similar
- **Larger distance** → Less similar

## Files

- `Semantic_Keyword_Search.ipynb` – Implementation of keyword search, semantic search, and similarity metrics.
- `README.md` – Project documentation.