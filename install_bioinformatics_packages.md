# Instructions for installing bioinformatics packages.

Author: Olga Botvinnik<br>
Email: olgabot@ucsd.edu<br>
Date: 2016-06-09<br>

This document sets up computers with no bioinformatics tools to be ready for running alignments and counting reads. This assumes you have the [Anaconda](https://www.continuum.io/downloads) package manager installed.

- 1. Add R and [Bioconda](https://bioconda.github.io) channels
```
$ conda config --add channels r
$ conda config --add channels bioconda
```
- 2. Install Bioinformatics packages
```
$ conda install --yes STAR samtools subread bedtools cutadapt fastqc
```
