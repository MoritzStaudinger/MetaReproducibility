# Meta-Analysis of Reproducible IR Research

## Summary

This is a quantitative analysis on the reproducibility of IR research. For this the problems of 21 reproduction reports from master students (https://zenodo.org/communities/tuw-exdds-ws20/) have been analyzed and aggregated. Each report tries to reproduce the results of a paper published at ECIR, SIGIR or CIKM in the years 2015-2020 and were done by groups of 3 students.

## Setup

All statistics and analysis have been executed under python 3.8.2, all necessary requirements are listed in the requirements.txt file.

## Dataset Description

The dataset (data.csv) consists of 21 papers, which are analyzed on the problems the students encountered. 1 means that the problem has been encountered and 0 means that this problem has not been encountered. Then the sum of all problems is given, as well as the PRIMAD functions used in the reproduction of the papers. If other factors than Actor, according to PRIMAD, have been tuned, the assumptions are stated in an extra column. Each column is separated with a semicolon. 

The columns are the following:

* Name ... String
* Year ... Integer (2015-2020)
* Conference ... String (ECIR/SIGIR,CIKM)
* Code not provided ... Boolean (0/1)
* Code partially not provided ... Boolean (0/1)
* Faulty Code provided ... Boolean (0/1)
* Information about Software Versions missing ... Boolean (0/1)
* Data not provided ... Boolean (0/1)
* Data is partially not provided ... Boolean (0/1)
* Metadata not provided ... Boolean (0/1)
* Comparison Metrics or Baselines not used ... Boolean (0/1)
* Experimental Setup not described ... Boolean (0/1)
* Experiment Workflow incomplete ... Boolean (0/1)
* Inconsistencies in Paper, Code and Data ... Boolean (0/1)
* Results differ significantly ... Boolean (0/1)
* Cultural Context differs ... Boolean (0/1)
* Specific Hardware and Software Setup necessary ... Boolean (0/1)
* Sum ... Integer (Sum of all Boolean Columns before)
* Platform ... Boolean (0/1)
* Research Objective ... Boolean (0/1)
* Implementation ... Boolean (0/1)
* Method ... Boolean (0/1)
* Actor ... Boolean (0/1)
* Data ... Boolean (0/1)
* Assumptions ... String