---
layout: page
permalink: /repositories/
title: research
description: This page provides a glimpse of my research projects.
nav: true
nav_order: 3
---


## Research projects undertaken

It has always fascinated me to see what mathematics can do especially in bringing together different disciplines to solve complex problems in real life. To that end, my research is interdisciplinary and the projects fall under four broad categories. 

- Projects undertaken in **inverse problems**.

  - Sensitivity-Based Damage Identification Algorithm using Vibration Data (An Inverse Eigen Value Problem): This project explores the use of structural intrinsic properties such as natural frequencies for computing the location and magnitude of structural damage (stiffness reduction). We derive a sensitivity equation by linearizing the perturbed linear dynamics to study the sensitivity of natural frequencies and static displacements to a stiffness reduction. An objective function representing a residual is then defined using the derived sensitivity equation and minimized using a metaheuristic optimization algorithm for determining structural damage.
  -  Indirect Health Monitoring of Bridges: Indirect health monitoring deals with damage identification strategies for bridges based on the dynamic response of a moving vehicle: In this project we have sucessfully integrated Tikhonov Regularization scheme with a signal averaging technique to define a cost function and showed that under some derived mathematical conditions, it is possible to extract the magnitude and location of bridge damage based on dynamic vehicle response data. In a related project, we have used Thermodynamic principles to relate the change in Vehicle–Bridge-Interaction (VBI) forces to the change in dynamic tyre pressure.  A Stein variational gradient descent implementation of the Bayes rule is employed to quantify the uncertainty in the estimated tyre parameters which is then used for bridge damage identification.
  -  On Unifying Randomized Methods For Inverse Problems: This work unifies the analysis of various randomized methods for solving linear and nonlinear inverse problems by framing the problem in a stochastic optimization setting. By doing so, we show that many randomized methods are variants of a sample average approximation. 

- Projects undertaken in **mathematical modelling**.

  - A novel mathematical model for simulating the nonlinear vehicle–pavement coupled dynamics: In this project, a non-linear vehicle-pavement interaction model has been proposed. The Galerkin method and Runge–Kutta method are employed to discretise the differential equations arising from the dynamic equations of motion of the system. The effect of coupling action on pavement displacements and vehicle body vertical displacement is examined numerically with the developed model.

  - Multi-patch epidemic models with partial mobility, residency, and demography:  In this work, a multi-patch epidemic model is proposed that take into account the effects of human mobility on the evolution of disease dynamics in a multi-population environment. In particular, the work develops  SEIRS multi-patch and multi-group epidemic models to practically account for distinct epidemiological-status-dependent mobilities in each patch.
  
- Projects undertaken in **numerical analysis**.


- Projects undertaken in **machine learning**.


## Recent readings!

- **[A Universal Law of Robustness via Isoperimetry](https://arxiv.org/abs/2105.12806)**

This paper provides mathematical insights into why overparametrized models are necessary to interpolate the data smoothly. In particular, the authors have used the term robustness (as measured by the Lipschitz constant of the function) to characterize smoothness in interpolation and show that overparametrization is necessary for reducing the lower bound of the Lipschitz constant. I found this paper particularly interesting since in my research, we use "robustness" as a desirable property for deep neural networks and use this as a criteria to devise a strategy for progressively adapting neural network to a given data-set.  Our  [algorithm](https://arxiv.org/abs/2211.06860) looks at a feasible way to control the upper bound of the Lipschitz constant which is then sufficient for robustness. 

- **[Side Effects of Learning from Low-dimensional Data Embedded in a Eucledian Space](https://arxiv.org/pdf/2203.00614.pdf)**

I came across this work by Juncai He, Richard Tsai and Rachel Ward while working on some ideas related to manifold regularization. The paper is an attempt to explain the behaviour of a network on data points that lies on a manifold which is close to but not identical to the original manifold 'M' on which the training data lies. This is practically relevant since there could be a shift in the distribution of the data that occurs post training. The paper makes interesting connection on how the training time (time for gradient descent) is related to data set’s variance in the orthogonal complement of M. The paper also talks about how the consistency in performance of the network improves as the number of data points increases according to some inverse power of the variance of noise.





