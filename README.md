# Bayesian Digit Analysis - O'Bayes 2019, Warwick

This repository accompanies the [Bayesian Digit Analysis](https://github.com/pedro-teles-fonseca/bda-poster-warwick/blob/master/poster.pdf)  poster, presented in the [O'Bayes 2019](https://warwick.ac.uk/fac/sci/statistics/staff/academic-research/robert/0bayesconference/) conference in the University of Warwick (UK). The purpose of this repository is to share the data and the code that was used, allowing the replicability of obtained results. Some supplementary graphs and tables are also provided.  

## Instructions

### Prerequisites

In order to run the R scripts provided in this repository, the following R packages are required:

```r
library("Hmisc")
library("tidyverse") 
```
Nevertheless, it is possible to reproduce all the results in the poster using only the base R package, since the `Hmisc` package is only used to export R tables in TeX format and the `tidyverse` packages are only used to produce plots, which are supplementary material. 

### Data

The raw data can be found in the `raw-data.xls` file, stored in the `data` folder. The reorganized version of the dataset that is imported by the R scripts is the `data.txt` file, stored in the same folder. 

### Reproducibility

Using an Rstudio project, we provide a self-contained workflow that allows for the replicability of all the results in the poster. In order to direct R to the correct working directory, the `bda-poster-warwick.Rproj` file should be run beforehand. After that, all R scripts should run smoothly.

### R Scripts

* `read-data.R` is an auxiliary script that is called within other scripts to import the data. 

* `auxiliary-functions.R` is an auxiliary script with several functions that we developed specifically for Bayesian digit analysis. This script is called within other scripts if necessary. 

* The tables in the poster can be reproduced with the `poster-tables-bin-beta.R` and `poster-tables-mu-dir.R` scripts.

### Supplementary Materials

* Plots comparing observed versus expected digit frequencies can be found in the `plots` folder. The code that generates the plots can be found in the `plots.R` file.

* Tables similar to the ones in the poster but with five decimal places instead of three can be found in the `aux-tables.pdf` file, stored in the `aux-tables` folder. These tables can be reproduced with the `aux-tables-bin.beta.R` and `aux-tables-mu-dir.R` files, stored in the same folder.

## Built With

* [R](https://www.r-project.org) - Free programming language and software environment for statistical computing and graphics.
* [R Studio](https://www.rstudio.com) - Free and open-source IDE for R.
* [TeX Live](https://www.tug.org/texlive/) - Free distribution of the TeX typesetting system.
* [Texmaker](https://www.xm1math.net/texmaker/) - Cross-platform and open-source LaTeX editor.

## Acknowledgments

This project was financially supported by:

* [CEMAPRE](https://cemapre.iseg.ulisboa.pt) - Center for Applied Mathematics and Economics
* [FCT](https://www.fct.pt/index.phtml.en) - Foundation for Science and Technology (Portugal). Research grant reference: SFRH/BD/129918/2017 (funded by the European Social Fund and by national funds from the MCTES)

## Contributors and Contacts

* Author: Pedro Fonseca ([ISEG](https://www.iseg.ulisboa.pt/aquila/instituicao/ISEG/)) - pedro.teles.fonseca@outlook.com 

* Advisor: Rui Paulo ([ISEG](https://www.iseg.ulisboa.pt/aquila/instituicao/ISEG/) and [CEMAPRE](https://cemapre.iseg.ulisboa.pt)) - rui@iseg.ulisboa.pt









