# Watson Distribution

This repository contains a class for the Dimroth-Watson distribution.  The primary class is DimrothWatson(). It is a subclass of the [rv_continuous](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.rv_continuous.html) class in Scipy.   

The Dimroth-Watson (or just 'Watson') distribution is a distribution for the spherical polar angles, theta (inclination) and phi (azimuth).  Phi is always a unfoirm random distribution.  Given this, this class is only for modeling the distribution of theta.  

This is a 1-parameter distribution, where the shape parameter, k, can take on values between negaitve infinity and positive infinity.  For k<0, the distribution takes the form of a girdle, for k=0 the distribution is uniform, and for k>0, the distribution is bi-polar on the surface of a sphere.  

![](./notebooks/pdf_plot.png)


## Installation

Downlod this directory and place it in your PYTHONPATH.  The primary class can be imported as:

```
from watson_distribution import DimrothWatson
```


## Dependencies

* Numpy
* Scipy
* Astropy
 