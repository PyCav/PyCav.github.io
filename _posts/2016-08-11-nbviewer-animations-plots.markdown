---
title: "Animations and Interactive Plots"
layout: post
date: 2016-08-11 12:13
description:
tag:
tools: true
blog:
jemoji:
author: aidancrilly
---

Jupyter Notebooks can used to run code within the [server](https://nile.pycav.org/) or locally however they can also be used to present the output of the code.
This could include figures, animations, parameter estimations etc. along with the markdown comments and LaTeX equations. Running the code to produce these when
presenting could include unwanted setup and delay. However the notebooks, along with the desired material, can be view in an internet browser using 
[NBViewer](https://nbviewer.jupyter.org) without the need to run any code.

Some examples produced from the PyCav Project, click the images to view the demonstrations:

<figure>
    <center><a href="https://nbviewer.jupyter.org/github/PyCav/Demos/blob/master/Dynamics/charge_torus.ipynb">
       <img src="/assets/images/nbviewerthumbs/charged_torus.png" alt="Electrodynamics: Charged Particle Motion near Fixed Charges">
    </a></center>
<figcaption>
    Electrodynamics: Charged Particle Motion near Fixed Charges
</figcaption>
</figure>

<figure>
    <center><a href="https://nbviewer.jupyter.org/github/PyCav/Demos/blob/master/Electromagnetism/Cherenkov.ipynb">
       <img src="/assets/images/nbviewerthumbs/cherenkov.png" alt="Electromagnetism: Cherenkov Radiation">
    </a></center>
<figcaption>
    Electromagnetism: Cherenkov Radiation
</figcaption>
</figure>
<figure>
    <center><a href="https://nbviewer.jupyter.org/github/PyCav/Demos/blob/master/WavesAndOscillations/FoldyLax.ipynb">
       <img src="/assets/images/nbviewerthumbs/foldy_lax.png" alt="Steady State Scattering: Foldy Lax">
    </a></center>
<figcaption>
    Steady State Scattering: Foldy Lax
</figcaption>
</figure>

<figure>
    <center><a href="https://nbviewer.jupyter.org/github/PyCav/Demos/blob/master/FluidDynamics/LatticeBoltzmann.ipynb">
       <img src="/assets/images/nbviewerthumbs/latticeboltzmann.png" alt="Fluid Dynamics: Flow onto a barrier via Lattice Boltzmann Method">
    </a></center>
<figcaption>
    Fluid Dynamics: Flow onto a barrier via Lattice Boltzmann Method
</figcaption>
</figure>
<figure>
    <center><a href="https://nbviewer.jupyter.org/github/PyCav/Demos/blob/master/WavesOscillations/numerical_wave_equation.ipynb">
       <img src="/assets/images/nbviewerthumbs/numerical_wave_equation.png" alt="Wave Equation: 1D & 2D">
    </a></center>
<figcaption>
    Wave Equation: 1D & 2D
</figcaption>
</figure>
<figure>
    <center><a href="https://nbviewer.jupyter.org/github/PyCav/Investigations/blob/master/LongProblems/shooting_method.ipynb">
       <img src="/assets/images/nbviewerthumbs/shooting_method.png" alt="Time-Independent QM: Shooting Method for Finite Square Well">
    </a></center>
<figcaption>
    Time-Independent QM: Shooting Method for Finite Square Well
</figcaption>
</figure>
<figure>
    <center><a href="https://nbviewer.jupyter.org/github/PyCav/Demos/blob/master/QuantumMechanics/split_step_schrodinger.ipynb">
       <img src="/assets/images/nbviewerthumbs/split_step_schroedinger.png" alt="Time-Dependent QM: 1D Barriers & Harmonic Potentials">
    </a></center>
<figcaption>
    Time-Dependent QM: 1D Barriers & Harmonic Potentials
</figcaption>
</figure>

A tutorial on how to use the PyCav display module can be found [here](https://nbviewer.jupyter.org/github/PyCav/Demos/blob/master/Animation/Inline_animation_tutorial.ipynb).

Animations are produced using matplotlib but plots can be produced by both matplotlib and bokeh. An advantage of bokeh is that when the notebook 
is viewed in the browser it allows for the plot tools such as zoom to be used, while matplotlib does not. However its documentation is not as extensive.
