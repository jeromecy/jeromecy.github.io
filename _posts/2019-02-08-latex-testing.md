---
layout: post
title: Latex testing
author: Zhanglong
published: true
status: publish
tags: Latex
draft: false
---

Copy and paste from https://petolau.github.io/about/.

What do these three words (or letters) in the name of this method mean and where does it come from? I am sure that you know something about **Linear Model** (maybe because you had read my [previous post about MLR](https://petolau.github.io/Forecast-double-seasonal-time-series-with-multiple-linear-regression-in-R/) :relaxed:). It is a simple regression method which models the response (dependent) variable by independent variable(s). It's solved by the OLS method. So now we know, what the **M** in the name means. When we want to linearly model a response variable which is not from [normal Gaussian distribution](https://en.wikipedia.org/wiki/Normal_distribution), for example, it can be binary (logistic regression) or discrete (Poisson) variable, we can use a generalization of the linear model - [Generalized Linear Model](https://en.wikipedia.org/wiki/Generalized_linear_model) (GLM). It's solved by the [iteratively reweighted least squares](https://en.wikipedia.org/wiki/Iteratively_reweighted_least_squares) (IRLS) method. The **G** in the name is also clear. The **A** letter [Additive Model](https://en.wikipedia.org/wiki/Additive_model), means that the response variable depends linearly on unknown smooth functions. In the other words, the goal is to model the response variable by independent variables, which are in the form of some smooth functions. Voilà, **GAM** is created.

The GAM can be formally written as:

$$g(E(y_i)) = \beta_0 + f_1(x_{i1}) + \dots + f_p(x_{ip}) + \varepsilon_i,$$

$$y_i \sim \mbox{some exponential family distribution,}$$

where \\( i = 1, \dots, N \\), \\( g \\) is a link function (identical, logarithmic or inverse), \\( y \\) is a response variable, \\( x_1, \dots, x_p \\) are independent variables, \\( \beta_0 \\) is an intercept, \\( f_1, \dots, f_p \\) are unknown smooth functions and \\( \varepsilon \\) is an i.i.d. random error.

The smooth function \\( f \\) is composed by sum of basis functions \\( b \\) and their corresponding regression coefficients \\( \beta \\), formally written:

$$f(x) = \sum_{i = 1}^q b_i(x)\beta_i,$$

$$\mbox{ where } q \mbox{ is basis dimension.}$$

Smooth functions are also called [splines](https://en.wikipedia.org/wiki/Spline_(mathematics)). [Smoothing splines](https://en.wikipedia.org/wiki/Smoothing_spline) are real functions that are piecewise-defined by polynomial functions (basis functions). The places, where the polynomial pieces connect are called knots. In **GAMs**, penalized regression splines are used in order to regularize the smoothness of a spline.
