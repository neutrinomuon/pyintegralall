### PyIntegral
####  A Fortran legacy package to easy integrate numerically
email: [antineutrinomuon@gmail.com](mailto:antineutrinomuon@gmail.com), [jean@astro.up.pt](mailto:jean@astro.up.pt)

© Copyright ®

J.G. - Jean Gomes

last stable version: 0.0.12.2

<hr>

![My Skills](https://skillicons.dev/icons?i=python,fortran,c,numpy&theme=light)<br>
[![python3](https://img.shields.io/pypi/pyversions/PyIntegral)](https://img.shields.io/pypi/pyversions/PyIntegral)
[![badgetlicense](https://anaconda.org/neutrinomuon/PyIntegral/badges/license.svg)](https://anaconda.org/neutrinomuon/PyIntegral/badges/license.svg)

<hr>

<div align="center">
<img src='https://github.com/neutrinomuon/PyIntegral/blob/main/figures/Definite_Integral.png?raw=true' width="50%">
</div>

<hr>

#### <b>RESUME</b>

<img src="https://raw.githubusercontent.com/neutrinomuon/PyIntegral/main/figures/PyIntegral.png" width=120>
Integrate arrays, functions numerically using different
methods. Original Fortran 2003+ routines date back to 2003-2004. Read the
<a href='https://github.com/neutrinomuon/PyIntegral/blob/main/LICENSE.txt'>LICENSE.txt</a> file. Definite integrals are mathematical calculations that allow
us to find the area under a curve between two defined points on the x-axis. In
other words, they give us the total accumulated value of a function over an
interval. Definite integrals are used in various fields, such as physics,
engineering, and finance, to solve real-world problems, such as calculating
the total distance travelled by a moving object or the total profit of a
company over a certain period.

There are various techniques for computing definite integrals, including
analytical methods (e.g., antiderivatives) and numerical methods (e.g., using
quadrature or Monte Carlo). The choice of method depends on the type of
function being integrated, the desired accuracy, and the computational
resources available. Some commonly used numerical integration techniques
include the trapezoidal rule, Simpson's rule, and Gaussian quadrature.

In computer programming, definite integrals can be calculated using
specialized libraries and routines that provide numerical integration
algorithms. These routines typically take as input the function to be
integrated, the interval over which to integrate, and the desired level of
accuracy. The output of the routine is an approximation of the definite
integral.

Now, PyIntegral has all its scripts in accordance with PEP 8 guidelines.

--------------------------------------------------------------------<br>
Your code has been rated at 10.00/10 (previous run: 10.00/10, +0.00)<br>

<hr>

#### <b>INSTALLATION</b>

You can easily install <a href=https://pypi.org/project/PyIntegral/>PyIntegral</a> by using pip - <a href='https://pypi.org/'>PyPI - The Python Package Index</a>:
<pre>
<code>
pip install PyIntegral
</code>
</pre>
or by using a generated conda repository <a href='https://anaconda.org/neutrinomuon/PyIntegral'>https://anaconda.org/neutrinomuon/PyIntegral</a>:

[![badgetanaconda](https://anaconda.org/neutrinomuon/PyIntegral/badges/version.svg)](https://anaconda.org/neutrinomuon/PyIntegral/badges/version.svg)
[![badgetreleasedate](https://anaconda.org/neutrinomuon/PyIntegral/badges/latest_release_date.svg)](https://anaconda.org/neutrinomuon/PyIntegral/badges/latest_release_date.svg)
[![badgetplatforms](https://anaconda.org/neutrinomuon/PyIntegral/badges/platforms.svg
)](https://anaconda.org/neutrinomuon/PyIntegral/badges/platforms.svg)
<pre>
<code>
conda install -c neutrinomuon PyIntegral
</code>
</pre>
OBS.: Linux, OS-X ad Windows pre-compilations available in conda.

You can also clone the repository and install by yourself in your machine:
<pre>
<code>
git clone https://github.com/neutrinomuon/PyIntegral
python setup.py install
</code>
</pre>

<hr>

#### <b>METHODS</b>

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

<div align="center">
<img src='https://github.com/neutrinomuon/PyIntegral/blob/main/figures/Example_Integration.png?raw=true' width="50%">
</div>

</table>


<hr>

#### <b>REFERENCES</b>

<ol><il> William H. Press, Saul A. Teukolsky, William T. Vetterling, and Brian
P. Flannery. Numerical Recipes: The Art of Scientific Computing. William ISBN:
978-0521880688. Link: <a
href='https://www.nr.com/'>https://www.nr.com/</a></il> </ol>

<hr>

#### <b>STRUCTURE</b>

The main structure of the directories and files are:

<pre>
<code>
PyIntegral
├── PyIntegral
├── dist
│   └── PyIntegral-0.0.10.tar.gz
├── README.md
├── showdown.min.js
├── scripts
│   └── update_readme.py
├── index.html
├── LICENSE.txt
├── setup.py
├── PyIntegral.egg-info
│   ├── PKG-INFO
│   ├── dependency_links.txt
│   ├── SOURCES.txt
│   ├── top_level.txt
│   └── requires.txt
├── tutorials
│   ├── Definite_Integral.png
│   ├── Definite_Integral.py
│   ├── .ipynb_checkpoints
│   │   ├── Example1 - pyintegralall-checkpoint.ipynb
│   │   └── Example1 - IntegralALL-checkpoint.ipynb
│   └── Example1 - pyintegralall.ipynb
├── src
│   ├── python
│   │   ├── __init__.py
│   │   └── PyIntegralALL.py
│   └── fortran
│       ├── LINinterpol.cpython-39-darwin.so
│       ├── GaussLegendreQuadrature.cpython-311-darwin.so
│       ├── IntegralALL.compile
│       ├── IntegralALL.f90
│       ├── IntegralALL.cpython-39-darwin.so
│       ├── IntegralALL.cpython-39-x86_64-linux-gnu.so
│       ├── IntegralALL.cpython-310-darwin.so
│       ├── IntegralALL.cpython-310-x86_64-linux-gnu.so
│       ├── GaussLegendreQuadrature.cpython-38-x86_64-linux-gnu.so
│       ├── IntegralALL.cpython-311-darwin.so
│       ├── DataTypes.f90
│       ├── GaussLegendreQuadrature.cpython-39-x86_64-linux-gnu.so
│       ├── GaussLegendreQuadrature.cpython-310-darwin.so
│       ├── LINinterpol.cpython-311-darwin.so
│       ├── IntegralALL.cpython-38-x86_64-linux-gnu.so
│       ├── LINinterpol.cpython-38-x86_64-linux-gnu.so
│       ├── GaussLegendreQuadrature.cpython-310-x86_64-linux-gnu.so
│       ├── LINinterpol.cpython-310-darwin.so
│       ├── LINinterpol.compile
│       ├── GaussLegendreQuadrature.f90
│       ├── README.txt
│       ├── LINinterpol.cpython-39-x86_64-linux-gnu.so
│       ├── GaussLegendreQuadrature.cpython-39-darwin.so
│       ├── LINinterpol.cpython-310-x86_64-linux-gnu.so
│       ├── LINinterpol.f90
│       └── GaussLegendreQuadrature.compile
├── version.txt
└── build
    └── src.linux-x86_64-3.9
        ├── pyintegralall
        ├── PyIntegral
        └── build

14 directories, 46 files
</code>
</pre>

PyIntegral.py is a python wrapper to the library in Fortran called
pyintegral.flib. The Fortran directory can be compiled separately for each
individual subroutine.

<hr>

#### <b>LICENSE</b>

This software is provided "AS IS" (see DISCLAIMER below). Permission to use,
for non-commercial purposes is granted. Permission to modify for personal or
internal use is granted, provided this copyright and disclaimer are included
in ALL copies of the software. All other rights are reserved. In particular,
redistribution of the code is not allowed without explicit permission by the
author.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
