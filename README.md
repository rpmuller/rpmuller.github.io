Projects
========
* [PyQuante](http://pyquante.sf.net)/[PyQuante2](https://github.com/rpmuller/pyquante2)
* [Sympy for Quantum Circuits](https://github.com/rpmuller/sympy/tree/sympy_qcircuit/sympy/physics/quantum)
* Python bindings for Libxc
* Python bindings for Libint
* Python2.7 bindings for Libquantum

IPython Notebooks
=================
* [Crash Course in Python for Scientists](http://nbviewer.ipython.org/5920182)
* Learning Quantum Chemistry with PyQuante: Coming Soon!
* Tensor Operations in Numpy: Using tensordot and einsum: Coming Soon!
* [PyQuante2 Overview](http://nbviewer.ipython.org/5745404)
* [Sympy Quantum Circuit Plotting](http://nbviewer.ipython.org/5843312)
* [SVG graphics in IPython notebooks](http://nbviewer.ipython.org/5666810)

Progress
========
* 29 Jul 2013
  - Further development of the class-based Qasm parser.  
    [Sympy Quantum Circuit Plotting](http://nbviewer.ipython.org/5843312) has an example 
    of use of this.
* 28 Jul 2013
  - Simplified the QASM parser and started to think about how to implement the def command.
* 27 Jul 2013
  - [Sympy Quantum Circuit Plotting](http://nbviewer.ipython.org/5843312) updated to include qasm parsing examples.
* 26 Jul 2013
  - Faux measurements merged.
* 25 Jul 2013
  - Again trying to merge the faux measurements into Sympy.
* 24 Jul 2013
  - Trying to get the sympy qasm parser to deal with 'def' statements.
* 23 Jul 2013
  - Still working on VWN. Moved test code into an ipython notebook and also compared to the PW Correlation
* 19 Jul 2013
  - Trying to debug VWN. Not having much luck.
* 18 Jul 2013
  - Created a new sympy branch off of master to handle qasm parsing.
* 17 Jul 2013
  - Trying to support SVWN, PBE, BLYP functionals. Tests for all exchange functionals work. Tests for all correlation functionals fail. :-(
* 16 Jul 2013
  - [Pull request submitted](https://github.com/sympy/sympy/pull/2294) for second set of changes to sympy
    circuit plotting.
  - pyquante2 xpbe tests pass.
* 15 Jul 2013
  - qcircuit_measurement branch created to hack measurements into 
    circuit plotting.
  - Initial set of hacks done: horizontal wires now doubled.
* 14 Jul 2013
  - First set of qcircuit hacks merged into master!
  - Outlined thoughts on [implementing measurement](https://github.com/rpmuller/rpmuller.github.io/blob/master/MeasurementThoughts.md) in sympy circuitplot.
* 13 Jul 2013
  - Trying to get Travis to accept my sympy changes for quantum circuits.
    Travis [appears to be working now](https://travis-ci.org/sympy/sympy/builds/9038252).
  - Travis now also regularly builds/tests pyquante2
  - pyquante2 test suite now runs without matplotlib or pyglet installed.
  - You can now do this Steane check with only 7 lines of code:
  - ![steane check](https://raw.github.com/rpmuller/rpmuller.github.io/master/steane.png)

[Older Progress](https://github.com/rpmuller/rpmuller.github.io/blob/master/Older.md)

Links
=====
* [My Sandia Homepage](http://www.cs.sandia.gov/~rmuller).
* [Citations on Google Scholar](http://scholar.google.com/citations?user=ihGf4wgAAAAJ&hl=en).

