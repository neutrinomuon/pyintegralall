# IntegralALL
##  A fortran legacy package to easy integrate numerically
email: antineutrinomuon@gmail.com, jean@astro.up.pt

© Copyright ®

J.G. - Jean Gomes

<hr>

[![My Skills](https://skillicons.dev/icons?i=python,fortran,c,numpy&theme=light)](https://skillicons.dev)<br>
[![python3](https://img.shields.io/pypi/pyversions/pyintegralall)](https://img.shields.io/pypi/pyversions/pyintegralall)
[![lastcommit](https://img.shields.io/github/last-commit/neutrinomuon/IntegralALL)](https://img.shields.io/github/last-commit/neutrinomuon/IntegralALL)
[![badgetlicense](https://anaconda.org/neutrinomuon/pyintegralall/badges/license.svg)](https://anaconda.org/neutrinomuon/pyintegralall/badges/license.svg)

<hr>

RESUME : Integrate arrays, functions numerically using different
methods. Original Fortran 2003+ routines date back to 2003-2004. Read the
LICENSE.txt file.

You can easily install by using pip:
<pre>
<code>
pip install pyintegralall
</code>
</pre>
or by using a generated conda repository <a href='https://anaconda.org/neutrinomuon/pyintegralall'>https://anaconda.org/neutrinomuon/pyintegralall</a>:

[![badgetanaconda](https://anaconda.org/neutrinomuon/pyintegralall/badges/version.svg)](https://anaconda.org/neutrinomuon/pyintegralall/badges/version.svg)
[![badgetreleasedate](https://anaconda.org/neutrinomuon/pyintegralall/badges/latest_release_date.svg)](https://anaconda.org/neutrinomuon/pyintegralall/badges/latest_release_date.svg)
[![badgetplatforms](https://anaconda.org/neutrinomuon/pyintegralall/badges/platforms.svg)](https://anaconda.org/neutrinomuon/pyintegralall/badges/platforms.svg)
<pre>
<code>
conda install -c neutrinomuon pyintegralall
</code>
</pre>
OBS.: Only linux pre-compilation platform in conda.

You can also clone the repository and install by yourself in your machine:
<pre>
<code>
git clone https://github.com/neutrinomuon/IntegralALL
python setup.py install
</code>
</pre>

The methods are given by Int_Type and may be summarized bellow:

<table>
<tr><td>Int_Type</td><td>Type</td><td>Description</td></tr>
<tr><td>0<td>R</td><td>Right rectangle Integral  </td></tr>
<tr><td>1<td>L</td><td>Left rectangle Integral   </td></tr>
<tr><td>2<td>T</td><td>Trapezoidal rule          </td></tr>
<tr><td>3<td>S</td><td>Simple Integral           </td></tr>
<tr><td>4<td>M</td><td>Median rectangle Integral </td></tr>
<tr><td>5<td>I</td><td>Simpsonregel's rule       </td></tr>
<tr><td>6<td>G</td><td>Gauss-Legendre Quadrature </td></tr>
</table>

The main structure of the directories and files are:

<pre>
<code>
IntegralALL
├── dist
│   └── pyintegralall-0.0.1.tar.gz
├── README.md
├── pyintegralall.egg-info
│   ├── PKG-INFO
│   ├── dependency_links.txt
│   ├── SOURCES.txt
│   ├── top_level.txt
│   └── requires.txt
├── LICENSE.txt
├── setup.py
├── build.bat
├── tutorials
│   ├── Example1 - IntegralALL.ipynb
│   └── .ipynb_checkpoints
│       └── Example1 - IntegralALL-checkpoint.ipynb
├── build.sh
├── src
│   ├── python
│   │   ├── __init__.py
│   │   └── PyIntegralALL.py
│   └── fortran
│       ├── IntegralALL.compile
│       ├── IntegralALL.f90
│       ├── IntegralALL.cpython-39-x86_64-linux-gnu.so
│       ├── DataTypes.f90
│       ├── GaussLegendreQuadrature.cpython-39-x86_64-linux-gnu.so
│       ├── LINinterpol.compile
│       ├── GaussLegendreQuadrature.f90
│       ├── LINinterpol.cpython-39-x86_64-linux-gnu.so
│       ├── LINinterpol.f90
│       └── GaussLegendreQuadrature.compile
├── version.txt
├── meta.yaml
└── build
    ├── lib.linux-x86_64-3.9
    │   └── pyintegralall
    ├── src.linux-x86_64-3.9
    │   ├── pyintegralall
    │   ├── build
    │   └── numpy
    └── temp.linux-x86_64-3.9
        ├── pyintegralall
        ├── __pycache__
        ├── ccompiler_opt_cache_ext.py
        ├── src
        └── build

19 directories, 28 files
</code>
</pre>

<mark>PyIntegralALL.py</mark> is a python wrapper to the library in fortran
called <mark>pyintegralall.flib</mark>. The fortran directory can be compiled
separately for each individual subroutine.
