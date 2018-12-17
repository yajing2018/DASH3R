# Local Install

## Python
For the main required Python packages (numpy, scipy, etc.) we recommend using
[Anaconda for Python 3.6](https://www.continuum.io/downloads)

## Install package and dependencies for HyperMatter

### install package
    git clone https://github.com/mgoubran/hypermatter.git hypermatter

        (or install zip file and uncompress)

    cd hypermatter

### install dependencies (if want to setup virtual env skip and move to next section)
    pip install -e .[{dependency}] -process-dependency-links
where dependency is either "tf_gpu" or if you have a gpu, or "tf" otherwise.


## Setup virtual environment (if wanted)

### create environment
    conda create -n hypermatter python=3.6 anaconda

### activate the environment (start session -- needed every time)
    source activate hypermatter

### install dependencies
    pip install -e .[{dependency}] --process-dependency-links
where dependency is either "tf_gpu" or if you have a gpu, or "tf" otherwise.

### deactivate (end session)
    source deactivate

## Download deep models

    wget bla

## For tab completion
    pip3 install argcomplete
    activate-global-python-argcomplete

## To update the package

    cd hypermatter

    git pull


### if you want to delete the environment!
    conda env remove --name hypermatter