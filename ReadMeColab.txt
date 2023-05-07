->This ReadMe explains the requirements and getting started to run the Interpretable Deep Learning for Dst Prediction on Colab.

->We only need to install three packages in colab as every other package is already installed.
1) To install lime package, execute the below command
    !pip install lime
2) To install alibi package, execute the below command
    !pip install alibi
3) To install ALEPython package, execute the below commands one by one
    !git clone https://github.com/blent-ai/ALEPython
    %cd ALEPython
    !pip install -r requirements.txt
    !python setup.py install
4) Restart the runtime

->Running the package:
To run ALE, execute the cells in ale-khr.ipynb files from top to bottom.
To run LIME, execute the cells in lime-khr.ipynb files from top to bottom.

