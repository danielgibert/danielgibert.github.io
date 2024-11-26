---
title: "Certified Adversarial Robustness of Machine Learning-based Malware Detectors via (De) Randomized Smoothing"
collection: publications
category: manuscripts
permalink: /publication/2024-ArXiv-DeRandomizedSmoothing
date: 2024-04-01
excerpt: 'This paper extends our AISEC paper with a preprocessing step that allows us to provide robustness certificates against patch, append, and content injection attacks.'
venue: 'ArXiv'
paperurl: 'https://arxiv.org/abs/2405.00392' #Add here link to paper
citation: 'Daniel Gibert, Luca Demetrio, Giulio Zizzo, Quan Le, Jordi Planes, Battista Biggio. (2024). &quot;Certified Adversarial Robustness of Machine Learning-based Malware Detectors via (De) Randomized Smoothing.&quot; <i>ArXiv</i>'
---

This paper extends our AISEC paper by:
* Introducing a preprocessing step that allows us to provide determinitstic robustness certificates against patch, append, and content injection attacks. 
* Extending the evaluation to four neural network architectures, i.e. MalConv, MalConvGCT, AvastConv, and ShallowConv.
* Comparing our defense with adversarial defenses based on randomized smoothing against SOTA functionality-preserving attacks.
* Showing how the proposed smoothing scheme can be used to facilitate a finer-grained analysis of a PE file, identifying 
specific chunks within the file that exhibit malicious traits.