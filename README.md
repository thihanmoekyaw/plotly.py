# plotly.py

<table>
    <tr>
        <td>Latest Release</td>
        <td>
            <a href="https://pypi.org/project/plotly/"/>
            <img src="https://badge.fury.io/py/plotly.svg"/>
        </td>
    </tr>
    <tr>
        <td>User forum</td>
        <td>
            <a href="https://community.plotly.com/"/>
            <img src="https://img.shields.io/badge/help_forum-discourse-blue.svg"/>
        </td>
    </tr>
    <tr>
        <td>PyPI Downloads</td>
        <td>
            <a href="https://pepy.tech/project/plotly"/>
            <img src="https://pepy.tech/badge/plotly/month"/>
        </td>
    </tr>
    <tr>
        <td>License</td>
        <td>
            <a href="https://opensource.org/licenses/MIT"/>
            <img src="https://img.shields.io/badge/License-MIT-yellow.svg"/>
        </td>
    </tr>
</table>

## Quickstart

`pip install plotly==5.13.1`

Inside [Jupyter](https://jupyter.org/install) (installable with `pip install "jupyterlab>=3" "ipywidgets>=7.6"`):

```python
import plotly.express as px
fig = px.bar(x=["a", "b", "c"], y=[1, 3, 2])
fig.show()
```

See the [Python documentation](https://plotly.com/python/) for more examples.


## Overview

[plotly.py](https://plotly.com/python/) is an interactive, open-source, and browser-based graphing library for Python :sparkles:

Built on top of [plotly.js](https://github.com/plotly/plotly.js), `plotly.py` is a high-level, declarative charting library. plotly.js ships with over 30 chart types, including scientific charts, 3D graphs, statistical charts, SVG maps, financial charts, and more.

`plotly.py` is [MIT Licensed](https://github.com/plotly/plotly.py/blob/master/LICENSE.txt). Plotly graphs can be viewed in Jupyter notebooks, standalone HTML files, or integrated into [Dash applications](https://dash.plotly.com/).

[Contact us](https://plotly.com/consulting-and-oem/) for consulting, dashboard development, application integration, and feature additions.

<p align="center">
    <a href="https://plotly.com/python/" target="_blank">
    <img src="https://raw.githubusercontent.com/cldougl/plot_images/add_r_img/plotly_2017.png">
</a></p>

---

- [Online Documentation](https://plotly.com/python/)
- [Contributing to plotly](https://github.com/plotly/plotly.py/blob/master/contributing.md)
- [Changelog](https://github.com/plotly/plotly.py/blob/master/CHANGELOG.md)
- [Code of Conduct](https://github.com/plotly/plotly.py/blob/master/CODE_OF_CONDUCT.md)
- [Version 4 Migration Guide](https://plotly.com/python/v4-migration/)
- [New! Announcing Dash 1.0](https://medium.com/plotly/welcoming-dash-1-0-0-f3af4b84bae)
- [Community forum](https://community.plotly.com)

---

## Installation

plotly.py may be installed using pip...

```
pip install plotly==5.13.1
```

or conda.

```
conda install -c plotly plotly=5.13.1
```

### JupyterLab Support

For use in [JupyterLab](https://jupyterlab.readthedocs.io/en/stable/), install the `jupyterlab` and `ipywidgets`
packages using `pip`:

```
pip install "jupyterlab>=3" "ipywidgets>=7.6"
```

or `conda`:

```
conda install "jupyterlab>=3" "ipywidgets>=7.6"
```

The instructions above apply to JupyterLab 3.x. **For JupyterLab 2 or earlier**, run the following commands to install the required JupyterLab extensions (note that this will require [`node`](https://nodejs.org/) to be installed):

```
# JupyterLab 2.x renderer support
jupyter labextension install jupyterlab-plotly@5.13.1 @jupyter-widgets/jupyterlab-manager
```

Please check out our [Troubleshooting guide](https://plotly.com/python/troubleshooting/) if you run into any problems with JupyterLab.

### Jupyter Notebook Support

For use in the Jupyter Notebook, install the `notebook` and `ipywidgets`
packages using `pip`:

```
pip install "notebook>=5.3" "ipywidgets>=7.5"
```

or `conda`:

```
conda install "notebook>=5.3" "ipywidgets>=7.5"
```

### Static Image Export

plotly.py supports [static image export](https://plotly.com/python/static-image-export/),
using either the [`kaleido`](https://github.com/plotly/Kaleido)
package (recommended, supported as of `plotly` version 4.9) or the [orca](https://github.com/plotly/orca)
command line utility (legacy as of `plotly` version 4.9).

#### Kaleido

The [`kaleido`](https://github.com/plotly/Kaleido) package has no dependencies and can be installed
using pip...

```
pip install -U kaleido
```

or conda.

```
conda install -c conda-forge python-kaleido
```

#### Orca

While Kaleido is now the recommended image export approach because it is easier to install
and more widely compatible, [static image export](https://plotly.com/python/static-image-export/)
can also be supported
by the legacy [orca](https://github.com/plotly/orca) command line utility and the
 [`psutil`](https://github.com/giampaolo/psutil) Python package.

These dependencies can both be installed using conda:

```
conda install -c plotly plotly-orca==1.3.1 psutil
```

Or, `psutil` can be installed using pip...

```
pip install psutil
```

and orca can be installed according to the instructions in the [orca README](https://github.com/plotly/orca).


### Extended Geo Support

Some plotly.py features rely on fairly large geographic shape files. The county
choropleth figure factory is one such example. These shape files are distributed as a
separate `plotly-geo` package. This package can be installed using pip...

```
pip install plotly-geo==1.0.0
```

or conda

```
conda install -c plotly plotly-geo=1.0.0
```

## Migration

If you're migrating from plotly.py v3 to v4, please check out the [Version 4 migration guide](https://plotly.com/python/v4-migration/)

If you're migrating from plotly.py v2 to v3, please check out the [Version 3 migration guide](https://github.com/plotly/plotly.py/blob/master/migration-guide.md)

## Copyright and Licenses

Code and documentation copyright 2019 Plotly, Inc.

Code released under the [MIT license](https://github.com/plotly/plotly.py/blob/master/LICENSE.txt).

Docs released under the [Creative Commons license](https://github.com/plotly/documentation/blob/source/LICENSE).
