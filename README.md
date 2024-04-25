# Introduction

This is my submission for the *Finding Donors for CharityML* project as part of the Udacity nanodegree [Introduction to Machine Learning with TensorFlow](https://learn.udacity.com/nanodegrees/nd230). The point of this project is to demonstrate understanding of scikit-learn and supervised learning concepts through a toy classification task.  The task is to identify potential donors for a fictitious organization (CharityML) by classifying individuals by income ("<=$50K" and ">$50K").  This closely resembles the related [*ML Charity* Kaggle competition](https://www.kaggle.com/competitions/udacity-mlcharity-competition).

I have left the provided file structure unchanged for ease of review. The public repo for this project is available here:

https://github.com/udacity/cd0025-supervised-learning/tree/master/starter

# Setup
This section outlines how to setup to run locally using `pyenv` to control virtual environments and using separate environments for `jupyter lab` and the IPython kernel used by `jupyter lab` to run all calculations.

## Jupyter lab
This step is optional if you already have `jupyter lab` set up.

```
# create virtual environment
pyenv install 3.11.7
pyenv virtualenv 3.11.7 jupyter
pyenv activate jupyter

# install jupyter lab
python3 -m pip install --upgrade pip
python3 -m pip install -r jupyter-requirements.txt
pyenv deactivate jupyter
```

## IPython kernel
```
# create virtual environment
pyenv install 3.11.7
pyenv virtualenv 3.11.7 udacity-finding-donors
pyenv local udacity-finding-donors
python3 -m pip install --upgrade pip

# clone git repo and install requirements
git clone git@github.com:mrperkett/udacity-project-finding-donors.git
cd udacity-project-finding-donors/
python3 -m pip install -r requirements.txt

# register IPython kernel
python3 -m ipykernel install --user --name udacity-finding-donors
```

# Running
```
# If you have named your jupyter python virtual environment something other than "jupyter", modify the line below
pyenv activate jupyter
jupyter lab
```

If you have successfully registered your IPython kernel, you should be able to open `finding-donors/finding_donors.ipynb` notebook in the newly launched Jupyter Lab webpage and select the *udacity-finding-donors* kernel to run it.

# Data
Additional links to the original data set for further exploration:
- https://archive.ics.uci.edu/ml/machine-learning-databases/adult/adult.names
- https://archive.ics.uci.edu/dataset/2/adult


# Results
- All work was completed in the following Jupyter notebook: [finding_donors.ipynb](finding-donors/finding_donors.ipynb)
  - run time for full notebook: 16 mins
- An HTML export of the notbook can be found here: [report.html](finding-donors/report.html)
- I have marked cells where I do work outside of what was explicitly requested as *scratchwork*