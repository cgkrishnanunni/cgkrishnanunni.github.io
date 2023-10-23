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

  - Sensitivity-Based Damage Identification Algorithm using Vibration Data (An Inverse Eigen Value Problem): This project explores the use of structural intrinsic properties such as natural frequencies for computing the location and magnitude of structural damage (stiffness reduction). [Link](https://link.springer.com/article/10.1007/s13349-018-0317-0)
    
  -  Indirect Health Monitoring of Bridges: This project deals with damage identification strategies for bridges based on the dynamic response of a passing vehicle.  We have sucessfully integrated Tikhonov Regularization scheme with a signal averaging technique to define a cost function and showed that under some derived mathematical conditions, it is possible to extract the magnitude and location of bridge damage based on dynamic vehicle response data.  [Link](https://onlinelibrary.wiley.com/doi/abs/10.1002/stc.2686)
    
  -  On Unifying Randomized Methods For Inverse Problems: This work unifies the analysis of various randomized methods for solving linear and nonlinear inverse problems by framing the problem in a stochastic optimization setting. By doing so, we show that many randomized methods are variants of a sample average approximation.  [Link](https://iopscience.iop.org/article/10.1088/1361-6420/acd36e/meta)

- Projects undertaken in **mathematical modelling**.

  - A novel mathematical model for simulating the nonlinear vehicle–pavement coupled dynamics: In this project, a non-linear vehicle-pavement interaction model has been proposed. The Galerkin method and Runge–Kutta method are employed to discretise the differential equations arising from the dynamic equations of motion of the system. The effect of coupling action on pavement displacements and vehicle body vertical displacement is examined numerically with the developed model.  [Link](https://www.tandfonline.com/doi/abs/10.1080/10298436.2018.1562189)

  - Multi-patch epidemic models with partial mobility, residency, and demography:  In this work, a multi-patch epidemic model is proposed that take into account the effects of human mobility on the evolution of disease dynamics in a multi-population environment. In particular, the work develops  SEIRS multi-patch and multi-group epidemic models to practically account for distinct epidemiological-status-dependent mobilities in each patch.  [Link](https://www.sciencedirect.com/science/article/abs/pii/S096007792300591X)
  
- Projects undertaken in **numerical analysis**.
  - Iterative decoupled technique for dynamic response of vehicle-pavement systems: This project focus on developing an iterative decoupled technique for the simulating the dynamic response of vehicle-pavement systems. The key idea of the approach involves decoupling the vehicle-pavement coupled system into two subsystems and solving them independently until the solution has converged using an iterative scheme. We look at various aspects of the method such as rate of convergence etc. [Link](https://www.sciencedirect.com/science/article/abs/pii/S0141029618334825)
    
  - A new look at the convergence of Ensemble Kalman inversion algorithm from a functunal analysis perspective: This is an ongoing research that looks at the Ensemble Kalman filter from a new viewpoint. We provide some new results on non-asymptotic convergence of EnKF. We also provide new proofs on the convergence of Ensemble Kalman Inversion algorithm which is a variant of the EnKF algorithm for inverse problems. 


- Projects undertaken in **machine learning**.
  
  - A two stage strategy for neural architecture adaptation: While deep neural networks (DNN) create increasinglysimpler but more useful  representations  of the learning problem layer by layer, such large networks however yieldcomputationally complex optimization problems. Furthermore, despite such successes, the mechanisms behind deep learning remain a mystery and a trial-and-error approach (Architecture search) is often employed to retrieve the best neural network.  This project focus on the development of a layerwise training strategy for progressively adapting neural networks along the depth. [Link](https://arxiv.org/abs/2211.06860)

  - An architecture design strategy inspired from topology optimization: This is an ongoing project that derives an architecture adaptation strategy borrowing ideas from topology optimization.
    
  - A deep learning framework  for inverse problems: This is an ongoing project that derives a purely data-driven, model-free and, prior-free framework for inverse problems. The framework is inspired from diffusion models and the Ensemble Kalman Inversion framework.
    
  - Learning low dimensional latent manifolds for dimension reduction using reinforcement learning: This is an ongoing project that looks at the use of a reinforcement learning strategy for manifold learning.
    


## Recent readings!

- **[A Universal Law of Robustness via Isoperimetry](https://arxiv.org/abs/2105.12806)**

This paper provides mathematical insights into why overparametrized models are necessary to interpolate the data smoothly. In particular, the authors have used the term robustness (as measured by the Lipschitz constant of the function) to characterize smoothness in interpolation and show that overparametrization is necessary for reducing the lower bound of the Lipschitz constant. I found this paper particularly interesting since in my research, we use "robustness" as a desirable property for deep neural networks and use this as a criteria to devise a strategy for progressively adapting neural network to a given data-set.  Our  [algorithm](https://arxiv.org/abs/2211.06860) looks at a feasible way to control the upper bound of the Lipschitz constant which is then sufficient for robustness. 

- **[Side Effects of Learning from Low-dimensional Data Embedded in a Eucledian Space](https://arxiv.org/pdf/2203.00614.pdf)**

I came across this work by Juncai He, Richard Tsai and Rachel Ward while working on some ideas related to manifold regularization. The paper is an attempt to explain the behaviour of a network on data points that lies on a manifold which is close to but not identical to the original manifold 'M' on which the training data lies. This is practically relevant since there could be a shift in the distribution of the data that occurs post training. The paper makes interesting connection on how the training time (time for gradient descent) is related to data set’s variance in the orthogonal complement of M. The paper also talks about how the consistency in performance of the network improves as the number of data points increases according to some inverse power of the variance of noise.





