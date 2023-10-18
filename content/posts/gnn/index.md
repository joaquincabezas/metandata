---
title: "AI explainability: GNNExplainer coefficients"
date: 2023-10-18
description: "How relevant is to tune the coefficients for your explanations"
type: 'post'
---

Explainability is always a hard topic. For any complex process, it is difficult to achieve the expectations of the person asking for the explanation. In part, because this person will not know anything about the internals and is asking for a "quick and simple", and in part because it is... well... complex (consisting of many different and connected parts). 

One of the approaches is analyzing what parts of the input were 'essential' for the explanation to be the way it is. If these inputs were different, the prediction would be different as well. So, by modifying part of the inputs and seeing how the prediction changes, we can detect these 'essential' parts of the input.

Applying explainability techniques to Graph Neural Networks is available thanks to many Open Source implementations of algorithms. One of these (and among the firt ones) is [GNNExplainer (Rex Ying et al)](https://arxiv.org/abs/1903.03894), available in [Pytorch Geometric GNNExplainer implementation](https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.explain.algorithm.GNNExplainer.html).