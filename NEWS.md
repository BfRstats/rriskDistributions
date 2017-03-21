# rriskDistributions 2.1.2

This release provides no new functionality and only contains two minor changes:

- moved the development repository to a new organizational github account
- moved the screenshot image in the README to the subdirectory 'tools' as requested by the CRAN maintainers


# rriskDistributions 2.1.1

This release provides no new functionality but fixes some issues:

- functions from the stats, graphics, tools, utils packages are now called via package:: to get rid of a lot of CRAN check NOTEs
- improved error/warning/message generation and handling (which also fixes a CRAN check ERROR on some platforms)

In addition, an effort was made to improve code readability by adding lots of whitespace...


# rriskDistributions 2.1

This release provides no new functionality but fixes some issues:

- rriskDistributions back on CRAN
- removal of '/donttest' calls in the examples
- better separation of GUI (tcltk windows) and underlying functionality
