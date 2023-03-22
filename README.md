# Social-Network-Graph-Link-Prediction-Facebook-Challenge
Problem statement: 
Given a directed social graph, have to predict missing links to recommend users (Link Prediction in graph)

# Data Overview:
We have taken data from facebook's recruting challenge on kaggle https://www.kaggle.com/c/FacebookRecruiting.
Data contains two columns source and destination each edge in graph. Data columns:-
- source_node int64
- destination_node int64

# Mapping the problem into supervised learning problem:
Generated training samples of good and bad links from given directed graph and for each link got some features like no of followers, is he followed back, page rank, katz score, adar index, some svd fetures of adj matrix, some weight features etc. and trained ml model based on these features to predict link.

# Business objectives and constraints:
- No low-latency requirement.
- Probability of prediction is useful to recommend ighest probability links

# Performance metric for supervised learning:
- Both precision and recall is important so F1 score is good choice
- Confusion matrix
