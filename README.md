# ecoli_me_testing
Reduced draft ME model of *E. coli*.
- Citation for final model: [TBA]()

## Contents
---
### Reduced ME model for rapid prototyping
- ME_NLP_082815.mat

A **reduced** ME model. Mathematical formulation:
max mu,
s.t. S\*v = b,
mu\*A\*v + B\*v = 0,
lb <= v <= ub,

where v is the vector of fluxes in mmol/gDW/h (both metabolic and expression), and mu is the growth rate (1/h).

Standard double-precision solvers do not work well due to the multiscale nature of ME models.
Therefore, a quad-precision-based solver suite (solveME) has been developed in a related effort: [Yang, Ma, et al. (2016) *BMC Bioinf* 17:391](http://doi.org/10.1186/s12859-016-1240-1).
