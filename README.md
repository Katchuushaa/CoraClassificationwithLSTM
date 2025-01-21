# Classification of Scientific Article Abstracts on Cora Dataset Using Long Short Term Memory

This repository contains the implementation and results of my undergraduate thesis research, titled **"Klasifikasi Abstrak Artikel Ilmiah pada Dataset Cora Menggunakan Long Short Term Memory"**. The research aims to classify scientific articles based on their abstracts using the Long Short Term Memory (LSTM) model and FastText word embedding.

---

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Research Stages](#research-stages)
- [Results](#results)
- [Conclusion](#conclusion)
---

## Introduction

In this study, text classification was conducted on the Cora dataset using the LSTM model. The dataset contains scientific article abstracts grouped into seven topics: 

1. Neural Networks
2. Probabilistic Methods
3. Genetic Algorithms
4. Theory
5. Case Based
6. Reinforcement Learning
7. Rule Learning

By utilizing text mining techniques, this research focuses on improving classification accuracy using FastText embeddings and optimizing hyperparameters.

---

## Dataset

The **Cora Dataset** was used, which consists of 2,708 scientific articles. Each article is represented by its abstract and associated topic label. For this research, pre-processing steps such as cleaning, stemming, stopword removal, and tokenization were applied to prepare the data.

### Dataset Source
- [Andrew McCallum's Cora Dataset](https://people.cs.umass.edu/~mccallum/data.html)

### Key Features of the Dataset
- Number of articles: 2,708
- Number of unique words: 16,155 (reduced to 1,433 after filtering)
- Seven predefined classes/topics

---

## Research Stages

1. **Data Collection**: Combining the content file and abstract data to form a unified dataset.
2. **Pre-processing**:
   - Cleaning text by removing punctuation and case folding.
   - Applying stemming and stopword removal.
   - Filtering unique words to match dataset specifications.
3. **Feature Engineering**:
   - Generating word embeddings using FastText.
4. **Data Splitting**:
   - Splitting data using K-Fold cross-validation with k=5.
5. **Model Development**:
   - Constructing LSTM architecture with optimized hyperparameters.
6. **Evaluation**:
   - Evaluating performance using accuracy, precision, recall, F1-score, and confusion matrix.

---

## Results

- The best model achieved an accuracy of **93.55%** with a loss of **0.3108**.
- Optimal hyperparameters:
  - Vector size: 8
  - Batch size: 32
  - Epochs: 50
  - Unique words: 11,147

### Comparison with Previous Studies
This research achieved higher accuracy compared to prior methods:
- Graph Convolutional Networks (GCN): 81.5%
- Graph Attention Networks (GAT): 83%
- Previous LSTM studies: ~90%

### Confusion Matrix
The confusion matrix analysis showed high precision and recall for all seven classes, with most scores exceeding 97%.

---

## Conclusion

The research demonstrates that LSTM combined with FastText embeddings effectively classifies scientific article abstracts from the Cora dataset. Key findings include:

- The use of stemming and filtering unique words significantly enhances accuracy.
- Larger input sizes generally improve accuracy but increase training time.

---
## Citation

If you use this repository or dataset, please cite:

```
Daffa Fikri. 2024. Klasifikasi Abstrak Artikel Ilmiah pada Dataset Cora Menggunakan Long Short Term Memory. Institut Pertanian Bogor.
```

---
