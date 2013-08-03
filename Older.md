Older Progress
==============
## July 2013
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



## June 2013
* 30 Jun 2013
  - Added an example of Surface Code X and Z checks to the 
    [Sympy Circuit
    Notebook](http://nbviewer.ipython.org/5843312). It's amazing how
    much less time 
    this takes than using QCircuit. Need to add some additional extra
    features today.
  - ![Z check](https://raw.github.com/rpmuller/rpmuller.github.io/master/zcheck.png)
  - Trying to get a single basis function eval call to evaluate a
  whole mesh of points in pyquante2. Had to ask [this question to Stackoverflow](http://stackoverflow.com/questions/17391052/compute-square-distances-from-numpy-array)
    along the way.
  - Added the mesh command, which evaluates a basis function on a mesh
    of points. 
  - Also improved the generation of lines in 3d in lineplot.
* 29 Jun 2013
  - Updated [Sympy Circuit Notebook](http://nbviewer.ipython.org/5843312) 
    and got a few more examples to work. 
  - Reviewed priorities.
  - Fixed the mixed cgbf/pbgf bug for the 1e code. Still exists for 2e
    code. 
* 28 Jun 2013
  - Removed old iterators: no more simple, usimple, averaging
* 27 Jun 2013
  - Killed the stuff I did with RuntimeErrors in the iterators, and
    wrote a non-generator-based SCFIterator that properly exits, and
    can keep track of whether or not it is converged. Haven't wired
    this in to much of the code yet.    
  - Making a little progress updating the pyqu bindings for Py27
* 26 Jun 2013
  - Added RuntimeErrors to PyQuante2 iterators when maxiters
    reached. Am not doing anything to catch these at this point, but
    could do so later on. 
* 25 Jun 2013
  - Poor man's scratcher: find . -size +100M -mtime +28 (yes, I need
    to clean my scratch directories). 
    Can also use with -exec rm {} \;
  - Had trouble getting the nosetests to run quickly in
    pyquante2. Worked around this by doing a  
    setup.py build_ext --inplace to get the cython libraries in the
    appropriate places, after which 
    the nosetest went from taking 74 sec to run to taking < 2 sec!
  - Also moved test_cython into the tests directory, since now nose can run these tests.
* 24 Jun 2013
  - Profiling of unit tests in PyQuante2: Weird results. Looks as if the python 
    versions of the integral routines are being called when running
    tests through nose, but the cython version are called when running
    from the command line.
  - Spent a little bit of time doing some more with the sympy circuit
    plotter. Updated the notebook. Can now do arbitrarily labelled 1Q
    gates, as well as controlled versions of these. Block multi-Q 
    gates don't work, nor do gates with matrices as their labels.
* 23 Jun 2013
  - libquantum wrappers: Extending python with C is very
    frustrating. Can't seem to get anything but segfaults!  
    Cython makes things much nicer, but I'm having trouble getting it
    to recognize _Complex 
  - When MacPorts won't download files for you, you can manually
    download them and stick them in [Macports root]/var/macports/distfiles. 
    But why does MacPorts fail to fetch
    so often?  EDIT: proxy problems, of course.
  - Sticking this here since I forget it so often. To change the
    default (python or whatever) version in macports, do 

    port select --list python

* 22 Jun 2013
  - Fixed pyquante2 orbital symmetry bug, which wasn't a bug but arose
    from my missing a transpose. 
  - Prettified the pyquante2 plotting routines, and added to IPython notebook.
  - Got proper X, CNOT, and CPHASE gates to work in Sympy
  - ![vtk orbital plotting](https://raw.github.com/rpmuller/rpmuller.github.io/master/h2-antibonding-pyquante2.png)
