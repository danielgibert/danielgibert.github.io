---
title: "Auditing static machine learning anti-Malware tools against metamorphic attacks"
collection: publications
category: manuscripts
permalink: /publication/2021-ML-Classifiers-VS-Metamorphic-Techniques
date: 2021-02-01
excerpt: 'This paper presents an exhaustive evaluation of the state-of-the-art approaches for malware classification against common metamorphic attacks.'
venue: 'Journal Computers & Security'
paperurl: 'https://www.sciencedirect.com/science/article/abs/pii/S0167404820304326' #Add here link to paper
citation: 'Daniel Gibert, Carles Mateu, Jordi Planes, Joao Marques-Silva. (2021). &quot;Auditing static machine learning anti-Malware tools against metamorphic attacks.&quot; <i>Journal Computers & Security</i>.'
---
This paper presents an exhaustive evaluation of the state-of-the-art approaches for malware classification against common metamorphic attacks. 

The metamorphic techniques investigated in this work include:
* Dead code insertion.
* Register reassignment.
* Subroutine reordering.
* Code reordering through jumps.

The machine learning-based classifiers evaluated include:
* MalConv: Raff et al. 2018. "Malware Detection by Eating a Whole EXE". AAAI Workshops 2018
* AvastConv: Krčál et al. 2018: "Deep Convolutional Malware Classifiers Can Learn from Raw Executables and Labels Only". ICRL Workshops 2018. 
* ShallowConv: Gibert et al. 2017. "Convolutional neural networks for classification of malware assembly code". CCIA 2017.
* Structural entropy-based CNN: Gibert et al. 2018. "Structural entropy-based convolutional neural networks for malware classification". IIAI-AAAI 2018.
* Logistic regression + N-Gram features