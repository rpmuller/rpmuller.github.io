Thoughts on implementing measurements in the sympy CircuitPlot
==============================================================
*Rick Muller*

Now that the [pull request containing the initial circuitplot
hacks](https://github.com/sympy/sympy/pull/2270) has been merged, I'd
like to start thinking about how to implement the classical lines in a
quantum circuit plot, which are typically rendered as double lines,
and that you can see here

![measured circuit](http://www.media.mit.edu/quanta/qasm2circ/test2.png).

One thing that I like about the current way sympy/physics/quantum
works is that the quantum circuits are acutal quantum state
simulators. I.e., you can apply them to a quantum state and they give
the right result.

There is no doubt a correct way to deal with quantum measurement in a
similar way, but I certainly haven't figured it out yet. In the
meantime, I would like to be able to output circuit plots that have
proper classical measurements.

The point, though, is that I want to do as much of this work as
possible in circuitplot.py, rather than in gate.py, because I don't
want to suggest that these are actual *measurements* (in the sense
that XGate() gives an object that implements a Pauli X
operator). These are just things that *look like* a quantum
measurement. 

CircuitPlot calls two steps, _plot_wires() and _plot_gates(), when it
renders a circuit. I want to create some additional data before it
calls either of these steps. The data will look someting like
_gate_grid() and _wire_grid() do, it will look at the circuit as an xy
array, and determine at which point in time (which _gate_grid()
measures) each wire (tracked by _wire_grid()) is measured.

We will define faux measurement operators, which will just be single
qubit gates, with labels like "M_x" or "M_z", and some property that
flags them as measurements. When the scanner sees one of these faux
operators, it will flip the switch on the corresponding wire to
"measured".

Initially, I'm just going to draw a second line when _plot_wire() is
called, slightly above the first. I also need to scan all of the gates
that use the classical line as a control, which should also be
doubled. Later we can figure out how to prettify this by drawing two
centered lines in each direction rather than a centered line and a
second one next to it.

Initially, I'll just use "M_x", and "M_z" as the measurement gates,
and we can later figure out how to do the little dials that the
qcircuit people like, or those "D" looking lines (e.g. [example 15
here](http://www.media.mit.edu/quanta/qasm2circ/)). I'm planning to
skip the purely classical lines, a la [example 10
here](http://www.media.mit.edu/quanta/qasm2circ/), because I have yet
to ever see one of these used.

I'm also planning to implement vertically stacked gates in this
revision, but I'll detail that separately.
