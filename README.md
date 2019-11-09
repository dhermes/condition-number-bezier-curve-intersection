# A Condition Number for B&#xe9;zier Curve Intersection

| Cite paper           |
| -------------------- |
| [![Paper DOI][8]][6] |

This originally appeared in my [thesis][1] and is now split out
into a (short) standalone [paper][3].

This repository is laid out in a manner described in
[Good Enough Practices in Scientific Computing][2].

The content itself has been uploaded to the [arXiv][4] and was submitted to
the journal [CAGD][5] in April 2019. The paper has been accepted and was
[published][6] [on][7] November 8, 2019.

## Abstract

We present a condition number of the intersection of two B&#xe9;zier curves.

## Citation

To cite this paper:

```
@article{Hermes2019,
  doi = {10.1016/j.cagd.2019.101791},
  url = {https://doi.org/10.1016/j.cagd.2019.101791},
  year = {2019},
  month = {Nov},
  publisher = {Elsevier {BV}},
  volume = {75},
  pages = {101791},
  author = {Danny Hermes},
  title = {A 2-norm condition number for B{\'{e}}zier curve intersection},
  journal = {Computer Aided Geometric Design}
}
```

## Installation

The code used to build the manuscript, generate images and verify
computations is written in Python. To run the code, Python 3.7
should be installed, along with `nox`:

```
python -m pip install --upgrade 'nox >= 2019.8.20' 'py >= 1.6.0'
```

Once installed, the various build jobs can be listed. For example:

```
$ nox --list-sessions
Sessions defined in .../condition-number-bezier-curve-intersection/noxfile.py:

* build_tex

sessions marked with * are selected, sessions marked with - are skipped.
```

To run `nox -s build_tex` (i.e. to build the PDF), `pdflatex` and
`bibtex` are required.

[1]: https://github.com/dhermes/phd-thesis
[2]: https://arxiv.org/abs/1609.00037
[3]: doc/paper.pdf
[4]: https://arxiv.org/abs/1808.06126
[5]: https://www.journals.elsevier.com/computer-aided-geometric-design
[6]: https://doi.org/10.1016/j.cagd.2019.101791
[7]: doc/1-s2.0-S0167839619301001-main.pdf
[8]: https://img.shields.io/badge/DOI-10.1016%2Fj.cagd.2019.101791-blue.svg
