---
layout: default
title: Michael C. Grundler
style: main
---

## Macroevolution of discrete traits with rate heterogeneity

The ability to accommodate among-lineage phenotypic rate variation
adds an important element of realism to stochastic models of trait evolution. In this
work I modified the [BAMM](http://bamm-project.org) code-base to work with a
binary state character.
Interestingly, this model for among-lineage rate variation fails when transition
rates are not constrained to be identical. The intuition for this failure is that
each rate-shift event can allow one rate to become arbitrarily large and the
other to become arbitrarily small, thereby guaranteeing the origin and persistence of a derived
character state. The rate-shift mechanism itself introduces another way to observe
an event of character state change!
Read more [here](https://blueraleigh.github.io/research). I have since explored
alternatives methods for accommodating among-lineage rate variation used in
phylogenetic inference that are also amenable to phenotypic evolution, and I
provide C implementations of the random-local clock model and the covarion model
in my macroevolution R package available [here](https://github.com/blueraleigh/macroevolution).

## Parsimony and likelihood

Transition rates in continuous-time Markov chain (CTMC) models of character
evolution are usually estimated by marginalizing over all histories of character
evolution that could possibly explain the data. An advantage of this approach is
that the resulting parameter estimates are not conditional on any particular
(uncertain) history of change. A disadvantage of this approach is that the resulting estimates
are not necessarily close to the truth. After all, history only happened once
and the average of all outcomes could be quite far from the single historical
outcome that actually occurred. In this work I explored a different approach to
estimating transition rates of CTMC models by conditioning the estimates on
most-parsimonious histories of character state change. These alternative
estimators have lower mean squared errors than the marginal likelihood estimators
used in common practice. Due to the rapidity with which they can be computed,
the parsimony-informed estimators can also be used to quickly explore datasets
for phylogenetic variation in tempo and mode. Read more [here](https://blueraleigh.github.io/research).


## The role of stasis in determining transition rate asymmetry

A lot of macroevolution studies today rely in some way on estimating and
interpreting the parameters of a stochastic process model. Unfortunately, it is
not always straightforward to know what features of the data inform these
parameter estimates, and this seems to be an important but under-studied area. I became
interested in this question while thinking about transition rates in continuous-time
Markov chain (CTMC) models of character evolution.
Transition rates estimated for these models are commonly interpreted as providing
a historical description of the pattern of change from ancestor to descendant.
In other words, if we estimate a higher transition rate from state A to state B
than the reverse this must be because more change from an ancestral state of A
to a derived state of B is needed to explain the data.
My work in this area suggests otherwise. Instead, especially in large phylogenies,
significant asymmetries in transition rates are most likely driven by asymmetries
in character state stasis rather than asymmetries in character state change.
In other words, even if nearly all change is from A to B the transition rate
from B to A can be much higher than the reverse rate if most of the tree is in
state B. Read more [here](https://blueraleigh.github.io/research).

## Macroevolutionary models for complex ecological traits

The complexity of how organisms interact with their environments means that for
the purpose of comparative analysis many characteristics of organismal ecology,
like what an animal eats, are summarized using ordinal or nominal variables, which
are then treated as evolutionary states in a CTMC. An advantage of this approach
is that it collapses a high degree of complexity into a more manageable set of
important features. A disadvantage is that a lot of useful data are discarded in
the process. My interest in snake diet evolution led me to explore an alternative
approach that uses a multinomial model to automatically classify taxa
into ecological states (based on empirical count data) and a CTMC model as an
evolutionary prior on the history of state-to-state transformations between
ancestor and descendant.
You can checkout the preprint [here](https://www.biorxiv.org/content/10.1101/640334v2).
The model itself is implemented in the macroevolution R package [here](https://github.com/blueraleigh/macroevolution).

## Snake diet evolution

Compared to other squamate reptiles (i.e., lizards), snakes have highly specialized
feeding habits. Among the world’s snakes there is nonetheless wide variation in
both the kinds of food and the number of food types recorded in dietary samples.
I maintain a global database of snake feeding observations (currently more than 30,000 observations
from over 1200 snake species!) to address macroevolutionary patterns
in the evolution of snake diets. The majority of observations originate from
previously published observations, but I also use museum specimens to generate
new primary observations (e.g., [see here](https://quod.lib.umich.edu/r/rept3ic)).
To checkout the database for use in your own research go [here](https://github.com/blueraleigh/squamatabase)
and download the R package I made for it. There is also a [preprint](https://blueraleigh.github.io/research)
describing the project and some of the motivation. Stay tuned for papers describing some cool
empirical results!
