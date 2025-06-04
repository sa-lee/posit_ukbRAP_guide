# Tutorial on using Posit Workbench (Rstudio) on UKB RAP

## Overview
- Setting up an Rstudio / Posit instance
    - cost and time limits
- Installing packages and getting bearings on where things are located
- Setting up renv and Rstudio project
- Linking your github credentials / cloning repository
  - set up GITHUB PAT on github
  - install credentials + gert to set the PAT
  - clone repository and go to project
  - using renv to restore R packages

- Accessing additional UKB fields with `dx extract_dataset`
  - Setting up project credentials
- Adding data you've already got in the project
- Proteomics workflow example (if time permits)
    - installing additional packages
    - basic run through QC steps 
    - Association of protein measurements with limma-voom on a PRS covariate adjusting for potential batch effects

- Saving the data/results back to the cloud using `dx upload`
- backing up work to the project using `dx-backup-folder`

## Useful links and documentation

* [DNAnexus documentation](https://dnanexus.gitbook.io/uk-biobank-rap/working-on-the-research-analysis-platform/running-analysis-jobs/rstudio)
* [UKB tutorial repository](https://statics.teams.cdn.office.net/evergreen-assets/safelinks/1/atp-safelinks.html)
