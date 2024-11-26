---
title: "Assessing the Impact of Packing on Machine Learning-Based Malware Detection and Classification Systems"
collection: publications
category: manuscripts
permalink: /publication/2024-Packing
date: 2024-10-01
excerpt: 'In this paper we investigate the impact of packing on the performance of machine learning-based malware detection and classification systems.'
venue: 'ArXiV'
paperurl: 'https://arxiv.org/abs/2410.24017' #Add here link to paper
citation: 'Daniel Gibert, Nikolaos Totosis, Constantinos Patsakis, Giulio Zizzo, Quan Le. &quot;Assessing the Impact of Packing on Machine Learning-Based Malware Detection and Classification Systems.&quot; <i>ArXiV</i>.'
---
The proliferation of malware, particularly through the use of packing, presents a significant challenge to static analysis and
machine learning-based malware detectors. Packing is a technique used by malware authors to obfuscate the code of their
malicious software, making it harder for security analysts to understand and classify the malware. Packing affects the features and
patterns that machine learning-based malware detectors rely on. However, little research has been done to understand the impact
of packing on the performance of machine learning-based malware detection and classification systems. This paper addresses this gap
by investigating the impact of packing on the performance of static machine learning-based models for malware detection and classification.

This work aism to answer the following research questions:
- Does a bias in the distribution of packers used in benign and malicious executables cause malware detectors
to learn "benign" and "malicious" packing routines? How does a bias in the distribution of packers affect
malware classifiers?
- Do packers limit the applicability of static machine learning-based malware detectors and classifiers? What
effort is required to bypass detection or raise false flags in malware detectors and cause a misclassification in
malware classifiers?

To address these questions, this paper we make the following contributions:
- We conduct an extensive analysis of the bias in the distribution of packers used in benign and malicious
executables, demonstrating how this bias influences the learning process of malware detectors. Our findings
reveal that malware detectors can indeed develop a reliance on specific packing routines as indicators of benign
or malicious behaviour, or among malware families, which can significantly impact their performance and
reliability
- We provide a detailed study of the performance of static machine learning-based malware detectors and
classifiers, including feature-based detectors, end-to-end detectors, and greyscale image-based detectors, when
subjected to packing techniques, and we identify scenarios where packers successfully bypass detection or
trigger false positives.
- We examine how 8 different packers and obfuscation tools affect the performance of static machine learning-based malware detectors and classifiers,
including well-known executable file compressors such as UPX and
MPress, crypters such as Hyperion, protectors such as Enigma and Themida, and obfuscation tools such as
Mangle. Through a series of experiments, we demonstrate which packing techniques are more effective against
each type of detector, highlighting the limitations of static detectors against obfuscated executables.