---
title: "The PyCav Library"
layout: post
date: 2016-08-05 10:44
image: '/assets/images/'
description:
tag:
blog: true
jemoji:
author: aidancrilly
---

The PyCav library consists of an ever-growing number of modules that proved useful in creating demonstrations, which any user could use through a simple set of functions and objects. It allows for easy creation and visualization of simulations ranging from a number of classical particles in a box to solving the time dependent Schrodinger equation.

The library has been made readily available on PyPI in the hopes that students and others can use it readily, making computer simulations an integral part of the learning experience. 

To install the PyCav Library, one can use the pip install command in Terminal/Command Line:

    pip install pycav

The project is also open sourced on [GitHub](https://github.com/PyCav/PyCav-Library, "PyCav library on GitHub"), and we hope that the more capable students will not only use, but also start contributing to the library.

### A Quick Tour of PyCav

#### Documentation

In depth documentation of PyCav's usage and implementation can be found [here](http://pycav.readthedocs.io/en/latest/api/index.html)

#### [Classic Mechanics](http://pycav.readthedocs.io/en/latest/api/mechanics/index.html)

This module contains particle, which can interact through user-defined force laws, and spring objects which can connect particle objects

This allows a large number of dynamical systems to be simulated e.g. resonance and gravitational interactions

Large numbers of particles can be used to model a gas, ideal or interacting.

#### [Quantum Mechanics](http://pycav.readthedocs.io/en/latest/api/quantum/index.html) (Time Independent)

This module includes the capability to:

1. Find the stationary states and energy eigenvalues of a potential via the shooting method

2. First order time independent perturbation theory for known unperturbed wavefunctions and eigenvalues

3. Plot the unperturbed and perturbed energy levels along the perturbed potential

#### [Partial Differential Equations](http://pycav.readthedocs.io/en/latest/api/pde/index.html)

Methods for solving the following PDEs numerically are included in the pde module:

1. Wave Equation - $ \ddot{\psi} = c^2 \nabla^2 \psi $

2. Heat Equation - $ \dot{\psi} = D \nabla^2 \psi $

3. Time-Dependent Schrödinger Equation - $ \hat{H} \psi = i \hbar \dot{\psi} $

#### [Geometric Optics](http://pycav.readthedocs.io/en/latest/api/optics/index.html)

Contains ray object for observing refraction into another medium. Other functions included allow to observe caustics caused by refraction