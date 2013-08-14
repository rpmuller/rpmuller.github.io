Projects
========
* [PyQuante](http://pyquante.sf.net)/[PyQuante2](https://github.com/rpmuller/pyquante2)
* [Sympy for Quantum Circuits](https://github.com/rpmuller/sympy/tree/sympy_qcircuit/sympy/physics/quantum)

IPython Notebooks
=================
* [Crash Course in Python for Scientists](http://nbviewer.ipython.org/5920182)
* [PyQuante2 Overview](http://nbviewer.ipython.org/5745404)
* [Sympy Quantum Circuit Plotting](http://nbviewer.ipython.org/5843312)
* [SVG graphics in IPython notebooks](http://nbviewer.ipython.org/5666810)
* Learning Quantum Chemistry with PyQuante: Coming Soon!
* Tensor Operations in Numpy: Using tensordot and einsum: Someday/Maybe

Progress
========
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

