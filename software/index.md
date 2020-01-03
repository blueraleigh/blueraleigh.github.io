---
layout: default
title: Michael C. Grundler
style: main
---
## macroevolution

An R package that provides functionality for useful macroevolutionary tools that are missing from commonly used R packages
(e.g., ape) as well as implementations of methods developed for my own research. Most functionality is written in C and called
from R using the ```.Call``` API. [Github](https://github.com/blueraleigh/macroevolution)

## rsqlite

Provides read-only access to a [SQLite](https://sqlite.org) database from within R. Written in C to take advantage of the SQLite API. Note that there is a CRAN package by the same name but it is significantly more complicated and hence offers a great deal more functionality. [Github](https://github.com/blueraleigh/rsqlite)

## dbedit

A form-based web application for entering data into a SQLite database. This was originally developed to help me compile
data on snake diets. Written in TCL. [Github](https://github.com/blueraleigh/dbedit)

## squamatabase

An R package that ships with a large database of diet records for the world's snakes. In addition to the data, it provides
some functions to perform common data filtering and manipulation operations. [Github](https://github.com/blueraleigh/squamatabase)
