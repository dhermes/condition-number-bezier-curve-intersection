# A Condition Number for B&#xe9;zier Curve Intersection

This originally appeared in my [thesis][1] and is now split out
into a (short) standalone [paper][3].

This repository is laid out in a manner described in
[Good Enough Practices in Scientific Computing][2].

The content itself has been uploaded to the [arXiv][4] and was submitted to
the journal [CAGD][5] in April 2019. The submission received reviewer comments
in June 2019 and a second revision was submitted to the journal. A second
round of reviewer comments were received in October 2019 and a third revision
has been submitted as well.

## Abstract

We present a condition number
of the intersection of two B&#xe9;zier curves. Since tangent
intersections are to transversal intersections as multiple roots are
to simple roots of a function, this condition number is infinite
for non-transveral intersections.

## Installation

The code used to build the manuscript, generate images and verify
computations is written in Python. To run the code, Python 3.7
should be installed, along with `nox`:

```
python -m pip install --upgrade 'nox >= 2018.10.17' 'py >= 1.6.0'
```

Once installed, the various build jobs can be listed. For example:

```
$ nox --list-sessions
Available sessions:
* build_tex
```

To run `nox -s build_tex` (i.e. to build the PDF), `pdflatex` and
`bibtex` are required.

[1]: https://github.com/dhermes/phd-thesis
[2]: https://arxiv.org/abs/1609.00037
[3]: doc/paper.pdf
[4]: https://arxiv.org/abs/1808.06126
[5]: https://www.journals.elsevier.com/computer-aided-geometric-design
