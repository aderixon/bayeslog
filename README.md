# bayeslog - a Bayesian log filter

bayeslog is a Perl script that filters standard syslog-style UNIX log
files using Bayes' Theorem (similar to the way many antispam tools filter
out unwanted email messages).

For more information, view the documentation included in the script:

    $ perldoc ./bayeslog

Note that bayeslog is very much experimental at this stage.


## Manifest

* bayeslog

  the filter script

* bayesprint

  a debugging tool to print out the current Bayes model from the storage file.


## Installation

1. Install the Algorithm::NaiveBayes module from [CPAN](http://www.cpan.org/).
2. Edit the bayeslog script and change the path to the Perl interpreter and
the extra library path if required.
3. Copy the bayeslog script to a directory in your PATH.


## Operation

See the integrated documentation or try the --help option.


## TODO list

* FIX: Strip out 'UNSURE XX/YY' from training input lines if present
(reentered output).
* Refine word weighting and interpretation.
* Improve selection of log records?
* Change keep/discard terminology to something simpler (good/bad? yes/no?)?


## Bug reports, suggestions, requests

It's experimental, you want the moon on a stick too? :-)
