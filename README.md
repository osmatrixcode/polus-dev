# Overview

POLUS is a data processing package integrated in the workflow of the machine-learned force field FFLUX. The package mainly works on
output from molecular dynamics simulators and electronic structure calculators. It handles a list of input files, including .csv, .txt,
and .xyz files. 

POLUS performs various tasks, such as: 
- Extraction of representative subsets of geometries based on structural diversity.
- Correction of atomic IQA energies following a penalised stakeholder master equation.
- Identification of spatially equivalent atoms based on the distribution of local properties along a dynamic path.
- Stratification of datasets based on the distribution of both atomic and molecular properties.


# Prerequisites
This project requires Python 3.7.3 through 3.11.7. Versions of Python higher than 3.11.7 or lower than 3.7.3 may result in installation issues with certain packages in requirements.txt.

You can check the version of python you are using with the command:
```python --version```


# Installation

POLUS can be easily installed by following these steps:

1. Download or clone a copy of the copy. For the moment, we have only
made available the development version called "polus-dev".

2. Move inside the downloaded/cloned folder: ```cd polus-dev```
   
3. Double check if you have the correct python version installed (for this codebase).

4. ```pip install .```

We recommend that the package be installed in a dedicated virtual environment.
Assuming the name of the environment is "polus", it is easy to create one following
one of the two solutions:

1.  ```python -m venv ~/.venv/polus```

2. ```source ~/.venv/polus/bin/activate```

OR

1. ```conda create --name polus```

2. ```conda activate polus```

It's recommended to install this package in a dedicated virtual environment to isolate dependencies, including the required Python version, ensuring they only impact this codebase and don’t interfere with other projects on your system.

# Examples

The package comes with an example folder containing input files and a python script that
tests different functionalities of the code. If successfully executed, the previous script 
generates several folders and files.


