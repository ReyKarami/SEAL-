# SEAL+
This project introduces SEAL+ (SubGraph Enhanced Link prediction), an enhanced framework for link prediction in graphs. Based on the SEAL framework, SEAL+ incorporates subgraph information in both the Encoder and Decoder to improve link prediction performance.

## Overview
SEAL+ introduces two key innovations:

### Subgraph Extraction Methods:
- h-hop extraction: Extracts traditional h-hop subgraphs to capture local graph structures and node relationships.
- DIS (Distance-based): A proposed method for subgraph extraction, selecting subgraphs based on the distance between feature vectors of subgraph nodes and those of target nodes.
### Subgraph Embedding Generation Methods:
- CNN-based feature extraction: Convolutional Neural Networks (CNN) are used to extract feature vectors from subgraphs.
- NDP (Normal Distance Penalty): This method introduces a novel approach to weighting nodes in subgraphs. It weighs the feature vectors of subgraph nodes to generate a more meaningful subgraph feature vector.
### Link Prediction Approach:
Classification-based prediction: Feature vectors of target and subgraph node pairs are concatenated and fed into a neural network for link prediction.

This framework is evaluated to demonstrate its effectiveness in improving link prediction accuracy and model performance metrics.

## Evaluation Metrics
The performance of the SEAL+ framework is evaluated using the following metrics:

- Accuracy
- Recall
- Precision
- F1-Score
- Average Precision (AP)
- Precision-Recall AUC (PR-AUC)

## Results
The SEAL+ framework demonstrates a notable improvement in link prediction performance over the original SEAL method. By directly utilizing subgraph feature vectors, SEAL+ achieves better overall results in accuracy, F1-score, and other performance metrics, particularly in graphs with denser linkages.
