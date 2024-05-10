# ML problems for the EIROForum summer school of May 2024

Each Jupyter notebook contains a problem to be solved with ML. The data is described and can be obtained in each
notebook. Some of it is downloaded from somewhere, while others are simply randomly generated on-the-fly.

The following instructions show how to setup your environment, so that you can easily play with the data.

All the data used in the examples are produced on-the-fly for demonstration purposes, or are taken from public and open resources.

## Anaconda setup

Using Anaconda or Miniconda, create an environment as follows.

```
# create the environment
conda create -n ml

# load it
conda activate ml

# install some packages to get started
conda install jupyterlab
mamba install pytorch torchvision torchaudio cpuonly -c pytorch
mamba install -c conda-forge numpy scipy scikit-learn pandas matplotlib seaborn gpytorch botorch
pip install torchbnn

# play with the notebooks ...
jupyter lab

# when you are done:
conda deactivate
```

## Virtualenv setup

Using a virtual environment,
the setup would be the following (for an environment called `env`, but use the name
you prefer):

```
# create the environment
python -m venv env

# load it
source env/bin/activate

# install some packages to get started
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cpu
pip install numpy scipy scikit-learn pandas matplotlib seaborn gpytorch botorch torchbnn jupyterlab

# play with the notebooks ...
jupyter lab

# when you are done:
deactivate
```

