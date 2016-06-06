# Instructions for setting up iMacs at CSHL

Author: Olga Botvinnik<br>
Email: olgabot@ucsd.edu<br>
Date: 2016-06-06<br>

This document sets up fresh iMacs with no bioinformatics tools to be ready for running alignments and counting reads.

1. Download latest Miniconda for Python3 and save as `miniconda.sh`
```
curl https://repo.continuum.io/miniconda/Miniconda3-latest-MacOSX-x86_64.sh -o miniconda.sh
```
2. Install Miniconda with defaults (`-b` flag) into specific folder
```
bash miniconda.sh -b -p $HOME/miniconda
```
3. Add `~/miniconda/bin` to `$PATH`
```
export PATH="$HOME/miniconda/bin:$PATH"
```
4. Add R and [Bioconda](bioconda.github.io) channels
```
conda config --add channels r
conda config --add channels bioconda
```
5. Install Bioinformatics packages

```
conda install --yes STAR samtools subread
```
