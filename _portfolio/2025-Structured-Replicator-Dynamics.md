---
title: "Structured Replicator Dynamics"
excerpt: "Code for the analysis and visualization of replicator dynamics with explicit relational structure in continuous time for both continuous and discrete player spaces.<br/><img src='/images/StructuredReplicatorImage.png'>"
collection: portfolio
---

[Link to the repository ](https://github.com/feffermanlab/JSM_2025_StructuredReplicatorDynamics)

<img src='/images/StructuredReplicatorImage.png'>

<i>When four neighbors connected in a path each play rock paper scissors against eachother simultainously, the mixture of strategies that each players uses meanders around the phase space in a way that seems chaotic.</i> 

Code for the analysis and visualization of replicator dynamics with explicit relational structure in continuous time for both continuous and discrete player spaces. As it exists now, this code can be used to investigate the dynamics of replicator dynamics where each individual uses a mixed strategy and local information is pereseved throughout.

The ODE and Nonlocal systems are described in a manuscript that will be linked here once the preprint is up:

In StructuredReplicator.m and StructuredReplicatorTer.m solutions to the problem in a discrete player space are solved and visualized. StructuredReplicatorTer.m does the visualizaion through ternery plots while StructuredReplicator.m visualizes the time axis explicitly. continuousspacereplicator1D.m Solves the nonlocal IVP in one spatial dimension and visualized it as a .fig animation.

connectionstrength.m and edgesensitivity.m are used to investigate how edge removal, addition, or weight perturbation can change the stability of different strategy profiles. The former can be used to understand the connection between two modules but it is made obsolete by the latter which can be used for general adjacency matricies

potentialfunction.m is a short script meant to visualize the potential function of the two player coordination or anticoordination game from game theoretic principles although it can be easily computed analytically and plotted far easier.