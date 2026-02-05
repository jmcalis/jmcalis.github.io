---
title: "Continuous Coordination in the Plane"
excerpt: "A collection of code used for the visualization and analysis of the structured coordination game with a continuous player space in the plane.<br/><img src='/images/CircleConsensus.png'>"
collection: portfolio
---

[Link to the repository ](https://github.com/jmcalis/JSM_2026_DualCoordination/releases/tag/v1.0.0)

<img src='/images/FigureRandomNonConsensus.gif'>

<i>When each point in space it picking a strategy to coordinate with those around it in a vanishingly small neighborhood, a rich set of dynamics emerge.</i> 

A collection of code used for the visualization and analysis of the structured coordination game in the dual setting. The structured coordination game is typically understood by examining strategy profiles. By examining the boundaries of strategy profiles instead, the game can be understood in a different light. Although the dual concept does not give us any additional numerical power in the discrete case, in the continuous case, considering the boundaries of strategic communities can be exceptionally powerful, especially in the setting where individuals only interact with a vanishingly small area of players around them. The code in this repository is used to visualize and analyze the continuous version of the coordination game.

This repository contains code to simulate these continuous dynamic games through myopic best response in order to understand the flows of their boundaries.  <code>ContinuousDualCoordination.m</code> is a set of functions which can be used to simulate and visualize the Myopic Best Response in this setting. <code>CurvatureLimit.m</code> is a script intended to give numerical support for a particular limit written about in the associated manuscript. Finally, <code>LimitAttempt1.nb</code> is a Mathematica notebook describing attempts to prove the same limit.