->This ReadMe explains the requirements and getting started to run the Interpretable Deep Learning for Dst Prediction on Linux.

->Tested on Ubuntu 22.04.2 LTS and Python 3.9.16

->To run on Linux: 
1) Install miniconda from https://docs.conda.io/projects/conda/en/latest/user-guide/install/linux.html
2) Create a new environment by typing the below command
    conda create -n <env_name> python=3.9.16 jupyter
3) Install the below mentioned libraries
    tensorflow==2.12.0
    keras==2.12.0
    tensorflow-probability==0.14.0
    numpy==1.23.5
    pandas==1.5.3
    scikit-learn==1.2.2
    matplotlib==3.7.1
    matplotlib-inline==0.1.6
    seaborn==0.12.2
    scipy==1.9.1
    loguru==0.7.0
    lime==0.2.0.1
    alibi==0.9.2
    protobuf==3.20.3
4) Also install ALEPython package by typing the below command
    pip install git+https://github.com/MaximeJumelle/ALEPython.git@dev#egg=alepython
    This package was tested on alepython version 0.1.dev17+g286350a
    
->Running the package:
To run ALE, execute the cells in ale-khr.ipynb files from top to bottom.
To run LIME, execute the cells in lime-khr.ipynb files from top to bottom.
