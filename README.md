## Extending CRAN Packages with Binaries: </br> The Example of x13binary

useR! 2016 at Stanford, CA

*[Dirk Eddelbuettel](http://dirk.eddelbuettel.com) and [Christoph Sax](http://www.christophsax.com)*

The slides can be downloaded from [here](https://github.com/x13org/useR-2016/raw/master/x13useR.pdf).

#### Abstract

The [x13binary](http://cloud.r-project.org/package=x13binary) package
provides pre-built binaries of
[X-13ARIMA-SEATS](https://www.census.gov/srd/www/x13as/), the seasonal
adjustment software by the
[U.S. Census Bureau](https://www.census.gov). X-13 is a well-established
tool for de-seasonalization of timeseries, and used by statistical offices
around the world.

Other packages such as
[seasonal](http://cloud.r-project.org/package=seasonal) can now rely on
[x13binary](http://cloud.r-project.org/package=x13binary) without requiring
any intervention by the user. Together, these packages bring a very
featureful and expressive interface for working with seasonal data to the R
environment. Thanks to
[x13binary](http://cloud.r-project.org/package=x13binary), installing
[seasonal](http://cloud.r-project.org/package=seasonal) is now as easy as any
other CRAN package as it no longer requires a manual download and
setup of the corresponding binary.

Like the [Rblpapi](http://cloud.r-project.org/package=Rblpapi) package,
[x13binary](http://cloud.r-project.org/package=x13binary) provides interesting
new ways in deploying binary software to aid CRAN: A GitHub repository provides
the underlying binary in a per-operating system form (see the
[x13prebuilt](https://github.com/x13org/x13prebuilt) repository). The actual
CRAN package then uses this repo to download and install the binaries once
per installation or upgrade.

This talk will detail our approach, summarize our experience in providing
binaries via CRAN and GitHub, and discuss possible future directions.


