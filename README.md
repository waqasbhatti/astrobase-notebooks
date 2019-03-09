This repository contains Jupyter notebooks that show how to use the
[astrobase](https://github.com/waqasbhatti/astrobase) package.

- **lightcurve-work.ipynb ([Jupyter nbviewer](https://nbviewer.jupyter.org/github/waqasbhatti/astrobase-notebooks/blob/master/lightcurve-work.ipynb))**: demonstrates usage of
    the [hatlc](https://astrobase.readthedocs.io/en/latest/astrobase.hatsurveys.hatlc.html), [periodbase](https://astrobase.readthedocs.io/en/latest/astrobase.periodbase.html), and
    [checkplot](https://astrobase.readthedocs.io/en/latest/astrobase.checkplot.html) modules for reading HAT light curves,
    finding periods, and plotting phased light curves.

- **lightcurves-and-checkplots.ipynb ([Jupyter nbviewer](https://nbviewer.jupyter.org/github/waqasbhatti/astrobase-notebooks/blob/master/lightcurves-and-checkplots.ipynb))**:
    demonstrates usage of the [hatlc](https://astrobase.readthedocs.io/en/latest/astrobase.hatsurveys.hatlc.html),
    [periodbase](https://astrobase.readthedocs.io/en/latest/astrobase.periodbase.html), [checkplot](https://astrobase.readthedocs.io/en/latest/astrobase.checkplot.html)
    modules, and the [checkplotserver](https://astrobase.readthedocs.io/en/latest/astrobase.cpserver.html) for doing
    period-finding and variability-classification work on a collection of light
    curves.

- **lc-collection-work.ipynb ([Jupyter nbviewer](https://nbviewer.jupyter.org/github/waqasbhatti/astrobase-notebooks/blob/master/lc-collection-work.ipynb))**: demonstrates usage of the
    [lcproc](https://astrobase.readthedocs.io/en/latest/astrobase.lcproc.html)
    module to process a collection of light curves in an arbitrary format in
    order to prepare them for review by
    [checkplotserver](https://astrobase.readthedocs.io/en/latest/astrobase.cpserver.html). This
    goes through all the various features one can add to checkplots, ranging
    from neighbor info, cross-matching, and color-magnitude diagrams.

- **lcc-server-setup.ipynb ([Jupyter nbviewer](https://nbviewer.jupyter.org/github/waqasbhatti/astrobase-notebooks/blob/master/lcc-server-setup.ipynb))**:
  describes how to use astrobase products like period-finding pickles and
  checkplot pickles to feed into the
  [LCC-Server](https://github.com/waqasbhatti/lcc-server), a browser interface
  for searching through collections of light curves in various ways.


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

- HATNet - [Bakos, G., Noyes, R. W., Kovács, G., et al. 2004, PASP, 116, 266](http://adsabs.harvard.edu/abs/2004PASP..116..266B)
- HATSouth - [Bakos, G. Á., Csubry, Z., Penev, K., et al. 2013, PASP, 125, 154](http://adsabs.harvard.edu/abs/2013PASP..125..154B)
