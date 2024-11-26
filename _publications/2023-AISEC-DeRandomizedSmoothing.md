---
title: "Certified robustness of static deep learning-based malware detectors against patch and append attacks"
collection: publications
category: conferences
permalink: /publication/2024-AISEC-DeRandomizedSmoothing
date: 2023-09-23
excerpt: 'This paper presents an adversarial defense based on (de)randomized smoothing that provides deterministic robustness certificates against patch and append attacks on end-to-end malware detectors.'
venue: '16th ACM Workshop on Artificial Intelligence and Security (AISEC)'
paperurl: 'https://dl.acm.org/doi/abs/10.1145/3605764.3623914' #Add here link to paper
citation: 'Daniel Gibert, Giulio Zizzo and Quan Le. (2023). &quot;Certified robustness of static deep learning-based malware detectors against patch and append attacks.&quot; <i>16th ACM Workshop on Artificial Intelligence and Security (AISEC 2023)</i>.'
---
End-to-end malware detectors have been shown to be susceptible to adversarial malware examples, i.e. malicious examples
that have been deliberately manipulated to evade detection. In this work, we present a practical and certifiable defense 
against patch and append attacks on malware detection. Our defense adapts the concept of (de)randomized smoothing to the 
task of malware detection. 

Our defense, instead of taking as input the whole byte sequences, operates on subsequences of bytes. It works as follows:
* During the training phase, a base classifier is trained to make classifications based on a subset of contiguous bytes or chunk of bytes from an executable. 
* At test time, an executable is divided into non-overlapping chunks of fixed size. Then, each chunk is classified independently. 
The final classification is the majority vote over the predicted classes of the chunks.

Leveraging the fact that patch and append attacks can only influence a certain number of chunks, we derive meaningful large
robustness certificates against both attacks. To demonstrate the suitability of our approach, we have trained a classifier
with our chunk-based scheme on the BODMAS dataset. We show that the proposed chunk-based smoothed classifier is more robust
against state-of-the-art evasion attacks in comparison to a non-smoothed classifier.

The following figure illustrates our (de)randomized smoothing scheme:![derandomized smoothing scheme](../images/derandomized_smoothing_scheme.png)