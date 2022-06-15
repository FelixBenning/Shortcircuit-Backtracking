# Shortcircuit Backtracking

## Abstract

Backtracking e.g. using the Armijo Rule requires knowledge
about the progress made. This is not the case in SGD, where
we do not know whether and how much progress we make. For quadratic Loss
functions it is possible to calculate the learning rate resulting from
backtracking. While backtracking fundamentally works like "wait unitl...'',
calculations can be approximated, so they might be more useful in stochastic
gradient settings.

## Note

At the moment this only works for full gradient, quadratic loss functions and it
only provides a `log` speedup over backtracking in this case.

Still necessary to be interesting
- [ ] generalization beyond quadratic losses
- [ ] generalization to SGD