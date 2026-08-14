---
layout: page
permalink: /repositories/
title: research
description: This page provides an overview of some of my research projects.
nav: true
nav_order: 3
---


## Research Overview

My research sits at the boundary of computational mathematics and machine learning. I am broadly interested in developing mathematically principled algorithms for scientific machine learning tasks. A recurring theme in my work is the use of tools from one field to answer questions in another, borrowing ideas from topology optimization to inform neural network design, adaptive finite element strategies to drive network growth, and dynamical systems theory to design and theoretically analyze neural surrogates for stiff ordinary differential equations. I am also interested in inverse problems, uncertainty quantification, numerical optimization, and the theoretical foundations of deep learning.

---

### PhD Research

- **Topological derivative approach for deep neural network architecture adaptation**: The central contribution is to define a network topological derivative for neural networks, borrowing ideas from topology optimization in mechanics. We ask and answer key questions such as: in what sense does adding a new layer constitute a perturbation of the neural network graph. We derived criteria for where to insert the layer and how to initialize it, all in a mathematically principled way. [Link](https://arxiv.org/abs/2502.06885) *(Accepted, [SIAM Journal on Scientific Computing](https://www.siam.org/publications/siam-journals/siam-journal-on-scientific-computing/))*

- **LiLaN: A linear latent network approach for real-time solutions of stiff nonlinear ordinary differential equations**: Solving stiff ODEs requires sophisticated numerical solvers that are often computationally expensive. State-of-the-art machine learning methods such as [Neural ODE](https://arxiv.org/abs/1806.07366) poorly handle timescale separation and require expensive implicit solvers at inference time. LiLaN takes a different path by learning a latent dynamics in which integration becomes analytic, completely avoiding numerical integration. We prove a universal approximation theorem for LiLaN, establishing that the approach is theoretically grounded and not merely a practical heuristic. [Link](https://arxiv.org/abs/2501.08423) *(Accepted, [Machine Learning for Computational Science and Engineering](https://link.springer.com/journal/44379))*

- **A two-stage strategy for neural architecture adaptation**: This project develops a layerwise training strategy for progressively adapting neural networks along the depth, with a stability-promoting criterion. [Link](https://arxiv.org/abs/2211.06860) *(Published, [Computer Methods in Applied Mechanics and Engineering](https://www.sciencedirect.com/journal/computer-methods-in-applied-mechanics-and-engineering))*

- **On unifying randomized methods for inverse problems**: This work unifies the analysis of various randomized methods for solving linear and nonlinear inverse problems by framing the problem in a stochastic optimization setting. By doing so, we show that many randomized methods are variants of a sample average approximation. [Link](https://iopscience.iop.org/article/10.1088/1361-6420/acd36e/meta) *(Published, [Inverse Problems](https://iopscience.iop.org/journal/0266-5611))*

- **A new look at the Ensemble Kalman filter for inverse problems**: This work examines the Ensemble Kalman filter from a new viewpoint via Lagrangian duality. We provide new results on non-asymptotic convergence of the EnKF and new schemes for convergence acceleration of the Ensemble Kalman Inversion algorithm for inverse problems. *(Under review, [Inverse Problems](https://iopscience.iop.org/journal/0266-5611))*

- **Multi-patch epidemic models with partial mobility, residency, and demography**: A multi-patch SEIRS epidemic model that accounts for the effects of human mobility on the evolution of disease dynamics in a multi-population environment. [Link](https://www.sciencedirect.com/science/article/abs/pii/S096007792300591X) *(Published, [Chaos, Solitons & Fractals](https://www.sciencedirect.com/journal/chaos-solitons-and-fractals))*

- **Transformer-powered surrogate for solving inverse problems**: A joint work with [Lawrence Livermore National Laboratory](https://www.llnl.gov/), USA. A transformer-based generative model that transports samples from a prior distribution to the posterior parameter distribution conditioned on an input measurement, while simultaneously reconstructing missing details via inpainting. [Details](/assets/pdf/summery_internship.pdf)

---

### Earlier Research

The following projects were undertaken during my M.Tech at [IIT Madras](https://www.iitm.ac.in) and B.Tech at [NIT Calicut](https://nitc.ac.in) (2013–2020), forming the mechanics and computational background behind my PhD work.

- **Indirect health monitoring of bridges**: Damage identification for bridges based on the dynamic response of a passing vehicle. We integrate Tikhonov regularization with a signal averaging technique and derive mathematical conditions under which bridge damage magnitude and location can be extracted from vehicle response data alone. [Link](https://onlinelibrary.wiley.com/doi/abs/10.1002/stc.2686)

- **Sensitivity-based damage identification using vibration data**: Structural intrinsic properties such as natural frequencies are used to compute the location and magnitude of structural damage via an inverse eigenvalue problem. [Link](https://link.springer.com/article/10.1007/s13349-018-0317-0)

- **Iterative decoupled technique for vehicle-pavement systems**: Decouples the vehicle-pavement system into two subsystems solved independently via an iterative scheme until convergence, with analysis of convergence rate. [Link](https://www.sciencedirect.com/science/article/abs/pii/S0141029618334825)

- **Nonlinear vehicle-pavement coupled dynamics**: A nonlinear vehicle-pavement interaction model using the Galerkin and Runge-Kutta methods, examining the effect of coupling on pavement and vehicle displacements. [Link](https://www.tandfonline.com/doi/abs/10.1080/10298436.2018.1562189)

---

    
## Project Repositories

- **[Sensitivity-based damage identification algorithm](https://github.com/cgkrishnanunni/Sensitivity-based-Damage-Detection)**

   MATLAB implementation of a fast optimization strategy for solving an Inverse Eigen Value Problem in structural mechanics.
  
- **[Numerical Simulation of vehicle-pavement coupled dynamical system](https://github.com/cgkrishnanunni/Decoupled-technique-for-Viscoelastic-Euler-Bernoulli-Beam-pavement-model)**

   MATLAB implementation of a novel iterative technique for simulating the dynamics of a vehicle-pavement coupled system. This repository contains simulation of a novel mathematical model that we developed in the context of vehicle-pavement coupled systems.

- **[Indirect health monitoring of bridges using Tikhonov regularization scheme and signal averaging technique](https://github.com/cgkrishnanunni/INDIRECT-HEALTH-MONITORING-OF-BRIDGES-USING-TIKHONOV-REGULARIZATION-SCHEME-AND-SIGNAL-AVERAGING-TECH)**

   MATLAB implementation of a damage identification algorithm for bridges based on the dynamic response of a passing vehicle.

- **[Sample finite element codes for elasticity](https://github.com/cgkrishnanunni/SAMPLE-FINITE-ELEMENT-CODES-FOR-PLANE-FRAME-TRUSS-QUAD-ELEMENTS)**

   C++ implementations of basic elements (Quadrilateral element, Plane frame, Plane truss etc) developed as a part of the 'Computational Elasticity' Course by Prof. Mohammed Ameen, NIT Calicut.

- **[LiLaN: A Linear Latent Network as the Solution Operator for Real-Time Solutions to Stiff Nonlinear Ordinary Differential Equations](https://github.com/colenockolds/LiLaN-Robertson-ODE)**

   Jax implementation of the [Lilan](https://arxiv.org/abs/2501.08423) approach. 

- **A Machine Learning approach for black-box optimization (Will be updated soon)**

   Pytorch implementation of an approach for black-box optimization-an alternative to Bayesian optimization. Classical Bayesian optimization uses Gaussian processes to model the objective and selects new evaluation points by maximizing an acquisition function. This project asks whether the [Topological derivative approach](https://arxiv.org/abs/2502.06885) developed in my PhD thesis can be used to grow and train a neural network surrogate (instead of Gaussian process regression), while simultaneously acquiring new data samples via a statistical active learning criterion. Therefore, in this project we combine neural network architecture adaptation with adaptive data sampling in a unified framework for black-box optimization.




## Interesting reads!

- **[A Universal Law of Robustness via Isoperimetry](https://arxiv.org/abs/2105.12806)**

This paper provides mathematical insights into why overparametrized models are necessary to interpolate the data smoothly. In particular, the authors have used the term robustness (as measured by the Lipschitz constant of the function) to characterize smoothness in interpolation and show that overparametrization is necessary for reducing the lower bound of the Lipschitz constant. I found this paper particularly interesting since in my research, we use "robustness" as a desirable property for deep neural networks and use this as a criteria to devise a strategy for progressively adapting neural network to a given data-set.  Our  [algorithm](https://arxiv.org/abs/2211.06860) looks at a feasible way to control the upper bound of the Lipschitz constant which is then sufficient for robustness. 

- **[On the Measure of Intelligence](https://arxiv.org/pdf/1911.01547)**

This work by François Chollet (creator of the Keras deep-learning library) attempts to provide a formal definition of intelligence as an agent's ability to adapt to a constantly changing environment and respond appropriately in novel situations. Contemporary Artificial intelligence (AI) community still gravitates towards benchmarking intelligence by comparing the skill exhibited by AIs and humans at specific tasks, such as board games and video games. Chollet argues that solely measuring skill at any given task falls short of measuring intelligence, because skill is heavily modulated by prior knowledge and experience: unlimited priors or unlimited training data allow experimenters to buy arbitrary levels of skills for a system, in a way that masks the system’s own generalization power. The work articulates a new formal definition of intelligence based
on Algorithmic Information Theory and proposes a set of guidelines for what a general AI benchmark should look like!



