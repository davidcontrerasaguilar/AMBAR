# BrecSys

A new fairness Dataset

## How to

These notebooks were tested using Python 3.8. A virtual environment is highly recommended.

```shell
python -m venv venv
source ./venv/bin/activate
```

The required packages are:

- tqdm: used for showing progress in some loops.
- numpy: used for data manipulation.
- pandas: used for data manipulation.
- cornac: used for obtaining the recommendations.

These can be installed (alongside some extra packages) using the requirements.txt provided.

```shell
python -m pip install --upgrade pip
python -m pip install -r ./requirements.txt
```

For running the notebooks, Jupyter is required and needs to be installed in the virtual environment (not included in
requirements.txt).

## Cornac

For running cornac on the data provided, use the notebook Cornac.ipynb where the process is explained. Some variables
were provided so it can be adapted to other use cases. The data used for this script is found in data/BRecSys.

## PyCPFair

For running PyCPFair on the data provided, use the notebook PyCPFair.ipynb. The main process is found in the process
section.
The data for this script is separated and based on the full set. This data may be found in data/PyCPFair.

## PFair

TODO