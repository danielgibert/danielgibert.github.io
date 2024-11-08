---
title: "Fusing feature engineering and deep learning: A case study for malware classification"
collection: publications
category: manuscripts
permalink: /publication/2022-FusingFeatureEngineeringAndDeepLearning
date: 2022-11-30
excerpt: 'In this work, we present an hybrid system for malware classification that combines feature engineering and deep learning using an early-fusion mechanism.'
venue: 'Journal Expert Systems With Applications'
paperurl: 'https://www.sciencedirect.com/science/article/pii/S0957417422011927' #Add here link to paper
citation: 'Daniel Gibert, Jordi Planes, Carles Mateu, Quan Le. (2022). &quot;Fusing feature engineering and deep learning: A case study for malware classification.&quot; <i>Journal Expert Systems With Applications</i>.'
---

While traditional feature-based approaches rely on the manual design of hand-crafted features based on experts’ 
knowledge of the domain, deep learning approaches replace the manual feature engineering process by an underlying system, 
typically consisting of a neural network with multiple layers, that perform both feature learning and classification altogether.

In this paper we present an hybrid approach to address the task of malware classification by fusing multiple types of 
features defined by experts and features learned through deep learning from raw data. 

In particular, our approach relies on deep learning to extract N-gram like features from the assembly language instructions
and the bytes of malware, and texture patterns and shapelet-based features from malware’s grayscale image representation
and structural entropy, respectively. 

These deep features are later passed as input to a gradient boosting model that combines the deep features and the
hand-crafted features using an early-fusion mechanism. 

![FusingFeatureEngineeringAndDeepLearningMethod.jpg](../images/FusingFeatureEngineeringAndDeepLearningMethod.jpg)

The suitability of our approach has been evaluated on the Microsoft Malware Classification Challenge benchmark and 
results show that the proposed solution achieves state-of-the-art performance and outperforms gradient boosting and
deep learning methods in the literature.

![table_results_fusing.png](../images/table_results_fusing.png)