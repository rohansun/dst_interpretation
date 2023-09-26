# dst_interpretation
The disturbance storm time (Dst) index is a widely used metric in space weather research to measure the intensity of geomagnetic storms caused by solar activity. This project analyzed six time series models that forecast the Dst-index 1-6 hours ahead using ALE and LIME techniques to better understand the features driving the Dst index prediction.

ALE analysis showed that all six models forecast a
lower Dst index as the value of the solar wind parameter interplanetary
magnetic field (IMF) increased and a higher Dst index as the magnetic
field Bz component parameter value increased. Moreover, the models
predict a higher Dst index if the values of these two parameters are both
small or large. The same is true for the parameter pairs IMF and proton
density.

According to LIME, the parameter plasma temperature had the
most effect on the prediction of the first observation of the test set for
models that forecast 1 hour, 2 hours, 5 hours, and 6 hours ahead. And for
models that forecast 3 and 4 hours ahead, the parameter plasma speed
had the most effect on the prediction.

## Binder
This notebook is Binder enabled and can be run on mybinder.org by using the link below.

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/rohansun/dst_interpretation/HEAD)

## Installation on local machine

Tested on Python 3.9.16 and the following version of libraries
|Library | Version   | 
|---|---|
|tensorflow| 2.10.1|
|keras| 2.10.0| 
|tensorflow-probability| 0.17.0|
|numpy| 1.24.3|
| pandas|1.5.3| 
| scikit-learn | 1.2.2|
| matplotlib|3.7.1|
| matplotlib-inline| 0.1.6|
| seaborn| 0.12.2|
|scipy | 1.9.1|
|loguru | 0.7.0|
|lime | 0.2.0.1|
|alibi | 0.9.1|
|alepython|0.1.dev17+g286350a|
|protobuf | 3.19.6|
