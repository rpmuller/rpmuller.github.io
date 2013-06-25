Github Projects
===============
* [PyQuante](http://pyquante.sf.net)/[PyQuante2](https://github.com/rpmuller/pyquante2)
* [Sympy for Quantum Circuits](https://github.com/rpmuller/sympy/tree/sympy_qcircuit/sympy/physics/quantum)
* Python bindings for Libxc
* Python bindings for Libint
* Python2.7 bindings for Libquantum

IPython Notebooks
=================
* Crash Course in Python for Scientists: Coming Soon!
* [PyQuante2 Overview](http://nbviewer.ipython.org/5745404)
* [Sympy Quantum Circuit Plotting](http://nbviewer.ipython.org/5843312)
* [SVG graphics in IPython notebooks](http://nbviewer.ipython.org/5666810)

Progress
========
* 24 Jun 2013
  - Profiling of unit tests in PyQuante2: Weird results. Looks as if the python versions of the integral routines
    are being called when running tests through nose, but the cython version are called when running from the
    command line.
  - Spent a little bit of time doing some more with the sympy circuit plotter. Updated the notebook. 
    Can now do arbitrarily labelled 1Q gates, as well as controlled versions of these. Block multi-Q
    gates don't work, nor do gates with matrices as their labels.
* 23 Jun 2013
  - libquantum wrappers: Extending python with C is very frustrating. Can't seem to get anything but segfaults! 
    Cython makes things much nicer, but I'm having trouble getting it to recognize _Complex
  - When MacPorts won't download files for you, you can manually download them and stick them in 
    [Macports root]/var/macports/distfiles. But why does MacPorts fail to fetch so often? 
    EDIT: proxy problems, of course.
  - Sticking this here since I forget it so often. To change the default (python or whatever) version in macports, do

    port select --list python

* 22 Jun 2013
  - Fixed pyquante2 orbital symmetry bug, which wasn't a bug but arose from my missing a transpose.
  - Prettified the pyquante2 plotting routines, and added to IPython notebook.
  - Got proper X, CNOT, and CPHASE gates to work in Sympy

Links
=====
* [My Sandia Homepage](http://www.cs.sandia.gov/~rmuller).

