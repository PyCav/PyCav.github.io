---
title: "Numerical Techniques"
layout: post
date: 2016-09-06 11:13
image: '/assets/images/'
description:
tag:
tools: true
blog: true
jemoji:
author: aidancrilly
---

One of the advantages of Python is the selection of libraries which greatly simplify complex tasks. For example NumPy allows for matrix multiplication and other vector operations as well as more complex operations such as eigenvalue evaluation which for other languages may require additional set up (such as workspaces in fortran).

For numerical techniques for solving ODEs, SciPy provides the general [odeint function](http://docs.scipy.org/doc/scipy/reference/generated/scipy.integrate.odeint.html) which can integrate a system of differential equations in a single line. In the background it calls from the fortran odepack, thus making it quick but only requires minimal boilerplate to call (unlike GSL as used in the current C++ course).

Many numerical algorithms, namely finite difference methods, require looping over grid points. In Python this would be excessively slow ([video showing looping comparison with explanation](https://youtu.be/EEUXKG97YRw?t=4m31s)), however using the NumPy library C/C++ and fortran operations can speed up such tasks by pushing repeated operations into compiled code (also shown in video). Now loops can be replaced by slicing and indexing, all done within a single line. Although not strictly faster than a low-level language equivalent, the time saved in writing the Python version using NumPy to replace the loops can make for an efficient program.

From the students perspective, the simplicity of these Pythonified algorithms allows for more to be investigated. For example, rather than spending time trying to figure out how to handle the output of a Fast Fourier Transform, NumPy and SciPy provide the fftshift function to place the zero frequency at the origin. This would give students more time to investigate complex diffraction patterns and think about the Physics while using the code as a tool.

Hopefully the reduced debugging and writing time would allow for different physical situations and therefore different numerical algorithms to be used. This would show that there is more to life than RK4.

Below we shall point to some Demo notebooks using particular numerical algorithms as well as resources providing explanation of the technique

## Algorithms and Resources

### From SciPy and NumPy:

|scipy.odeint|[Gyroscope](http://nbviewer.jupyter.org/github/PyCav/Demos/blob/master/Dynamics/gyroscope.ipynb)|[odeint](http://docs.scipy.org/doc/scipy/reference/generated/scipy.integrate.odeint.html)|
|scipy.quad|[Perturbation Theory](http://nbviewer.jupyter.org/github/PyCav/Investigations/blob/master/LongProblems/perturbation_theory_solutions.ipynb)|[quad](http://docs.scipy.org/doc/scipy/reference/generated/scipy.integrate.quad.html)|
|numpy.eig|[Linear Chain](http://nbviewer.jupyter.org/github/PyCav/Demos/blob/master/Eigensystems/LinearChain.ipynb)|[eig](http://docs.scipy.org/doc/numpy/reference/generated/numpy.linalg.eig.html)|

### Established Numerical Techniques written in Python:

|Lax & Lax-Wendroff|[Wave Equation](http://nbviewer.jupyter.org/github/PyCav/Demos/blob/master/WavesAndOscillations/numerical_wave_equation.ipynb)|Numerical Recipes: The Art of Scientific Computing Book, [Solving PDEs numerically](http://www.aei.mpg.de/~rezzolla/lnotes/Evolution_Pdes/evolution_pdes_lnotes.pdf) & [Algorithm summaries in 1D and 2D](http://homepage.univie.ac.at/franz.vesely/cp_tut/nol2h/new/c5pd_s1ih.html)|
|Split Step Fourier method|[Reflectionless Potential](http://nbviewer.jupyter.org/github/PyCav/Demos/blob/master/QuantumMechanics/1D_reflectionless_potential.ipynb)|[Quantum Python](https://jakevdp.github.io/blog/2012/09/05/quantum-python/) & [Split-step wiki](https://en.wikipedia.org/wiki/Split-step_method)|
|Shooting method|[Finite Square Well](http://nbviewer.jupyter.org/github/PyCav/Investigations/blob/master/LongProblems/shooting_method.ipynb)|[Numerov Method](http://www.fisica.uniud.it/~giannozz/Corsi/MQ/LectureNotes/mq-cap1.pdf)|
|Monte-Carlo|[Bateman Equation](http://nbviewer.jupyter.org/github/PyCav/Demos/blob/master/Statistics/Bateman_Eqn.ipynb)|[Monte Carlo wiki](https://en.wikipedia.org/wiki/Monte_Carlo_method) (see also Ising model notebooks for Metropolis algorithm)|
|Lattice Boltzmann|[Flow onto a barrier](http://nbviewer.jupyter.org/github/PyCav/Demos/blob/master/FluidDynamics/LatticeBoltzmann.ipynb)|[LBM](http://physics.weber.edu/schroeder/javacourse/LatticeBoltzmann.pdf)|
and others

### Custom Algorithms:

|Cherenkov Radiation|[Notebook](http://nbviewer.jupyter.org/github/PyCav/Demos/blob/master/Electromagnetism/Cherenkov.ipynb)|	|
|Light Ray Caustic|[Caustic](http://nbviewer.jupyter.org/github/PyCav/Demos/blob/master/Optics/Caustics.ipynb)|[Ray Transfer Matrix Analysis](https://en.wikipedia.org/wiki/Ray_transfer_matrix_analysis) & [PyCav Optics Docs](http://pycav.readthedocs.io/en/latest/api/optics/index.html)|