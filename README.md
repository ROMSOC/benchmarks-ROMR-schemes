<img src="images/romsoclogo-logo.png" alt="ROMSOC logo"  width="150"/>

# Benchmarks for the application of reduced order multirate schemes
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5171813.svg)](https://doi.org/10.5281/zenodo.5171813) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ROMSOC/benchmarks-ROMR-schemes/HEAD?labpath=ROMSOC.ipynb)

## Summary
This document presents a benchmark case for the application of reduced order multirate schemes in a MATLAB/Octave environment.

## Description
The benchmark case can be run using the script file ``ROMSOC.m``. 

### Run Jupyter notebooks
The entire benchmark repository can be executed in a provided Docker container where a full installation of Octave is available. Once you have clone or downloaded this repository, to build the container just type
```bash
docker build -t benchmarks-ROMR-schemes . 
```
and for running it locally:
```bash
docker run -it --rm -p 8888:8888 benchmarks-ROMR-schemes jupyter-lab --ip=0.0.0.0 --port=8888 --allow-root
```
Alternatively, please use the following link to run a user-friendly Jupyter Notebook ``ROMSOC.ipynb`` where the same benchmarks are implemented:
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ROMSOC/benchmarks-ROMR-schemes/HEAD?labpath=ROMSOC.ipynb) Please, notice that mybinder cloud computations are limited to 2GB of RAM memory.

## Directory structure
```
.
├── Circuits
├── Components
│   ├── Diodes
│   ├── MOSFETS
│   └── Vsources
├── Documentation
├── Numerical
│   ├── Integration
│   ├── Jacobian
│   ├── MOR
│   ├── NonLinear
│   └── Visual
├── Parser
├── Images
├── CITATION
├── CONTRIBUTORS
├── LICENSE
├── README
├── ROMSOC.m
└── .gitignore
```
## Disclaimer
In downloading this SOFTWARE you are deemed to have read and agreed to the following terms:
This SOFTWARE has been designed with an exclusive focus on civil applications. It is not to be used
for any illegal, deceptive, misleading or unethical purpose or in any military applications. This includes ANY APPLICATION WHERE THE USE OF THE SOFTWARE MAY RESULT IN DEATH,
PERSONAL INJURY OR SEVERE PHYSICAL OR ENVIRONMENTAL DAMAGE. Any redistribution of the software must retain this disclaimer. BY INSTALLING, COPYING, OR OTHERWISE
USING THE SOFTWARE, YOU AGREE TO THE TERMS ABOVE. IF YOU DO NOT AGREE TO
THESE TERMS, DO NOT INSTALL OR USE THE SOFTWARE

## Acknowledgments
<img src="images/EU_Flag.png" alt="EU Flag"  width="150" height="100" />

The ROMSOC project has received funding from the European Union’s Horizon 2020 research and innovation programme under the Marie Skłodowska-Curie Grant Agreement No. 765374.
This repository reflects the views of the author(s) and does not necessarily reflect the views or policy of the European Commission. The REA cannot be held responsible for any use that may be made of the information this repository contains.
