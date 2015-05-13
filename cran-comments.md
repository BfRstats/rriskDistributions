## Re-submission

This is a re-submission. In this version, we have:

* removed all unnecessary \\donttest's (more detail below)
* moved packages from 'Depends' to 'Imports' in the DESCRIPTION and changed the NAMESPACE and function calls accordingly


## Test environments
* ubuntu 14.04 LTS (local install):  R under development (2015-05-06 r68336) and R 3.1.3
* windows 7 (local install): R 3.2.0
* win-builder: R under development and R 3.2.0


## R CMD check results
There were no ERRORs or WARNINGs. 

There was 1 common NOTE and 1 additional NOTE under win-builder.
The common NOTE:

* checking CRAN incoming feasibility ... NOTE  
  Maintainer: ‘Matthias Greiner <matthias.greiner@bfr.bund.de>’  
  New submission  
  Package was archived on CRAN  
  CRAN repository db overrides:  
    X-CRAN-Comment: Archived on 2015-03-13 as misuse of \\donttest was not
      corrected.

__Our comment__: First, we'd like to apologize for failing to submit a properly checked package the last time (which led to your archiving of rriskDistributions).
We have now removed all \\donttest's, such that allmost all of the previously not ran examples now are run and tested. Only in three examples, we have to use \\dontrun's: These are necessary due to tcltk windows which are used.
               
The additional NOTE under win-builder:

* Possibly mis-spelled words in DESCRIPTION:  
  Quantiles (3:53)  
  quantiles (6:14)
    
__Our comment__: We believe this NOTE to be spurious as we use title case "Quantiles" in the 'Title' field and normal lower case "quantiles" in the 'Description' field, as required by the "Writing R Extensions" manual.


## Downstream dependencies
There are currently no downstream dependencies for this package.
