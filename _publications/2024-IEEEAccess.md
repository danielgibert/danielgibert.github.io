---
title: "Adversarial Robustness of Deep Learning-based Malware Detectors via (De) Randomized Smoothing"
collection: publications
category: manuscripts
permalink: /publication/2024-IEEEAccess-DeRandomizedSmoothing
date: 2024-05-01
excerpt: '  In this work, we propose a chunk-based smoothing scheme that reduces the chances of sampling adversarial content injected by malware authors by selecting 
  correlated subsets of bytes. During training, our chunk-based smoothing scheme trains a base classifier to make classifications on 
   a subset of contiguous bytes or chunk of bytes. At test time, a large number of chunks are then classified by a base
    classifier and the consensus among these classifications is then reported as the final prediction. We propose two 
    strategies to determine the location of the chunks used for classification: (1) randomly selecting the locations
     of the chunks and (2) selecting contiguous adjacent chunks. To showcase the effectiveness of our approach, we have
      trained two classifiers with our chunk-based smoothing schemes on the BODMAS dataset. Our findings reveal that
       the chunk-based smoothing classifiers exhibit greater resilience against adversarial malware examples generated 
       with state-of-the-art evasion attacks, outperforming a non-smoothed classifier and a randomized smoothing-based 
       classifier by a great margin.'
venue: 'IEEE Access'
paperurl: 'https://arxiv.org/abs/2405.00392' #Add here link to paper
citation: 'Daniel Gibert, Giulio Zizzo, Quan Le, Jordi Planes. (2024). &quot;Adversarial Robustness of Deep Learning-based Malware Detectors via (De) Randomized Smoothing.&quot; <i>IEEE Access</i>.'
---

In this work,  we propose a chunk-based smoothing scheme that reduces the chances of sampling adversarial content injected by malware authors by selecting 
correlated subsets of bytes. Our approach works as follows:
* During training, our chunk-based smoothing scheme trains a base classifier to make classifications on 
a subset of contiguous bytes or chunk of bytes. 
* At test time, a large number of chunks are then classified by a base
classifier and the consensus among these classifications is then reported as the final prediction.

The following figure illustrates our adversarial defense:![dynamic_chunk_based_classification.png](../images/dynamic_chunk_based_classification.png)

We propose two strategies to determine the location of the chunks used for classification: (1) randomly selecting the locations
of the chunks (RCA) and (2) selecting contiguous adjacent chunks (SCA).

The RCA scheme has three key components:
- Sampling L chunks randomly from the input sequence using a uniform distribution.
- Classifying each chunk independently.
- Combining the classification results by taking a majority vote.

The SCA scheme samples chunks in an orderly way from the start of the input byte sequence to its end, instead of randomly sampling chunks. The SCA scheme has three key components:
- Sampling L sequentially adjacent chunks from the input sequence.
- Classifying each chunk independently.
- Combining the classification results by taking a majority vote.

To showcase the effectiveness of our approach, we have trained two classifiers with our chunk-based smoothing schemes on the BODMAS dataset. 
Our findings reveal that the chunk-based smoothing classifiers exhibit greater resilience against adversarial malware examples generated  
with state-of-the-art evasion attacks, outperforming a non-smoothed classifier and a randomized smoothing-based 
classifier by a great margin.

![IEEE_ACCESS_shift.png](../images/IEEE_ACCESS_shift.png)
![IEEE_ACCESS_code_caves.png](../images/IEEE_ACCESS_code_caves.png)
