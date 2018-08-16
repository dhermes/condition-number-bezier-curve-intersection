# A Condition Number for B&#xe9;zier Curve Intersection

This originally appeared in my [thesis][1] and is now being split out
into a (short) standalone paper.

This repository is laid out in a manner described in
[Good Enough Practices in Scientific Computing][2].

## Abstract

We present a short note describing a condition number
of the intersection of two B&#xe9;zier curves. Since tangent
intersections are to transversal intersections as multiple roots are
to simple roots of a function, this condition number is infinite
for non-transveral intersections.

## Installation

The code used to build the manuscript, generate images and verify
computations is written in Python. To run the code, Python 3.7
should be installed, along with ``nox-automation``:

```
python -m pip install --upgrade nox-automation
```

Once installed, the various build jobs can be listed. For example:

```
$ nox --list-sessions
Available sessions:
* build_tex
```

To run ``nox -s build_tex`` (i.e. to build the PDF), ``pdflatex`` and
``bibtex`` are required.

[1]: https://github.com/dhermes/phd-thesis
[2]: https://arxiv.org/abs/1609.00037
