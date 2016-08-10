# ecoli_me_testing
Reduced draft ME model of *E. coli*.
- solved using solveME software. [Citation TBA]()
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
Off-the-shelf solvers do not work well due to the multiscale nature of M & E fluxes.
Therefore, a quad-precision-based solver suite has been developed [Link TBD]().
