# Secure code synthesis

## Abstract

TODO

### Building document locally

A `Makefile` is provided for building the document locally. This requires a LaTeX compiler, such as [`texlive`](https://www.tug.org/texlive/), installed locally, which has to provide the commands `pdflatex` and `biber`.


### FAQ
If sources produces an error, try running 
```
rm -rf `biber --cache`
```
