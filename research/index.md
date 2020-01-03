---
layout: default
title: Michael C. Grundler
style: main
---
## Macroevolution of discrete traits with rate heterogeneity

## Parsimony and likelihood

## The role of stasis in determining transition rate asymmetry

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
Although there is general consensus that this diversity of modern feeding types
arose from ecologically restricted lizard-like forebears, there have been few
quantitative studies investigating phylogenetic patterns in the trophic ecological
transformations that took place during snake evolution, particularly with regard
to patterns of specialization and generalization and rates of change. I maintain
a global database of snake feeding observations (currently more than 30,000 observations
from over 1200 snake species!) to address macroevolutionary patterns
in the evolution of snake diets. The majority of observations originate from
previously published observations, but I also use museum specimens to generate
new primary observations (e.g., [see here](https://quod.lib.umich.edu/r/rept3ic)).
To checkout the database for use in your own research go [here](https://github.com/blueraleigh/squamatabase)
and download the R package I made for it. There is also a [preprint](https://blueraleigh.github.io/research)
describing the project and some of the motivation.
