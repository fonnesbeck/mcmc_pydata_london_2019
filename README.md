# Markov chain Monte Carlo with PyMC3
### Chris Fonnesbeck
### PyData London 2019 Tutorial

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/fonnesbeck/mcmc_pydata_london_2019/master)

Bayesian methods are powerful tools for data science applications, complimenting traditional statistical and machine learning methods. Importantly, Bayesian models generate predictions and inferences that fully account for uncertainty. The main tool for conducting Bayesian analysis is Markov chain Monte Carlo (MCMC), a computationally-intensive numerical approach that allows a wide variety of models to be estimated. MCMC algorithms are available in several Python libraries, including PyMC3. I will teach users a practical, effective workflow for applying Bayesian statistics using MCMC via PyMC3 using real-world examples.

This tutorial is intended for analysts, data scientists and machine learning practitioners. Anyone looking for effective ways of making predictions and obtaining inference from datasets should find it useful. The material will assume an intermediate level of Python familiarity. Ideally, attendees should be familiar with Numpy and Jupyter. There is no expectation of students having a statistical background. Having completed the tutorial, students should be able to build basic Bayesian statistical models using their own data, validate those models, and interpret their output.

## Outline

1. Introduction to Bayes and PyMC3
    - What is a Baysian statistical model?
    - The Bayesian workflow in three steps
    - A high-level introduction to the PyMC3 API
    - Motivating examples
2. Markov chain Monte Carlo
    - Why is Bayesian analysis hard?
    - If you can't calculate, simulate!
    - The Metropolis algorithm
    - A better way: Hamiltonian Monte Carlo
3. Building and Fitting Models with PyMC3
    - Stochastic variables
    - Custom distributions
    - Deterministic variables
    - Factor potentials
    - MCMC sampling with step methods
4. Model Checking and Diagnostics
    - Convergence diagnostics
    - Autocorrelation
    - Diagnostics for gradient-based samplers
    - Posterior predictive checks

## Setup

This tutorial assumes that you have [Anaconda](https://www.anaconda.com/distribution/#download-section) (Python 3.7 version) setup and installed on your system.

The next step is to clone or download the tutorial materials in this repository. If you are familiar with Git, run the clone command:

    git clone https://github.com/fonnesbeck/mcmc_pydata_london_2019.git
    
otherwise you can [download a zip file](https://github.com/fonnesbeck/mcmc_pydata_london_2019/archive/master.zip) of its contents, and unzip it on your computer.

The repository for this tutorial contains a file called `environment.yml` that includes a list of all the packages used for the tutorial. If you run:

    conda env create
    
from the main tutorial directory, it will create the environment for you and install all of the packages listed. This environment can be enabled using:

    conda activate mcmc_tutorial
    
Then, I recommend using JupyterLab to access the materials:

    jupyter lab
