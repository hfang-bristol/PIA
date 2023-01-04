# [An R package `PIA`](https://github.com/hfang-bristol/PIA)

## @ Overview

> The `PIA` is an R package enabling genomics-led target prioritisation and crosstalk-based drug repurposing for asthma.


## @ Installation

### 1. Install R

Please install R (version 4.2.1 or above); see https://cran.r-project.org

If installed on `Ubuntu` (assuming you have a `ROOT (sudo)` privilege), please do so below

```ruby
sudo su
# here enter your password

wget http://www.stats.bris.ac.uk/R/src/base/R-4/R-4.2.1.tar.gz
tar xvfz R-4.2.1.tar.gz
cd ~/R-4.2.1
./configure
make
make check
make install
R # start R
```

### 2. Install R packages

```ruby
R # start R

# if the package 'BiocManager' not installed, please do so
if(!("BiocManager" %in% rownames(installed.packages()))) install.packages("BiocManager")

# first, install basic packages: remotes, tidyverse
BiocManager::install(c('remotes','tidyverse'), dependencies=T)

# then, install the package 'PIA' (now hosted at github)
BiocManager::install("hfang-bristol/PIA", dependencies=T, force=T)

# check the package 'PIA' successfully installed
library(PIA)
```


## @ Showcase

> A showcase describing a step-by-step protocol on how to genetic targets and repurposed drugs for asthma is made available and reproducible [`here`](http://www.genetictargets.pro/PIA/showcase).


## @ Contact

> Please drop [email](mailto:fh12355@rjh.com.cn) for bug reports or other enquiries.


