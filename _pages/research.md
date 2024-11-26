---
permalink: /research
title: "Research"
author_profile: true
redirect_from: 
  - /research/
  - /research.html
---

My main area of research lies at the intersection of Machine Learning (ML) and Information Security. 
My work has focused on building, attacking, and defending malware detectors.

Adversarial Attacks and Defenses for Malware Detection
======
I am currently conducting research on attacks and defenses for malware detection. Machine learning models are vulnerable to adversarial attacks - attacks that intentionally manipulate the input data to cause the model to misclassify or produce incorrect outputs.
Machine learning-based malware detectors are no exception. 

I have developed methods to attack feature-based detectors without having to query the target detector and without requiring knowledge of the model's parameters using [Generative Adversarial Networks (GANs)](/publication/2023-IEEE-Security-And-Privacy-Workshops). 

I have developed methods to defend against adversarial attacks on end-to-end malware detectors based on:
- [Randomized smoothing](/publication/2024-ESORICS-RandomizedSmoothing).
- [(De)randomized smoothing](/publication/2024-IEEEAccess-DeRandomizedSmoothing) 

I have proposed the [first deterministic robustness certificate for end-to-end malware detectors](/publication/2024-AISEC-DeRandomizedSmoothing) and I have investigated the limitations of static machine learning-based detectors against [packing](/publication/2024-Packing).

Machine Learning for Malware Detection and Classification
======
During my PhD, I focused on the design, implementation, and evaluation of ML-based approaches for the task of malware classification. I developed methods to classify malware based on:
- [Assembly code of the binary files](/publication/2017-CNN-Opcodes).
- [Structural entropy representation of the binary files](/publication/2018-StructuralEntropy).
- [Grayscale images of the binary files](/publication/2020-Grayscale-Images-CNN).
- [Hand-crafted features and deep learning](/publication/2020-HYDRA).