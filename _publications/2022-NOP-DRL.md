---
title: "Enhancing the insertion of NOP instructions to obfuscate malware via deep reinforcement learning"
collection: publications
category: manuscripts
permalink: /publication/2022-NOP-DRL
date: 2022-05-01
excerpt: 'This paper explores the vulnerability of classifiers against the dead code insertion technique and it poposes a reinforcement learning framework to bypass malware classifers'
venue: 'Journal Computers & Security'
paperurl: 'https://arxiv.org/abs/2405.00392' #Add here link to paper
citation: 'Daniel Gibert, Matt Fredrikson, Carles Mateu, Jordi Planes, Quan Le. (2022). &quot;Enhancing the insertion of NOP instructions to obfuscate malware via deep reinforcement learning.&quot; <i>Journal Computers & Security</i>.'
---

It has been shown that machine learning models, in particular deep neural
networks, lack robustness against crafted inputs (adversarial examples). In this work, we have investigated the vulnerability of a
state-of-the-art shallow convolutional neural network malware classifier against the dead code insertion technique.

We propose a
general framework powered by a Double Q-network to induce misclassification over malware families. The framework trains an
agent through a convolutional neural network to select the optimal positions in a code sequence to insert dead code instructions so
that the machine learning classifier mislabels the resulting executable.

![DRL-MalwareEvasion.png](../images/DRL-MalwareEvasion.png)

The experiments show that the proposed method significantly
drops the classification accuracy of the classifier to 56.53% while having an evasion rate of 100% for the samples belonging to the
Kelihos_ver3, Simda, and Kelihos_ver1 families. In addition, the average number of instructions needed to mislabel malware in
comparison to a random agent decreased by 33%.