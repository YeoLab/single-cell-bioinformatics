# Instructions for setting up iMacs at CSHL

Author: Olga Botvinnik<br>
Email: olgabot@ucsd.edu<br>
Date: 2016-06-06<br>

This document sets up fresh iMacs with no bioinformatics tools to be ready for running alignments and counting reads.

- 1. Download latest Miniconda for Python3 and save as `miniconda.sh`
```
curl https://repo.continuum.io/miniconda/Miniconda3-latest-MacOSX-x86_64.sh -o miniconda.sh
```
- 2. Install Miniconda with defaults (`-b` flag) into specific folder
```
bash miniconda.sh -b -p $HOME/miniconda
```
- 3. Add `~/miniconda/bin` to `$PATH`
```
export PATH="$HOME/miniconda/bin:$PATH"
```
- 4. Add R and [Bioconda](https://bioconda.github.io) channels
```
conda config --add channels r
conda config --add channels bioconda
```
- 5. Install Bioinformatics packages
```
conda install --yes STAR samtools subread
```
- 6. Download STAR genome
```
mkdir -p ~/genomes/mm10/gencode/m8/
cd ~/genomes/mm10/gencode/m8/
scp -r obotvinnik@tscc.sdsc.edu:/projects/ps-yeolab/biom262-2016/genomes/mm10/gencode/m8/star_chr11 . 
```
- 7. Make `shalek2013` project
```
mkdir -p ~/projects/shalek2013/raw_data ~/projects/shalek2013/processed_data ~/projects/shalek2013/scripts
```
- 8. Download `shalek2013` data subset of just chr11 for one sample
```
cd ~/projects/shalek2013/raw_data
```
