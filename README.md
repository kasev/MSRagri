#  Affluence, Agricultural Productivity and the Rise of Moralizing Religion in the Ancient Mediterranean

---
## Authors
* Vojtěch Kaše
* Tomáš Glomb

## License
CC-BY-SA 4.0, see attached License.md

## Description

This repository contains our analyses for a commentary article to be published in Religion, Brain & Behavior journal. The target article is "Explaining the Rise of Moralizing Religions: A test of competing hypotheses using the Seshat Databank". 
We  build on  data and analyses accompanying the target article as available from [here](https://osf.io/pa4qf/).

---
# Getting started

Our analysis aims at full reproducibility. To reproduce our analysis, follow the steps below:

* download or clone the repository
* run Python3 jupyter notebook files within the `scripts` directory using Python3 distribution and a jupyter server (local or remote). 

For that, we highly recommend to use a python 
virtual environment. To create a virtual environment for this project, 
follow the steps below:


* go to Terminal and move to the cloned directory
* run the following bash commands (modify the `$VENVNAME` variable value as you wish):
```
# check which python will be by default used as a source for your virtualenv
# (otherwise specify manually when defining the INTERPRETER variable)
which python3

# check that your pip is python 3 pip:
pip --version
# install virtualenv package
pip install virtualenv

VENVNAME=rbb_venv # choose approapriate name for your virtual environment
INTERPRETER="which python3" # or any other interpreter, e.g. $HOME/.local/lib/python-3.9.7/bin/python3
virtualenv $VENVNAME --python=$INTERPRETER

# install everything from `requirements.txt` by:
$VENVNAME/bin/python -m pip install -r requirements.txt 

# create jupyter kernel based on the environment:
$VENVNAME/bin/python -m ipykernel install --user --name=$VENVNAME

# create folder for large files:
mkdir data/large_files

```

* subsequently, in all jupyter notebooks, always check that you are connected to the correct kernel 
* (alternatively, if you do not wish to use virtual environment, make sure that you have installed all required python packages within the `requirements.txt` file: `pip install -r requiremnts.txt`)

---
