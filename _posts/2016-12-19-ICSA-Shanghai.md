---
layout: post
title:  Presentation at ICSA Shanghai 2016
date:   2016-12-19 00:00:00 +0800
categories: Presentation
---

The first international conference that I attended at Dec 2016. This is part of the work during my PhD at the University of Otago.


### Title: Trajectory estimation from GPS data using an adaptive smoothing spline

Abstract: GPS units record time series data of a moving object. Connecting location points consequently, will represent the trajectory of an individual or a vehicle. However, sparse points and data errors will give a trajectory with angels, which are unlike for a moving object. Smoothing spline methods can efficiently build up a more smooth trajectory. In conventional smoothing spline, the objective function tries to
minimize errors of locations with a penalty term, who has a single parameter that controls the smoothness of reconstruction. Adaptive smoothing spline extends single parameter to a function varying in different domains and adapting the change of roughness. In this talk, I will introduce a tractor spline that incorporates both location and velocity information but penalizes excessive accelerations. The penalty
term is dependent on mechanic boom status. A new parameter, which controls the error of velocity, and adjusted penalty terms, which adapts to a more complicated curvature status, are introduced to the new objective function. We develop cross validation techniques to find the three smoothing parameters of interest. Moreover, researchers found that a conventional smoothing spline can be constructed by Gaussian Process Regression, if it is equipped with an appropriate inner product in a Reproducing Kernel Hilbert Space. Similarly, we give an inner product to the "tractor spline" in a space and make it a RKHS, the function in which has piecewise continuous second derivatives. Then a posterior mean of the estimates can be found by GPR. At the end, simulation studies and a real data example are presented to demonstrate the effectiveness of "tractor spline".

<a href="//JeromeCY.github.io/PDF/2016-ICSA.pdf" target="_blank">Presentation files</a>
