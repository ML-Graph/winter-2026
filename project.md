---
layout: page
title: Project
permalink: /project/
---

### 1. Background and Problem Formulation - 10%
- **Background - 5%**: 
  - What is the general background of the problem you are working on?
    - I want to develop a better paper categorization system
- **Problem Formulation - 5%**: 
  - Under the general topic, what specific problem is your project addressing?
    - I want to develop a machine learning model/algorithm to take input of the paper, output the paper topic (machine learning, computer system, human-computer collaboration, etc.)

### 2. Data Mining Stage - 35%
- **Data Collection and Store - 15%**: 
  - What data are you looking to kick off your project? How do you collect them? What data structure do you use to represent them?
    - I collect Cora/Citeseer/Pubmed Data from somewhere (e.g., a paper, a GitHub repository, Hugging Face, etc.), and I use an adjacency list to store their connection and a matrix to store their node feature
- **Data Mining - 20%**: 
  - What kind of data mining problem do you need to do and why? 
    - I need to analyze the network homophily/heterophily since leveraging this property might help me develop a better machine learning model for paper classification.
  - How do you do it?
    - I calculate for every edge, the two ending points, whether they are in the same class or not, and quantify the average ratio as a homophily ratio
  - What kind of pattern do you find? How do you present your findings/analysis?
    - I find that in many paper citation networks, the homophily is pretty high. Using Number/Table/Figure, etc.

### 3. Machine Learning Stage - 35%
- **Machine Learning Model Design**: 
  - Based on your targeted problem, what kind of machine learning model do you want to build and why?
    - I want to build a graph neural network to fully exploit the discovered homophily principle.
  - How do you build your machine learning model, and what is the key design?
    - The key design is to aggregate neighborhood information together, and I use the PyTorch Geometric Package, and within this package, certain functions can help me achieve my design philosophy
  - What kind of experiments do you have to achieve your task?
    - I conduct paper classification by taking the paper as input through my graph neural network, and it helps me achieve very high node classification performance.

### 4. Discussion - 10%
- **Discussion - 5%**: 
  - Any further discussion on your exploration of this project?
    - I take networks of different homophily and derive a clear positive relation between node classification and homophily level.
  - Any further thinking and interesting questions you can ask about this project?
    - How about the network performance on a heterophily network like dating networks? If we maliciously upload some papers that are meaningless, would that compromise the performance?
- **Feeling of this class - 5%**: 
  - Feeling of this class.

Bonus Points will apply if you consider doing projects in the following fields with (*) or any domain beyond the following:

## * Infrastructure Mining and Machine Learning
- Water/Power/Gas network
- Transportation network
- Networking system

## * Neural Biology Learning
- Brain Network
- Protein/Molecule
- Gene

## Social Mining and Machine Learning
- Reddit
- Twitter
- Bluesky
- Amazon Recommender System

## Document and Citation Networks
