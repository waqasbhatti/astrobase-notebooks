This repository contains Jupyter notebooks that show how to use the
[astrobase](https://github.com/waqasbhatti/astrobase) package.

- **[lightcurve-work](lightcurve-work.ipynb)**: demonstrates usage of
    the [hatlc](https://github.com/waqasbhatti/astrobase/blob/master/astrobase/hatsurveys/hatlc.py), [periodbase](https://github.com/waqasbhatti/astrobase/blob/master/astrobase/periodbase), and
    [checkplot](https://github.com/waqasbhatti/astrobase/blob/master/astrobase/checkplot.py) modules for reading HAT light curves,
    finding periods, and plotting phased light curves.

- **[lightcurves-and-checkplots](lightcurves-and-checkplots.ipynb)**:
    demonstrates usage of the [hatlc](https://github.com/waqasbhatti/astrobase/blob/master/astrobase/hatsurveys/hatlc.py),
    [periodbase](https://github.com/waqasbhatti/astrobase/blob/master/astrobase/periodbase), [checkplot](https://github.com/waqasbhatti/astrobase/blob/master/astrobase/checkplot.py)
    modules, and the [checkplotserver](https://github.com/waqasbhatti/astrobase/blob/master/astrobase/cpserver/checkplotserver.py) for doing
    period-finding and variability-classification work on a collection of light
    curves.

- **[parallel-ipython](parallel-ipython.ipynb)**: shows examples of
    how to map `astrobase` functions across an
    [ipyparallel](http://ipyparallel.readthedocs.io/en/stable/) cluster to speed
    up light curve processing.

# Installation

To use the notebooks in this package, git clone this repository, install
[astrobase](https://pypi.python.org/pypi/astrobase) and then invoke the Jupyter
server.

```bash

# best to do stuff in a virtualenv you've already setup (in this example: venv)
$ source venv/bin/activate

# install numpy, jupyter and astrobase
(venv) $ pip install numpy jupyter
(venv) $ pip install astrobase

# clone this repository
(venv) $ git clone https://github.com/waqasbhatti/astrobase-notebooks

# start jupyter
(venv) $ cd astrobase-notebooks
(venv) $ jupyter notebook
```

# Example data

Example light curve data from the HATNet and HATSouth surveys is available as a
[tarball](https://github.com/waqasbhatti/astrobase-notebooks/raw/master/nb-data/astrobase-example-hatlcs.tar.gz) in this repository. These are the same files used for the
notebooks. You may have to play with the file paths in the notebooks as
appropriate to get to these on your machine.

# License

These notebooks are provided under the MIT License. See the LICENSE file for the
full text.

If you use the HAT light curve data provided here for a publication, please cite
the following papers as appropriate:

- [Bakos, G., Noyes, R. W., Kovács, G., et al. 2004, PASP, 116, 266](http://adsabs.harvard.edu/abs/2004PASP..116..266B)
- [Bakos, G. Á., Csubry, Z., Penev, K., et al. 2013, PASP, 125, 154](http://adsabs.harvard.edu/abs/2013PASP..125..154B)
