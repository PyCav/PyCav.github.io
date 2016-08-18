---
title: "Animations and Interactive Plots"
layout: post
date: 2016-08-11 12:13
image: '/assets/images/'
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

Some examples produced from the PyCav Project:

[Steady State Scattering: Foldy Lax](https://nbviewer.jupyter.org/github/PyCav/Demos/blob/master/WavesAndOscillations/FoldyLax.ipynb)

[Wave Equation: 1D and 2D examples](https://nbviewer.jupyter.org/github/PyCav/Demos/blob/master/WavesAndOscillations/numerical_wave_equation.ipynb)

[Time-Dependent QM: 1D examples, barrier and harmonic potentials](https://nbviewer.jupyter.org/github/PyCav/Demos/blob/master/QuantumMechanics/split_step_schrodinger.ipynb)

[Fluid Dynamics: Flow onto a barrier via Lattice Boltzmann Method](https://nbviewer.jupyter.org/github/PyCav/Demos/blob/master/FluidDynamics/LatticeBoltzmann.ipynb)

[Electromagnetism: Cherenkov radiation](https://nbviewer.jupyter.org/github/PyCav/Demos/blob/master/Electromagnetism/Cherenkov.ipynb)

[Time-Independent QM: Shooting Method for finite square well](https://nbviewer.jupyter.org/github/PyCav/Investigations/blob/master/LongProblems/shooting_method.ipynb)

[Electrodynamics: Charged particle motion near fixed charges](https://nbviewer.jupyter.org/github/PyCav/Demos/blob/master/Dynamics/charge_torus.ipynb)

A tutorial on how to use the PyCav display module can be found [here](https://nbviewer.jupyter.org/github/PyCav/Demos/blob/master/Animation/Inline_animation_tutorial.ipynb).

<figure>
    <a href="https://nbviewer.jupyter.org/github/PyCav/Demos/blob/master/QuantumMechanics/split_step_schrodinger.ipynb">
       <img src="../images/nbviewerthumbs/split_step_schroedinger.png" alt="Time-Dependent QM: 1D Barriers & Harmonic Potentials">
    </a>
<figcaption>
    Time-Dependent QM: 1D Barriers & Harmonic Potentials
</figcaption>
</figure>

Animations are produced using matplotlib but plots can be produced by both matplotlib and bokeh. An advantage of bokeh is that when the notebook 
is viewed in the browser it allows for the plot tools such as zoom to be used, while matplotlib does not. However its documentation is not as extensive.
