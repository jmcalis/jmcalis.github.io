---
title: "Coordination through nonlinear nonlocal diffusion"
excerpt: "Code for the numerical approximation of solutions to the continuous coordination non-local equation.<br/><img src='/images/CPTfigure.png'>"
collection: portfolio
---

[Link to the repository ](https://github.com/feffermanlab/JSM_2024_ContinuousCoordination)

<img src='/images/ICfigure.png'>
<img src='/images/CPTfigure.png'>

<i>When the radius of recognition in the strategy space is limited, players form discrete bands of strategies at equilibrium.</i> 

Code for the numerical approximation of solutions to the continuous coordination non-local equation as described in [this manuscript](http://jmcalis.github.io/files/McAlister2025d.pdf)

There is one function and two matlab scripts in this repository.

The function is <code>CoordSolve.m</code>. This is the numerical method which approximates the solution to the IVP described in the associated manuscript by a first order forward difference method with simple righthand quadrature

The script <code>NumericalExperiments.m</code> uses the function to investigate the behavior of solutions in four different ways described in the associated manuscript. It is not very useful beyond generating figures

The script <code>ContinuousCoordinationSim2D.m</code> is more flexible and can be used to animate solutions to the IVP in 2D To use this code, find where the initial condition, familiarity kernel, and recogntion functions are included in the code. If you wish to change any of these, replace them. (You cannot use a singular kernel). When you are ready to approximate your soluiton, run the sript and see the surface changes in the animation window 'figure 1'.

Currently this code only supports the free boundary problem and does not approximate solutions to the initial boundary value problem. The theory behind the boundary value problem is not well understood.

For more information on the theory, read the associated manuscript. It is likely that the only way that you are reading this readme file is because you have already begun to read the associated manuscript but if not, go read it.