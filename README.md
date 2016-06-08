[![Binder](http://mybinder.org/badge.svg)](http://mybinder.org/repo/YeoLab/single-cell-bioinformatics)

# single-cell-bioinformatics

Course material in notebook format for learning about single cell bioinformatics methods. To view this material, you have several options:

## 1. View the [live version](http://mybinder.org/repo/YeoLab/single-cell-bioinformatics) 

Where you can run and edit code (also accessible by clicking the pink "launch binder" badge above)

## 2. View the [static version](http://nbviewer.jupyter.org/github/yeolab/single-cell-bioinformatics/blob/master/index.ipynb) 

Where you cannot run or edit code, but view all the content


## 3. Set this up on your own computer

* 0. If you're using Windows, install [git](https://msysgit.github.io/)
* 1. Install [Miniconda](http://conda.pydata.org/miniconda.html) with Python 3. Command line instructions for mac and linux are shown below.
```
# Mac OS X
curl https://repo.continuum.io/miniconda/Miniconda3-latest-MacOSX-x86_64.sh > miniconda.sh

# 64-bit Linux
curl https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86_64.sh > miniconda.sh

# After downloading, install (both Mac and Linux)
bash -b miniconda.sh
```
* 2. Clone this repository and all submodules

```
git clone --recursive https://github.com/YeoLab/single-cell-bioinformatics
```
* 3. Go to the new directory
```
cd single-cell-bioinformatics
```
* 4. Create a new environment with the necessary packages
```
conda create --yes -n single-cell-bioinformatcs --file conda_requirements.txt
```
* 5. Activate the environment
```
source activate single-cell-bioinformatcs  # On windows, do "activate single-cell-bioinformatcs"
```
* 6. Install the remaiing requirements
```
pip install -r requirements.txt
```
* 7. PHEW. Now you can launch the notebooks!!
```
jupyter notebook
```

## Frozen versions of previous implementations

* [SCRM 2016](https://github.com/YeoLab/single-cell-bioinformatics-scrm-2016)


