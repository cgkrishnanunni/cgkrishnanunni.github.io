---
layout: page
permalink: /repositories/
title: projects
description: This page provides a glimpse of my research.
nav: true
nav_order: 3
---

# Here are some recent papers I have been reading!

- **[A Universal Law of Robustness via Isoperimetry](https://arxiv.org/abs/2105.12806)**

This paper provides mathematical insights into why overparametrized models are necessary to interpolate the data smoothly. In particular, the authors have used the term robustness (as measured by the Lipschitz constant of the function) to characterize smoothness in interpolation and show that overparametrization is necessary for reducing the lower bound of the Lipschitz constant. I found this paper particularly interesting since in my research, we use "robustness" as a desirable property for deep neural networks and use this as a criteria to devise a strategy for progressively adapting neural network to a given data-set.  Our  [algorithm](https://arxiv.org/abs/2211.06860) looks at a feasible way to control the upper bound of the Lipschitz constant which is then sufficient for robustness. 

- **[Side Effects of Learning from Low-dimensional Data Embedded in a Eucledian Space](https://arxiv.org/pdf/2203.00614.pdf)**

I came across this work by Juncai He, Richard Tsai and Rachel Ward while working on some ideas related to manifold regularization. The paper is an attempt to explain the behaviour of a network on data points that lies on a manifold which is close to but not identical to the original manifold 'M' on which the training data lies. This is practically relevant since there could be a shift in the distribution of the data that occurs post training. The paper makes interesting connection on how the training time (time for gradient descent) is related to data set’s variance in the orthogonal complement of M. The paper also talks about how the consistency in performance of the network improves as the number of data points increases according to some inverse power of the variance of noise.





