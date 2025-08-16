---
layout: page
permalink: /repositories/
title: Research
description: This page provides an overview of some of my research projects.
nav: true
nav_order: 3
---


## Research projects undertaken

It has always fascinated me to see what mathematics can do especially in bringing together different disciplines to solve complex problems in real life. To that end, my research is interdisciplinary and the projects fall under four broad categories. 

- Projects undertaken in **inverse problems**.

  - Sensitivity-Based Damage Identification Algorithm using Vibration Data (An Inverse Eigen Value Problem): This project explores the use of structural intrinsic properties such as natural frequencies for computing the location and magnitude of structural damage (stiffness reduction). [Link](https://link.springer.com/article/10.1007/s13349-018-0317-0)
    
  -  Indirect Health Monitoring of Bridges: This project deals with damage identification strategies for bridges based on the dynamic response of a passing vehicle.  We have sucessfully integrated Tikhonov Regularization scheme with a signal averaging technique to define a cost function and showed that under some derived mathematical conditions, it is possible to extract the magnitude and location of bridge damage based on dynamic vehicle response data.  [Link](https://onlinelibrary.wiley.com/doi/abs/10.1002/stc.2686)
    
  -  On Unifying Randomized Methods For Inverse Problems: This work unifies the analysis of various randomized methods for solving linear and nonlinear inverse problems by framing the problem in a stochastic optimization setting. By doing so, we show that many randomized methods are variants of a sample average approximation.  [Link](https://iopscience.iop.org/article/10.1088/1361-6420/acd36e/meta)
    
  -  Transformer-powered surrogate for solving inverse problems via joint modeling with forward process: This is a joint work with Lawrence Livermoore National Laboratory, USA. In this work we trained a transformer architecture based generative model that transports samples from a prior distribution to samples from the posterior parameter distribution conditioned on an input measurement. The method also simultaneously reconstructs the missing details in the input measurement field (Inpainting). High level details are provided [HERE](/assets/pdf/summery_internship.pdf)

- Projects undertaken in **mathematical modelling**.

  - A novel mathematical model for simulating the nonlinear vehicle–pavement coupled dynamics: In this project, a non-linear vehicle-pavement interaction model has been proposed. The Galerkin method and Runge–Kutta method are employed to discretise the differential equations arising from the dynamic equations of motion of the system. The effect of coupling action on pavement displacements and vehicle body vertical displacement is examined numerically with the developed model.  [Link](https://www.tandfonline.com/doi/abs/10.1080/10298436.2018.1562189)

  - Multi-patch epidemic models with partial mobility, residency, and demography:  In this work, a multi-patch epidemic model is proposed that take into account the effects of human mobility on the evolution of disease dynamics in a multi-population environment. In particular, the work develops  SEIRS multi-patch and multi-group epidemic models to practically account for distinct epidemiological-status-dependent mobilities in each patch.  [Link](https://www.sciencedirect.com/science/article/abs/pii/S096007792300591X)
  
- Projects undertaken in **numerical analysis**.
  
  - Iterative decoupled technique for dynamic response of vehicle-pavement systems: This project focus on developing an iterative decoupled technique for the simulating the dynamic response of vehicle-pavement systems. The key idea of the approach involves decoupling the vehicle-pavement coupled system into two subsystems and solving them independently until the solution has converged using an iterative scheme. We look at various aspects of the method such as rate of convergence etc. [Link](https://www.sciencedirect.com/science/article/abs/pii/S0141029618334825)
    
  - A new look at the convergence of Ensemble Kalman inversion algorithm from a functunal analysis perspective: This is an ongoing research that looks at the Ensemble Kalman filter from a new viewpoint. We provide some new results on non-asymptotic convergence of EnKF. We also provide new proofs on the convergence of Ensemble Kalman Inversion algorithm which is a variant of the EnKF algorithm for inverse problems. 


- Projects undertaken in **machine learning**.
  
  - A two stage strategy for neural architecture adaptation: While deep neural networks (DNN) create increasingly simpler but more useful  representations  of the learning problem layer by layer, such large networks however yieldcomputationally complex optimization problems. Furthermore, despite such successes, the mechanisms behind deep learning remain a mystery and a trial-and-error approach (Architecture search) is often employed to retrieve the best neural network.  This project focus on the development of a layerwise training strategy for progressively adapting neural networks along the depth. [Link](https://arxiv.org/abs/2211.06860)

  - Topological derivative approach for deep neural network architecture adaptation: We developed a neural network architecture adaptation strategy borrowing ideas from topology optimization in mechanics.  At the heart of our approach are two key ingredients: i) the introduction of a shape functional to be minimized, which depends on neural network topology, and ii) the introduction of a topological derivative of the shape functional with respect to the neural network topology. [Link](https://arxiv.org/abs/2502.06885).
    
  - Lilan: A linear latent network approach for real-time solutions of stiff, nonlinear, ordinary differential equations: Solving stiff ordinary differential equations (StODEs) requires sophisticated numerical solvers, which are often computationally expensive. In particular, StODE's often cannot be solved with traditional explicit time integration schemes and one must resort to costly implicit methods to compute solutions. On the other hand, state-of-the-art machine learning (ML) based methods such as Neural ODE (NODE) poorly handle the timescale separation of various elements of the solutions to StODEs and require expensive implicit solvers for integration at inference time. In this work, we embark on a different path which involves learning a latent dynamics for StODEs, in which one completely avoids numerical integration [Link](https://arxiv.org/abs/2501.08423).

    
## Project Repositories

- **[Sensitivity-Based Damage Identification Algorithm](https://github.com/cgkrishnanunni/Sensitivity-based-Damage-Detection)**

   MATLAB implementation of a fast optimization strategy for solving an Inverse Eigen Value Problem in structural mechanics.
  
- **[Numerical Simulation of Vehicle-Pavement Coupled Dynamical System](https://github.com/cgkrishnanunni/Decoupled-technique-for-Viscoelastic-Euler-Bernoulli-Beam-pavement-model)**

   MATLAB implementation of a novel iterative technique for simulating the dynamics of a vehicle-pavement coupled system. This repo contains simulation of a novel mathematical model that we developed in the context of vehicle-pavement couspled systems.

## Interesting reads!

- **[On the Measure of Intelligence](https://arxiv.org/pdf/1911.01547)**

This work by François Chollet (creator of the Keras deep-learning library) attempts to provide a formal definition of intelligence as an agent's ability to adapt to a constantly changing environment and respond appropriately in novel situations. Contemporary Artificial intelligence (AI) community still gravitates towards benchmarking intelligence by comparing the skill exhibited by AIs and humans at specific tasks, such as board games and video games. Chollet argues that solely measuring skill at any given task falls short of measuring intelligence, because skill is heavily modulated by prior knowledge and experience: unlimited priors or unlimited training data allow experimenters to buy arbitrary levels of skills for a system, in a way that masks the system’s own generalization power. The work articulates a new formal definition of intelligence based
on Algorithmic Information Theory and proposes a set of guidelines for what a general AI benchmark should look like!

- **[A Universal Law of Robustness via Isoperimetry](https://arxiv.org/abs/2105.12806)**

This paper provides mathematical insights into why overparametrized models are necessary to interpolate the data smoothly. In particular, the authors have used the term robustness (as measured by the Lipschitz constant of the function) to characterize smoothness in interpolation and show that overparametrization is necessary for reducing the lower bound of the Lipschitz constant. I found this paper particularly interesting since in my research, we use "robustness" as a desirable property for deep neural networks and use this as a criteria to devise a strategy for progressively adapting neural network to a given data-set.  Our  [algorithm](https://arxiv.org/abs/2211.06860) looks at a feasible way to control the upper bound of the Lipschitz constant which is then sufficient for robustness. 

- **[Side Effects of Learning from Low-dimensional Data Embedded in a Eucledian Space](https://arxiv.org/pdf/2203.00614.pdf)**

I came across this work by Juncai He, Richard Tsai and Rachel Ward while working on some ideas related to manifold regularization. The paper is an attempt to explain the behaviour of a network on data points that lies on a manifold which is close to but not identical to the original manifold 'M' on which the training data lies. This is practically relevant since there could be a shift in the distribution of the data that occurs post training. The paper makes interesting connection on how the training time (time for gradient descent) is related to data set’s variance in the orthogonal complement of M. The paper also talks about how the consistency in performance of the network improves as the number of data points increases according to some inverse power of the variance of noise.





