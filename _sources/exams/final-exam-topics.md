# Exam Content Guide

---

## Overview

Our final exam format will be similar to the midterm exam. It is a big quiz covering all the topics we've learned after midterm exam. You'll have 1 hour and 50 minutes to complete the exam.

> Important Note: You need to use your laptop or computer to finish the exam.

- **Dimensionality Reduction**:
  - Curse of Dimensionality
  - Feature extraction
    - Principal Component Analysis
    - Nonlinear Dimensionality Reduction Methods:
      - Kernel PCA
      - Stochastic Neighbor Embedding (SNE)
  - Feature Selection
    - Feature extraction vs. Feature selection
    - Filter method,Fisher score, Wrapper method, Embedded method
    - Bayesian Belief Networks, Markov Blanket & Boundary: Incremental Association Markov Blanket(IAMB)
- **Classification**:
  - Decision Tree, Regression Tree, Information Gain, Gini impurity
  - Regression Tree
  - Overfitting and Tree Pruning
  - Bayesian Classification
    - Bayes’ Theorem
    - Classification Based on Bayes’ Theorem
    - Naïve Bayes Classifier
      - Avoiding the Zero-Probability Problem
  - Lazy vs. Eager Learning
    - Lazy Learner(Instance-Based Methods): k-Nearest Neighbor Algorithm
  - Linear, Logistic regression and Perceptron
  - Classifier Evaluation and Selection
    - Classifier Evaluation Metrics: Confusion Matrix, Accuracy, Error Rate,Sensitivity Specificity, Precision and Recall,and F-measures
    - Evaluating Classifier Accuracy: Holdout, Cross-Validation Methods, Bootstrap
    - Model Selection: ROC Curves
- **Clustering**
  - What is Clustering? What is the difference between Clustering and Classification?
  - K-Means: Algorithm, Strength and Limitations
    - Strength: Simple and Efficient.
    - Weaknesses: 1. Clusters with different sizesand densities.2. Non-spherical clusters.3. Sensitive to initial centroids
    - How can we deal with the initialization problem?
  - Agglomerative Clustering
    - Merging (Linkage) Criteria: Single Linkage, Average Linkage, Complete Linkage: Smallest maximum distance
- **Neural Network**
  - Feed Forward Network
    - Architecture
    - Activation function
    - Loss function
    - Regularization
    - Optimization: backpropagation, learning rate
  - RNN: Limitations of Traditional Neural Networks on Sequences data, Long-Term Dependencies
    - Long Short Term Memory Networks (LSTMs), Gated recurrent unit (GRU)
  - RNN with Attention Mechanisms
  - Transformer: Encoder-Decoder Architecture, Word Embedding
    - Self-Attention: Q, K, V, Softmax
    - Multi-Headed Self-Attention, Positional Encoding, Residual Connections, Layer Normalization
  - Convolutional Neural Networks
    - Convolution Layer: Output volume size? Number of parameters in Convolution Layer?
    - Pooling layer
      - Max Pooling, Avg Pooling
    - Fully connected layer
    - 1-D Convolution for Sequences data
