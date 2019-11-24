Case 0 - K8S
=============

ACME Co. wants increase its relevance as certified member of  [Cloud Native Computing Foundation](https://www.cncf.io) and wants offer specialized support for a popular software called Kubernetes. ACME wants to be an active contributor to the project as payment CNFC membership. ACME agreement with needs to be monitored in order to accomplish SLAs and estimated budget.

ACME membership to CNFC cost about 370.000 \$ in cash, but current agreement with CNCF increases this budget up to 400.000 \$ expent in human resources part of ACME. 

ACME and CNCF wants monitor this agreement in this points:

* Issues
  
  * Number of issues that remains open in a particular moment.
  
  * Average open and closed issues between 2 weeks

* Contributions
  
  * Active contributors
  
  * Number of pull requests
  
  * Most updated files



## Exercise 1: Load Sources

Load JSON sources from 'cases/k8s/resources



## Exercise 2: First Dashboard - Issues







# Technical Helps

Cummulative issues group by closed date

`Cumulative Closed Issues = CALCULATE (
    SUM ( 'Issues Closed by Date'[Issues Closed] );
    ALL ( 'Issues Closed by Date' );
    'Issues Closed by Date'[Issues.closed_at] <= EARLIER ( 'Issues Closed by Date'[Issues.closed_at] )
)`


