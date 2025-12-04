---
title: "Discrete stuctured coordination"
excerpt: "A collection of tools for the analysis of an n-player, n-strategy coordination game on a network with neutral options. Considering the game as a dynamical system we describe orbits, equilibria, and stability.<br/><img src='/images/DiscreteStructuredImage.png'>"
collection: portfolio
---

[Link to the repository ](https://github.com/feffermanlab/JSM_2024_StructuredCoordination)

<img src='/images/DiscreteStructuredImage.png'>

<i>A non-consensus equilibrium in a coordination game on an asymmetric network.</i>

This repository contains a collection of tools for the analysis of an \\(n\\)-player, \\(n\\)-strategy coordination game on a network with neutral options. 
Considering the game as a dynamical system we describe orbits, equilibria, and stability.  

The Class <code>Orbit</code> is a (non-unique) solution to the initial value problem. Given a initial strategy profile (which will later be thought of as partitions) and a graph, an instance of the class is produced by solving the IVP with the best response replicator dynamic. The solution is a list of arrays which represent the strategy each vertex in the graph is taking on at that time step. 

Using the <code>Orbit</code> class we can describe equilibrium partitions (which are those partitions corresponding to equilibrium strategy profiles). <code>SCCatalogue.py</code> runs a script to find all equilibrium partitions among connected graphs in the networkx Graph Atlas. 

<code>SCBasinSim.py</code> is a script which generates a random array of graphs and estimates the size of the basin of stability for the consensus equilibrium It has been parallelized to be run with the shell script <code>JobBasinSim.srun.sh</code>
Likewise, <code>SCBroadSim.py</code> is a script which generates a random array of graphs and measures their limiting behavior. It also has been parallelized to run with the shell script <code>JobBroadSim.srun.sh</code>.
The python script and shell script <code>DataCollect.py</code> and <code>JobDataCollect.srun.sh</code> take the slices of simulation data from the simulations mentioned above are compile it into one process. 

<code>PartitionTools.py</code> is a collection of tools which are used in the simulations to measure partitions

<code> SCCatalogue.py, SCBasinSim.py, SCBroadSim.py,</code> and <code>PartitionTools.py</code> all depend on <code>Orbit.py, SCBasinSim.py</code> and <code>SCBroadSim.py</code> depends on <code>PartitionTools.py</code>

The Jupiter Notebook <code>McAlisterProjectDemo.ipynb</code> steps through the functionality of the <code>Orbit </code>class. (note the visualizations are not supported on when run in VScode)