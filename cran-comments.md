## Test environments
* local OS X install, R 3.4.2
* ubuntu 14.04 (on travis-ci), R 3.4.2
* win-builder (devel and release submitted)
* AppVeyor, R-release
* r-hub Windows Server 2008 R2 SP1, R-release, 32/64 bit

## R CMD check results

0 errors | 0 warnings | 1 note

* This is a new release.

## Reverse dependencies

This is a new release, so there are no reverse dependencies.

---

Some tests and parts of examples do not run on CRAN due to being calls to external APIs. These are run on Travis (<https://travis-ci.org/hrbrmstr/voteogram>), AppVeyor (<https://ci.appveyor.com/project/hrbrmstr/voteogram>) and when building the README so they are tested frequently.

`roll_call()` cannot (well, shouldn't) be tested on CRAN as it makes external API calls to a service run bu a non-profit.

Resolved earlier submission issue (README dependent files issue). It's def weird that neither r-hub nor travis catches the same thing.

Code coverage is 73% <https://codecov.io/github/hrbrmstr/voteogram?branch=master> and will be improved for the next submission.
