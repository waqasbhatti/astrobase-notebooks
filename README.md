This repository contains Jupyter notebooks that show how to use the
[astrobase](https://github.com/waqasbhatti/astrobase) package.

- **[lightcurve-work](lightcurve-work.ipynb)**: demonstrates usage of
    the [hatlc](https://github.com/waqasbhatti/astrobase/hatlc.py), [periodbase](https://github.com/waqasbhatti/periodbase), and
    [checkplot](https://github.com/waqasbhatti/astrobase/checkplot.py) modules for reading HAT light curves,
    finding periods, and plotting phased light curves.

- **[lightcurves-and-checkplots](lightcurves-and-checkplots.ipynb)**:
    demonstrates usage of the [hatlc](https://github.com/waqasbhatti/astrobase/hatlc.py),
    [periodbase](https://github.com/waqasbhatti/astrobase/periodbase), [checkplot](https://github.com/waqasbhatti/astrobase/checkplot.py)
    modules, and the [checkplotserver](https://github.com/waqasbhatti/astrobase/checkplotserver.py) for doing
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

# License

These notebooks are provided under the MIT License. See the LICENSE file for
the full text.
