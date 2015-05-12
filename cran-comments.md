## Test environments
* ubuntu 14.04 LTS (local install):  R under development (2015-05-06 r68336) and R 3.1.3
* win-builder: R under development and R 3.2.0

## R CMD check results
There were no ERRORs or WARNINGs. 

There was 1 commen NOTE and 1 additional NOTE under win-builder.
The common NOTE:

* checking CRAN incoming feasibility ... NOTE
  Maintainer: ‘Matthias Greiner <matthias.greiner@bfr.bund.de>’
  New submission
  Package was archived on CRAN
  CRAN repository db overrides:
    X-CRAN-Comment: Archived on 2015-03-13 as misuse of \donttest was not
      corrected.

  Our comment: We removed all \\donttests, such that allmost all of the previously not ran examples
               now are run and tested. Only in three examples, we have to use \\dontruns: These are
               necessary due to tcltk windows which are used.
               
The additional NOTE under win-builder:
  * Possibly mis-spelled words in DESCRIPTION:
      Quantiles (3:53)
      quantiles (6:14)
      
    Our comment: Our comment: We believe this NOTE to be spurious as we use title case
                "Quantiles" in the Title field and lower case "quantiles" in the
                 Description field, as required by the "Writing R Extensions" manual.


## Downstream dependencies
**TODO**
