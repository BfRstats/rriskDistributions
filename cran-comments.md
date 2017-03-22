## Re-submission

This is a re-submission. In this version, we have:

* moved the image used in the README.md file into the tools subdirectory in order to ensure that the pandoc '--self-contained' option produces a "complete" README.html file


## Test environments
* ubuntu 16.10 (local install):  R under development (2017-03-22 r72383)
* ubuntu 16.10 (local install): R 3.3.3
* win-builder: R under development and R 3.2.0


## R CMD check results
There were no ERRORs or WARNINGs. 



__Our comment__: First, we'd like to apologize for failing to submit a properly checked package the last time (which led to your archiving of rriskDistributions).
We have now removed all \\donttest's, such that almost all of the previously not ran examples now are run and tested. Only in three examples, we have to use \\dontrun's: These are necessary due to tcltk windows which are used.
               
The additional NOTE under win-builder:

* Possibly mis-spelled words in DESCRIPTION:  
  Quantiles (3:53)  
  quantiles (6:14)
    
__Our comment__: We believe this NOTE to be spurious as we use title case "Quantiles" in the 'Title' field and normal lower case "quantiles" in the 'Description' field, as required by the "Writing R Extensions" manual.


## Downstream dependencies
There are currently no downstream dependencies for this package.
