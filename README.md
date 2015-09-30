PHRAPL --  user manual
=======

##**WARNING**
This user manual is under development. Please send me an [email](ariadna.biologia@gmail.com) if you have comments.
Figures and examples need to be added.

________

<img src="https://github.com/ariadnamorales/phrapl-manual/blob/master/phrapl_logo.png?raw=true" width="200" height="200" />

### CITATION
O'Meara BC, Jackson ND, Morales A, & Carstens BC [(in review)](http://biorxiv.org/content/early/2015/08/24/025353) Phylogeographic Inference using Approximate likelihoods. Evolution.

### CODE
`PHRAPL` is writen in `R`, but it uses `perl` and `ms` to perform simulations. The pre-CRAN (code under development) can be found in [github.](https://github.com/bomeara/phrapl)

## Why to use `PHRAPL`?
Phylogeographic research aims to understand the recent history of species. Over the last decades, researchers have increasingly incorporated demographic models in order to estimate parameters (i.e., divergence times, population sizes, and rates of migration and expansion) that can contribute phylogeographic inference. 
Typically, this is conducted via the use of software packages that contain specified models (n-island models or fixed topologies). Alternatively, simulation-based approaches allow researchers to customize models for the particular details of their system, and may be useful in testing preexisting biogeographic hypotheses. Because the demographic model is central to the analysis in either case, researchers may wish to assess the appropriateness of their model to the data. `PHRAPL` is designed to give such a tool to researchers. 

## How `PHRAPL` works ?
`PHRAPL` simulates genealogies under a wide range of demographic models and compares the empirical genealogies to the simulated gene tree distributions. Demographic models that are probable given the data will contain many genealogies that match the estimated gene trees. Because the proportion of matching gene trees for a given model is equivalent to the probability of the data given the model and parameter values, we can use this value in an information theoretic framework to evaluate the relative weight of all models. This provides the researcher with an independent assessment of both the best model, given the data as well as the ability to calculate the model likelihoods of classes of models (e.g., n-island vs. isolation models).

Watch [these YouTube videos](https://www.youtube.com/watch?v=UC4Mj1K6c0k) to learn more about `PHRAPL`.

## Contents

1. [Installation](https://github.com/ariadnamorales/phrapl-manual/blob/master/1.Installation.Rmd)
2. [Input files](https://github.com/ariadnamorales/phrapl-manual/blob/master/2.Input_files.Rmd)
3. [Generate a set of models (migrationArray object)](https://github.com/ariadnamorales/phrapl-manual/blob/master/3.Generate_set_of_models.Rmd)
  - [3a. How models are built?](https://github.com/ariadnamorales/phrapl-manual/blob/master/3a.How_models_are_built.Rmd)
  - [3b. Ploting models](https://github.com/ariadnamorales/phrapl-manual/blob/master/3b.Ploting_models.Rmd)
4. [Subsampling and creating an input for `PHRAPL`](https://github.com/ariadnamorales/phrapl-manual/blob/master/4.Subsample_CreateInput.Rmd)
5. [Running `PHRAPL` (GridSearch option)](https://github.com/ariadnamorales/phrapl-manual/blob/master/5.Run_Phrapl.Rmd)
  - [5a. Running in parallel]()
6. [Post-processing](https://github.com/ariadnamorales/phrapl-manual/blob/master/6.Post-processing.Rmd)
7. [Output]()
  - [7a. Model selection]()
8. Examples
