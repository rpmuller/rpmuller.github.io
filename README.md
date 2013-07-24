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
* 12 Jul 2013
  - Added unit tests to sympy circuitplot
  - Attempted to get a array version of the b88 functional working. The failures with this may make me
    give up altogether with array versions of these functionals. I guess I should verify that all the 
    functionals work first, and then worry about making their evaluation faster.
* 11 Jul 2013
  - Further edits and simplifications to the sympy qcircuit branch.
  - [Pull request sent](https://github.com/sympy/sympy/pull/2270) for first 
    batch of sympy qcircuit changes.
  - Tested (and verified) that b88 functional works.
* 10 Jul 2013
  - Testing vwn5 and b88 functionals.
  - Touched the sympy circuit printing just so I wouldn't go too long without working on it.
    Positively stupid wire labelling implemented.
  - Labelled wires now work in sympy.
  - ![Labeled wires](https://github.com/rpmuller/rpmuller.github.io/raw/master/qft-labelled.png)
* 9 Jul 2013
  - Testing lda functionals.
* 8 Jul 2013
  - Minor cleaning and updating.
  - Started to work on DFT functionals and (more importantly) a test suite for DFT functionals
* 7 Jul 2013
  - Debugging radial meshes:
  - ![radial](https://raw.github.com/rpmuller/rpmuller.github.io/master/radial-meshses.png)
* 6 Jul 2013
  - pyquante2 now has a rudimentary pyglet-based viewer
  - Advanced DFT meshes.
  - ![Plotting of DFT Meshes](https://raw.github.com/rpmuller/rpmuller.github.io/master/h2o-mesh.png)
* 5 Jul 2013
  - Simplified arguments to mp2, and moved int transformation to
    integral module. 
* 4 Jul 2013
  - More work on dft grids.
* 3 Jul 2013
  - Work started on dft grids.
  - Release of  [Crash Course in Python for
    Scientists](http://nbviewer.ipython.org/5920182)! 
* 2 Jul 2013
  - Feature to mesh entire basis set not added and tested.
  - Lineplot and Contourplot modules simplified.
  - MP2 now works.
* 1 Jul 2013
  - Einsum: Mind == Blown! Don't have good intuition for either
    np.einsum or np.tensordot, so I've decided  to write a tutorial
    for both, since they contain some nice tensor contractions that
    can seriously  speed a scientific calculation. 
    [Know of any good tutorials for either?](http://www.reddit.com/r/Python/comments/1hf4i6/good_documentation_for_tensordot_and_einsum/)? 
    Let me know, either by posting to the reddit thread or emailing
    rpmuller@gmail.com. 
  - Major speed up to the pyquante2 integral code by using the
    bad-assedness of einsum. 

[Older Progress](https://github.com/rpmuller/rpmuller.github.io/blob/master/Older.md)

Links
=====
* [My Sandia Homepage](http://www.cs.sandia.gov/~rmuller).
* [Citations on Google Scholar](http://scholar.google.com/citations?user=ihGf4wgAAAAJ&hl=en).

