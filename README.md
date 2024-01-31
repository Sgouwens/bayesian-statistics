# Bayesian Statistics

This repository contains notebooks for experiments in Bayesian statistics using the PyMC framework. This branch of statistics focusses on doing inference using posterior distributions of parameters. That is, given a model
$$X \sim N(\mu, \sigma^2) $$
the assumption that there exists a fixed true value for $\mu$ and $\sigma$ is not made. They are rather seen as random themselves. Bayes theorem states that the density of X conditional on the the density assumed for its parameter, saym $\mu$, is proportional to the density of $\mu|X$, that is,

$$ f_{\mu|X} = \frac{f_{X|\mu}(x)(\mu)f_X(x)}{\int f_\mu(\mu)d\mu}$$

and so a distribution of the parameter $\mu$ is obtained given the data and the so-called prior distribution assumed on $\mu$. The prior is chosen by the statistician and could be based on contextual knowledge. 

This repository contains some exercises on this topic. Until now, a sinoid data is fitted using a sine function and a more flexible spline. And posterior of gaussian mixture data is fitted using a Dirichlet Process.
