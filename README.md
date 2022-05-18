[![License](https://img.shields.io/badge/License-MIT%202.0-blue.svg)](https://opensource.org/licenses/MIt)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-blue.svg)](https://github.com/Kohulan/STOUT-2/graphs/commit-activity)
![Workflow](https://github.com/OBrink/RanDepict/actions/workflows/ci_pytest.yml/badge.svg)
[![GitHub issues](https://img.shields.io/github/issues/Kohulan/STOUT-2.svg)](https://GitHub.com/Kohulan/STOUT-2/issues/)
[![GitHub contributors](https://img.shields.io/github/contributors/Kohulan/STOUT-2.svg)](https://GitHub.com/Kohulan/STOUT-2/graphs/contributors/)
[![GitHub release](https://img.shields.io/github/release/Kohulan/STOUT-2.svg)](https://GitHub.com/Kohulan/STOUT-2/releases/)
[![PyPI version fury.io](https://badge.fury.io/py/STOUT-2.svg)](https://pypi.python.org/pypi/STOUT-2/)
![versions](https://img.shields.io/pypi/pyversions/STOUT-2.svg)

![GitHub Logo](https://github.com/Kohulan/STOUT-2/blob/main/Stout-2.png?raw=true)

This repository contains STOUT-V2, SMILES to IUPAC name translator using transformers. STOUT-V2 can translate SMILES to IUPAC names and IUPAC names back to a valid SMILES string. STOUT-V1 is already publiahed and for more details check [here](https://github.com/Kohulan/Smiles-TO-iUpac-Translator)

#### OS-Support: Linux, MACOS and Windows (On Windows you can run STOUT inside the Ubuntu shell). But It is highly recommended to use a Linux system.

# Usage

### We suggest to use STOUT inside a Conda environment, which makes the dependencies to install easily.
- Conda can be downloaded as part of the [Anaconda](https://www.anaconda.com/) or the [Miniconda](https://conda.io/en/latest/miniconda.html) plattforms (Python 3.7). We recommend to install miniconda3. Using Linux you can get it with:
```shell
$ wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
$ bash Miniconda3-latest-Linux-x86_64.sh
```
## How to install STOUT

```shell
$ sudo apt update
$ sudo apt install unzip
$ conda create --name STOUT python=3.7.9
$ conda activate STOUT
$ conda install pip
$ python -m pip install -U pip
$ pip install git+https://github.com/Kohulan/STOUT-2.git
```

## Py-Pi installation instructions coming soon,
```shell

```


## Simple usage
```python3

from STOUT import translate_forward, translate_reverse

# SMILES to IUPAC name translation

SMILES = "CN1C=NC2=C1C(=O)N(C(=O)N2C)C"
IUPAC_name = translate_forward(SMILES)
print("IUPAC name of "+SMILES+" is: "+IUPAC_name)

# IUPAC name to SMILES translation

IUPAC_name = "1,3,7-trimethylpurine-2,6-dione"
SMILES = translate_reverse(IUPAC_name)
print("SMILES of "+IUPAC_name+" is: "+SMILES)

```




# STOUT-V2 is part of DECIMER project
[![GitHub Logo](https://github.com/Kohulan/DECIMER-Image-to-SMILES/raw/master/assets/DECIMER.gif)](https://kohulan.github.io/Decimer-Official-Site/)

# More about Us

[![GitHub Logo](https://github.com/Kohulan/DECIMER-Image-to-SMILES/blob/master/assets/CheminfGit.png?raw=true)](https://cheminf.uni-jena.de)
