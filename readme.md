# Graph Convolutional Networks for Homophilic and Heterophilic Graphs

This project explores the performance of Graph Convolutional Networks (GCNs) on datasets with homophilic and heterophilic properties. The primary focus is on comparing the performance of GCNs on the **Cora** dataset (homophilic) and the **Texas** dataset (heterophilic).

## Table of Contents
1. [Introduction](#introduction)
2. [Datasets](#datasets)
3. [Model Architecture](#model-architecture)
4. [Experiments](#experiments)
5. [Results](#results)
6. [Usage](#usage)
7. [License](#license)

## Introduction
Graph Convolutional Networks (GCNs) assume that connected nodes in a graph share similar features and labels, which aligns well with homophilic graphs but struggles with heterophilic ones. This project demonstrates how GCNs perform under these contrasting conditions.

## Datasets
1. **Cora**:
   - Type: Homophilic
   - Homophily Ratio: 0.81

2. **Texas**:
   - Type: Heterophilic
   - Homophily Ratio: 0.11

## Model Architecture
The implemented GCN consists of:
- **2 GCN Layers**:
  - First layer: Applies ReLU activation
  - Second layer: Outputs logits for classification
- Dropout regularization for better generalization.

## Experiments
The experiments involve:
1. Computing the homophily ratio of each dataset.
2. Training a GCN on both datasets.
3. Comparing validation and test accuracies to assess the impact of homophily.

## Results
- **Cora** (Homophilic):
  - Best Validation Accuracy: 78.40%
  - Test Accuracy at Best Validation: 80.50%
- **Texas** (Heterophilic):
  - Best Validation Accuracy: 63.89%
  - Test Accuracy at Best Validation: 27.78%

The stark performance gap highlights the limitation of GCNs in handling heterophilic datasets.




## Visualization
The homophily and heterophily ratios are visualized as bar charts for easy comparison between datasets.

## License
This project is licensed under the MIT License.









