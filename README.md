This notebook is Binder enabled and can be run on mybinder.org by using the link below.

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/rohansun/dst_interpretation/HEAD)

->This ReadMe explains the requirements and getting started to run the Interpretable Deep Learning for Dst Prediction.

->Tested on Windows 11 and Python 3.9.16

The following python packages and modules are required to run Interpretable Deep Learning for Dst Prediction:
tensorflow==2.10.1
keras==2.10.0
tensorflow-probability==0.17.0
numpy==1.24.3
pandas==1.5.3
scikit-learn==1.2.2
matplotlib==3.7.1
matplotlib-inline==0.1.6
seaborn==0.12.2
scipy==1.9.1
loguru==0.7.0
lime==0.2.0.1
alibi==0.9.1
protobuf==3.19.6


->To install the above mentioned packages and modules, copy the above packages into a text file called "requirements.txt" and then execute the following command. 

pip install -r requirements.txt

->In addition to the above mentioned packages, there is one other important package called ALEPython that needs to be installed. You can install this package by executing the following command.

git clone https://github.com/blent-ai/ALEPython && cd ALEPython && pip install -r requirements.txt && python setup.py install

->This package was tested on alepython version 0.1.dev17+g286350a

Note: If you run into an error while running the program, make sure the version of Python and the libraries you are using are the same as above.


Package Structure:
After downloading the zip file, the package includes the following folders and files

1) README.md - this ReadMe file.
2) environment.yml - includes the packages and modules required and their versions.
3) data - Data sets to train and interpret models that forecast Dst index 1-6 hrs ahead.
4) models - Directory in which the weights of six trained models are saved.
5) DSTT-model-and-utils - folder that contains the following four Python files.
	DSTT_model.py - Used for Loading the trained models and Predicting on data inorder to interpret.
	DSTT_utils.py - Used for retrieving the data present in the 'data' folder.
	Attention.py - implements Attention layer of DSTT.
	DSTT_dropout.py - implements Custom Monte Carlo Dropout for DSTT.
6) ale-khr.ipynb - Jupyter notebook files for global interpretation of the models. They implement ALE on models that forecast Dst index k = 1-6 hrs ahead.
7) lime-khr.ipynb - Jupyter notebook files for local interpretation of the models. They implement LIME on models that forecast Dst index k = 1-6 hrs ahead.  

Note: DSTT refers to the Dst Transformer referred here https://github.com/ccsc-tools/Dst-prediction 

Running the package:
To run ALE, execute the cells in ale-khr.ipynb files from top to bottom.
To run LIME, execute the cells in lime-khr.ipynb files from top to bottom.
