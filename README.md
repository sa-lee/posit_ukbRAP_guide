# Tutorial on using Posit Workbench (Rstudio) on UKB RAP

## Overview

#### Set up

-   Setting up an Rstudio / Posit instance

    -   cost and time limits

-   Installing packages and getting bearings on where things are located

-   Setting up renv and Rstudio project

-   Linking your github credentials / cloning repository

    -   set up GITHUB PAT on github
    -   install credentials + gert to set the PAT
    -   clone repository and go to project
    -   using renv to restore R packages

#### Working with data

-   Accessing additional UKB fields with `dx extract_dataset`

    -   Setting up project credentials
    -   UKB data dictionary and fields

-   Adding data you've already got in the projects directory

-   Saving the data/results back to the cloud using `dx upload`

-   backing up work to the project using `dx-backup-folder`

-   Concluding remarks

## Additional thoughts

-   Assuming here that you can already do the analysis of interest, that you would like to do, this guide is intended more as way of showing how to retrieve data.
-   Rstudio generally seems a bit clunky on the RAP, at least compared to using DNANexus Jupyter notebook, several times throughout writing these docs my connection dropped and I lost all of my work.
-   Work that is more exploratory in nature or an analysis that you are uncertain about - it would be best to mock up the analysis outside of the RAP first. Infrastructure for doing fake data simulation might be useful - R package idea?
-   No clear documentation on switching R versions, the Posit Workbench is fixed at the moment with R4.4.0.
-   Spark compute doesn't appear to be supported in Posit Workbench (as far as I can tell, but I could be wrong here!).
-   Documentation for 'best' practices has been difficult to find
-   Everything said here is transferable to Jupyter notebook infrastructure, the dx tooling is python native, so less friction / requirement to use `system()` calls.
-   RAP is perhaps better suited for batch analysis workflows?

## Useful links and documentation

-   [DNAnexus documentation](https://dnanexus.gitbook.io/uk-biobank-rap/working-on-the-research-analysis-platform/running-analysis-jobs/rstudio)
-   [UKB tutorial repository](https://statics.teams.cdn.office.net/evergreen-assets/safelinks/1/atp-safelinks.html)
  - [UKB Best Practices guide (2023)](https://laderast.github.io/best_practices_dnanexus/)
  - [Extracting phenotypic data on UKB](https://community.ukbiobank.ac.uk/hc/en-gb/articles/26205157055261-Extracting-phenotypic-data)
  - Sng, L.M., Kaphle, A., O’Brien, M.J. et al. Optimizing UK biobank cloud-based research analysis platform to fine-map coronary artery disease loci in whole genome sequencing data. Sci Rep 15, 10335 (2025). https://doi.org/10.1038/s41598-025-95286-2
