---
title: "A PyCav Course"
layout: post
date: 2016-08-22 11:13
image: '/assets/images/'
description:
tag:
tools: true
blog: true
jemoji:
author: niallmcconville
---

# Introduction

As part of the PyCav project, the team drew upon their experiences of studying Computational Physics at the University of Cambridge in an endeavour to create a new _proof-of-concept_ course centred around Python.

This blog post will outline our motivation for such a course, the course structure we adopted, the content of the course, a discussion of the outcome of the course development, the future work required, and a conclusion to tie the post together.

# Motivation

The motivation for development of this course is best encapsulated in the [PyCav Manifesto](http://pycav.org/pycav-manifesto/).

As of August 2016, the Physics course at Cambridge does not have a Computational Physics course that was developed around Python.
Although, in fairness, the [computational course](http://www.mrao.cam.ac.uk/~dfb/teaching/computationalphysics/) in Part II (the third year) has shifted its weight behind Python.
This represents a direct transition from C++ - perhaps closer to the truth, a translation therefrom. We felt that the consistency derived from working with one language in a course would help students transition to seeing the bigger picture after building confidence and maturity in programming.

One could argue that the Scientific Computing aspects of the (Physical) Natural Sciences Tripos (NST) are quite fragmented.
For example, in Part IA (the first year), one completes a standalone course in MATLAB.
A self-taught, standalone C++ course in Computational Physics is encountered, if one then proceeded to take the Physics B option in Part IB (the second year).
This in some regard, is a result of the flexibility provided by the level of choice available to students in the NST - which itself is highly desirable.
What is undesirable is that this compartmentalisation of teaching creates a horizontal learning environment; that is to say, one finds many occasions where one has to start close to square one, rather than building directly and consistently upon previous years experience. Of course, this is not an absolute rule. It is certainly true that the skill development throughout these courses extends the type of problems that an undergraduate student can tackle. 
The PyCav team felt that a higher level of integration was desirable. 
It was our belief that increased integration across year boundaries would improve feelings of relevance among students as well as providing opportunities for repetition and subsequent advancement of programming and scientific computing concepts.

Finally, we were motivated to use modern development tools without the hurdles that accompany more advanced software development practices. We are Physicists, after all. In part, this was influenced by attempting to reduce the 'cognitive overload' that undergraduates encounter when approaching the field. This decision was based upon our interpretation of discussion from [this paper](http://arxiv.org/abs/1505.05425).

We felt that it was desirable to start from scratch. Thus we created this hypothetical course, which we hope some keen individuals may attempt to learn from.

# Structure

Directly following from our motivation, the course is structured from Part IA to Part II; the Bachelor's components of the course.

On top of this, we split the course into three streams. Each year, the learning focus would shift towards Scientific Computing as fluency increases. These streams are:

* _Programming_: How to program in Python, using the features that the language provides. Additionally, this outlines some of the more abstract concepts associated with programming which are not scientific (at least, physically) in nature.
* _Scientific Computing_: This would use the skills learnt in the _Programming_ stream to help students understand how to use Python to tackle scientific programming challenges.
* _Optional Components_: For students who want to learn more, this stream provides more challenging programming concepts (like OOP and Lambda expressions).

Exercises for this course would be classified in the following way:

<iframe src="http://docs.google.com/gview?url=https://github.com/PyCav/Investigations/raw/master/investigations_framework.pdf&embedded=true" 
style="width:400px; height:400px;" frameborder="0"></iframe>

To balance the load for what is an already intense course, we suggest replacing some exercises on the example sheets for courses with shorter Python problems.

Additionally, we think that the [Demonstrations](https://github.com/PyCav/Demos) that we have produced could be used in lectures. These would effectively be open source, allowing students to view the code for some physics examples. This is in eeping with the PyCav ethos of unification.

# Content

You can view the course content on the [Course GitHub](https://github.com/PyCav/Course).

An outline of the course syllabus, as well as the divisions across year groups and content is presented in the table below. The Part II material, while it exists is currently distributed in the [Investigations](https://github.com/PyCav/Investigations) repository. This is due to our focus on the earlier years which don't have any Python teaching at all.

|               |     Part IA       |     Part IB       |      Part II      |      
| ------------- | ------------- | ------------- | ------------- |
|  **Programming**  |      [Algorithms](http://nbviewer.jupyter.org/github/PyCav/Course/blob/master/IA/Lessons/1.1.Algorithms.ipynb)       |      [Recap](http://nbviewer.jupyter.org/github/PyCav/Course/blob/master/IB/Lessons/2.1%20Advanced%20functions%20and%20loops.ipynb)      |       Random Numbers     |
|               |      [Variables & Types](http://nbviewer.jupyter.org/github/PyCav/Course/blob/master/IA/Lessons/1.2.Variables.ipynb)       |      [Adv. Algorithms](http://nbviewer.jupyter.org/githu/PyCav/Course/blob/master/IB/Lessons/2.2%20Advanced%20algorithms.ipynb)      |       Floating Point Numbers     |
|               |      [Lists & Loops](http://nbviewer.jupyter.org/github/PyCav/Course/blob/master/IA/Lessons/1.3.Control%20Flow.ipynb)       |      [Modules](http://nbviewer.jupyter.org/github/PyCav/Course/blob/master/IB/Lessons/2.4%20Make%20your%20own%20library.ipynb)       |       Errors      |
|               |      [Functions](http://nbviewer.jupyter.org/github/PyCav/Course/blob/master/IA/Lessons/1.4.Functions%20Methods.ipynb) & [Libraries](http://nbviewer.jupyter.org/github/PyCav/Course/blob/master/IA/Lessons/1.5.%20Libraries.ipynb)       |      [Introduction to OOP](http://nbviewer.jupyter.org/github/PyCav/Course/blob/master/IB/Lessons/2.3%20OOp.ipynb)       |       Recursion     |
|  **Scientific Computing** |      [Euler Step](http://nbviewer.jupyter.org/github/PyCav/Course/blob/master/IA/SciComp/Euler%20method.ipynb)       |      Further Simulation Techniques      |       ODEs      |
|               |      [Plotting](http://nbviewer.jupyter.org/github/PyCav/Course/blob/master/IA/SciComp/plot_ex2.ipynb)      |      Singular Value Decomposition       |       PDEs      |
|               |      [Integration by the Trapezium Rule](http://nbviewer.jupyter.org/github/PyCav/Course/blob/master/IA/SciComp/int_ex.ipynb)       |      Eigenanalysis      |       FFT      |
|               |      [Importing & Analysing Data](http://nbviewer.jupyter.org/github/PyCav/Course/blob/master/IA/SciComp/importingdata.ipynb)       |      Monecarlo Methods       |       Additional Signal Processing | 
| | | Central Limit Theorem | |
| **Optional** | [Comments & Coding Style](http://nbviewer.jupyter.org/github/PyCav/Course/blob/master/IA/Extra/GoodPractices.ipynb) | [$\lambda$ functions](http://nbviewer.jupyter.org/github/PyCav/Course/blob/master/IB/Extra/2.Optional%20-%20Lambdas.ipynb) | Alternative OSes & Hardware |
|  |  | [Gotchas](http://nbviewer.jupyter.org/github/PyCav/Course/blob/master/IB/Extra/2.Optional-%20Common%20mistakes%20in%20python.ipynb) | Optimisation/Cython |
|  |  | Animations | |
|  |  | Debugging |  | 

# Discussion

The proposed course structure does go someway towards resolving some of the issues mentioned in the motivation. Where applicable, lessons were designed with a 'Theory' followed by 'Practice' section. We think that viewing examples first, followed by exercises that step to one side of the material are useful for easing students into new concepts.

As for the content, the early programming courses aim to introduce people to thinking about processes, a key step in translating thoughts and intentions into programs. The OOP lesson aims to introduce the concept to students while keeping it relevant for a physics student.

An area where we agreed that we were deficient is that of data analysis. Thus we think that more focus could be placed on teaching students how to use data analysis packages such as ROOT which are currently being used by modern institutions (namely CERN). Additionally, it would be apt for Python to be used in data analysis in the Part IB and Part II labs. The current structure of experimental classes is largely the domain of the Heads of Class and thus would require a joint decision to move in that direction. Currently, it seems, Excel and MATLAB are the most popular software implementations in the Teaching Labs at the Cavendish and it would requirethe establishment and overcoming a transitionary period, which is easier said than done. On top of this, the presiding language agnosticism of the Part II labs affords some students the flexibility to conduct experiments as they see fit, which is worth considering.

# Future Work

*It doesn't matter how beautiful your theory is, it doesn't matter how smart you are. If it doesn't agree with experiment, it's wrong.* <br> R.P. Feynman.

Hopefully without sounding too much like a EULA, we can note that this course is **untested**. We had many thoughts about what was right and what was wrong about the way we were taught computational physics. It would not be in keeping with the exercise of our critical capacity to suggest that it is the *right* way to teach computational physics. Good practice requires good evidence. Thus, the future of such a course lies in testing it, gathering meaningful feedback from those who participate in it, and measuring whether or not it improves the understanding of scientific computation in the NST.

A starting point for this may be to draw upon the UCL experience in their 2016 paper on the matter (referenced above).

In terms of the development of the course (as opposed to the above, which concerns measurement of effectiveness), pursuing better integration into the degree course would be desirable. So far we have only created a course with some content but haven't worried about questions like:

* Who is teaching it?
* When are they teaching it?
* How are they teaching it?

Engaging with lecturers and students to further develop an enjoyable course would be ideal. To an extent, this is already happening.

Testing will also need to be done with the _nbgrader_ software. The backend was setup and configured for use with the University of Cambridge auth systems - apart from this, no rigorous testing was conducted.

More work on Data Analysis would be highly desirable.
