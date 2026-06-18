# Peer Review Assignment Optimization

This repository explores and compares various algorithmic approaches for the Peer Review Assignment problem. The core objective is to analyze the trade-offs between **Fairness (Max-Min)** and **Efficiency (Nash Social Welfare / Total Similarity)** in paper-reviewer matching.

## Research Context
Peer review systems often face the "bottleneck" problem: a small number of papers with low similarity to available reviewers can significantly lower the overall fairness of the assignment. 

We benchmark our implementation against the **PeerReview4All (PR4A)** algorithm, which utilizes an iterative Max-Flow approach to ensure worst-case fairness.

### Reference Implementation
We acknowledge the original research and the official implementation by the authors:
* **Paper:** [PeerReview4All: A Peer Review Assignment System](https://www.jmlr.org/papers/volume22/20-190/20-190.pdf)
* **Official Repository:** [https://github.com/niharshah/peerreview4all](https://github.com/niharshah/peerreview4all)

## Project Objectives
Our research investigates whether we can achieve significant gains in **Total Similarity** or **Nash Social Welfare** by accepting a controlled trade-off in **Max-Min Fairness**. 

We compare:
1.  **PR4A (Fairness-Centric):** Focuses on maximizing the similarity of the most disadvantaged paper.
2.  **Binary NSW / Min-Cost Flow (Efficiency-Centric):** Optimizes for global welfare by balancing reviewer loads against logarithmic utility functions.