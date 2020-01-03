---
layout: default
title: Michael C. Grundler
style: main
---
{% include lib/mathjax.html %}

## The role of stasis in determining transition rate asymmetry

Abstract
--------
Transition rates estimated for macroevolutionary models of discrete character evolution are commonly interpreted as providing a historical
description of the pattern of change from ancestor to descendant. In other words, if we estimate a higher transition rate from state A to
state B than the reverse this must be because more change from an ancestral state of A to a derived state of B is needed to explain the data.
However, because the likelihood calculations in these models are also affected by patterns of apparent stasis, it is unclear when asymmetries
in transition rates match the pattern of asymmetry in the historical sequence of state changes that actually occurred. To gain insight into
this problem I study the expected behavior of a simple two-state model of discrete character evolution. To a first order approximation, I
find that the ratio of transition rates equals the ratio of the number of character state changes (i.e., when the pattern of asymmetry in
rates matches the pattern of asymmetry in character change) only when the amount of time spent in stasis in each state is equal. When the
amount of time in stasis in each state is unequal, the ratio of transition rates is biased in the direction of the state displaying the most
stasis, sometimes to the point where it can overwhelm the pattern change. In other words, even if nearly all change is from A to B the
transition rate from B to A can be much higher than the reverse rate if most of the tree is in state B. Researchers who use asymmetric models
of discrete character evolution should be aware of this property and exercise caution when attempting to interpret asymmetries in transition
rates as reflective of a historical pattern of asymmetry in character state change. Especially in large phylogenies, significant asymmetries
in transition rates are most likely driven by asymmetries in character state stasis rather than asymmetries in character state change.

Results
-------
For a two-state continuous-time Markov chain of discrete character evolution the
lineage transition probabilities are,

$$
p_{01}(t) = \frac{\epsilon}{1 + \epsilon} - \frac{\epsilon}{1 + \epsilon}e^{-\tau t}
$$

$$
p_{00}(t) = \frac{1}{1 + \epsilon} + \frac{\epsilon}{1 + \epsilon}e^{-\tau t}
$$

$$
p_{10}(t) = \frac{1}{1 + \epsilon} - \frac{1}{1 + \epsilon}e^{-\tau t}
$$

$$
p_{11}(t) = \frac{\epsilon}{1 + \epsilon} - \frac{1}{1 + \epsilon}e^{-\tau t}
$$

where $$ \tau = q_{01} + q_{10}$$, $$ \epsilon = \frac{q_{01}}{q_{10}} $$, and
$$ q_{01} $$ and $$ q_{10} $$ are the forward and reverse transition rates.

My focus for this study concerns the behavior of the maximum likelihood estimator
for the parameter $$ \epsilon $$. I use the symbol $$ L_{\hat{X}} $$  to represent
the likelihood of \hat{X}, which represents an assignment of character states to
all nodes in a phylogeny that is consistent with the observed state assignments at
the terminal nodes. In standard practice, the likelihood $$ L $$ of the observed
state assignments is computed by summing over all possible $$ \hat{X} $$  so that
$$ L = \sum_{\hat{X}}{L_{\hat{X}}} $$. Because $$ L_{\hat{X}} $$  is just a product
of independent lineage transition probabilities we have,
