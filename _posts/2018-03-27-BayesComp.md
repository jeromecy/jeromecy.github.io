---
layout: post
title:  Poster at Bayes Comp 2018, Barcelona
date:   2018-03-27 00:00:00 +0800
categories: Presentation
---


This is the poster of the work done with my supervisor Dr. Matthew Parry. The poster was given at the conference
Bayes Comp 2018, Barcelona.

Bayes Comp is a biennial conference sponsored by the ISBA section of the same name. The conference and the section both aim to promote original research into computational methods for inference and decision making and to encourage the use of frontier computational tools among practitioners, the development of adapted software, languages, platforms, and dedicated machines, and to translate and disseminate methods developed in other disciplines among statisticians. The detail is at <a href="https://www.maths.nottingham.ac.uk/plp/pmztk/bayescomp/" target="_blank">conference information</a>.


### Title: Adaptive Sequential MCMC for Combined State and Parameters Estimation

Abstract: Most algorithms for combined state and parameter estimation in state space models either estimate the states and parameters by incorporating the param-eters in the state space, or marginalize out the parameters through suﬃcient statistics. In the case of a linear state space model and starting with a joint distribution over states, observations and parameters, we implement an MCMC sampler with two phases. In the learning phase, a self-tuning sampler is used to learn the parameter mean and covariance structure. In the estimation phase, the parameter mean and covariance structure informs the proposal mechanism and is also used in a delayed-acceptance algorithm, which greatly improves sam-pling eﬃciency. Information on the resulting state of the system is given by a Gaussian mixture. In on-line mode, the algorithm is adaptive and uses a sliding window approach by cutting oﬀ historical data to accelerate sampling speed and to maintain appropriate acceptance rates. We apply the algorithm to joint state and parameter estimation in the case of irregularly sampled GPS time series data.

<a href="//JeromeCY.github.io/PDF/2018-BayesCompPoster.pdf" target="_blank">Presentation files</a>
