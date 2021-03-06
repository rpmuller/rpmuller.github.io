Projects
========
* [PyQuante](http://pyquante.sf.net)/[PyQuante2](https://github.com/rpmuller/pyquante2)
* [Matplotlib/sympy quantum circuit plotting](https://github.com/rpmuller/PlotQCircuit/blob/master/PlotQCircuit.ipynb)

IPython Notebooks
=================
* [Crash Course in Python for Scientists](http://nbviewer.ipython.org/5920182)
* [PyQuante2 Overview](http://nbviewer.ipython.org/5745404)
* [Sympy Quantum Circuit Plotting](http://nbviewer.ipython.org/5843312)
* [Matplotlib Quantum Circuit Plotting](https://github.com/rpmuller/PlotQCircuit/blob/master/PlotQCircuit.ipynb)
* [SVG graphics in IPython notebooks](http://nbviewer.ipython.org/5666810)

Progress
========
* 23 Mar 2019
  - Wow, has it really been almost 2 years? I switched to a management job. Fixed some bugs involved in making sure the cython routines work with py 3.7. Had to rebuild the bindings. Also pushing a mac version of pyquante2-2.0-py3.7 to the conda.org cloud.
* 27 Jun 2017
  - GVB works for H2.
* 2 Jun 2017
  - There is a new module [scf/mcscf](https://github.com/rpmuller/pyquante2/blob/master/pyquante2/scf/mcscf.py) that contains GVB. GVB itself doesn't work (yet), but the general ROHF does using ROTION/OCBSE.
  - A good reference for these methods is [Bobrowicz and Goddard, 1977](http://www.wag.caltech.edu/publications/sup/pdf/108.pdf)
* 5 May 2017
  - The [Matplotlib Quantum Circuit Plotting](https://github.com/rpmuller/PlotQCircuit/blob/master/PlotQCircuit.ipynb) notebook has a very lightweight toolset for plotting quantum circuits with Python/Matplotlib that also works with Jupyter notebooks.
* 20 Apr 2017
  - Avogadro for linux is now out on [my anaconda channel](http://anaconda.org/rpmuller).
  - Also openmpi-2.1.0
* 17 Apr 2017
  - The pure python branch of pyquante2 is now called "pure".
  - There are pyquante2_pure conda builds for all platforms on https://anaconda.org/rpmuller/pyquante2_pure.
  - There are compiled pyquante2 conda builds for linux/mac on https://anaconda.org/rpmuller/pyquante2
  - Conda rocks! 
* 12 Apr 2017
  - There is a pyquante2.0_pure branch that is pure python, for those without a compiler.
* 3 Mar 2017
  - Updating documentation for the sympy quantum circuit tools
  - Has it really been 2 years?!
* 3 Apr 2015
  - ROHF works in pyquante2
* 30 Mar 2015
  - LDA works in pyquante2
* 22 Mar 2015
  - MayaVi display of DFT density and molecules added to pyquante2
* 21 Jun 2014
  - Very trivial PyQuante function now works in Julia
* 10 Apr 2014
  - Added a preliminary zmatrix utility to pyquante2
* 14 Aug 2013
  - Qasm parser was merged into sympy master
* 13 Aug 2013
  - Fixing end-of-line whitespace
* 11 Aug 2013
  - More tests for qasm parser
* 9 Aug 2013
  - Added tests for Qasm parser
* 8 Aug 2013
  - Got the labelled/initialized gates to work.
  - Initiated pull request for the Qasm parser.
* 7 Aug 2013
  - Tried to handle QASM commands like "qubit q0,0", failed
* 6 Aug 2013
  - Added a two-electron Hylleraas code to pyquante2/hylleraas/helios.py
* 5 Aug 2013
  - Working on a better division between the scf iterators and Hamiltonians. Want to be able to mix and match more,
    so that I can combine any iterator with any Hamiltonian. Probably not possible, but any movement in this
    direction would be good.
* 4 Aug 2013
  - The pyquante2 test suite now runs under python 2.7 and python 3.3!
* 3 Aug 2013
  - Updated to py3 style print statements in qasm module.
* 2 Aug 2013
  - Rebased Sympy qasm_parser branch against master.
* 1 Aug 2013
  - Qasm now properly parses quoted gate symbols in def statements.
  - Qasm now also parses controlled gate def statements.
  - [Sympy Quantum Circuit Plotting](http://nbviewer.ipython.org/5843312) updated.
* 31 Jul 2013
  - Very simple def statements work in sympy qcircuit qasm parser.
  - All pyquante2 classes are now "new style".
* 30 Jul 2013
  - Working on DFT iterators in pyquante2.
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

[Older Progress](https://github.com/rpmuller/rpmuller.github.io/blob/master/Older.md)

Links
=====
* [My Sandia Homepage](http://www.cs.sandia.gov/~rmuller).
* [Citations on Google Scholar](http://scholar.google.com/citations?user=ihGf4wgAAAAJ&hl=en).

