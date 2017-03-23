## Re-submission

This is a re-submission. In this version, we have:

* moved the image used in the README.md file into the tools subdirectory in order to ensure that the pandoc '--self-contained' option produces a "complete" README.html file


## Test environments
* ubuntu 16.10 (local install):  R under development (2017-03-22 r72383)
* ubuntu 16.10 (local install): R 3.3.3
* win-builder: R version 3.3.3 (2017-03-06)
* win-builder: R Under development (unstable) (2017-03-21 r72375)


## R CMD check results
There were no ERRORs or WARNINGs. 

The additional NOTE under win-builder:

* Possibly mis-spelled words in DESCRIPTION:  
  Quantiles (3:53)  
  quantiles (6:14)
    
__Our comment__: We believe this NOTE to be spurious as we use title case "Quantiles" in the 'Title' field and normal lower case "quantiles" in the 'Description' field, as required by the "Writing R Extensions" manual.


## Downstream dependencies
decisionSupprt suggests rriskDistributions, a check was passed without errors via
tools::check_packages_in_dir(
    check_args = c("--as-cran", ""),
    reverse = list(repos = getOption("repos")["CRAN"], which = "most")
)
