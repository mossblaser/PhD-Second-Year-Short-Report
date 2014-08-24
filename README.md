End of Year Report
==================

This is the LaTeX source for my 'long' end-of-year report for the second year of
my PhD.  The report is aimed at 'general' computer scientists and aims to give
some context for the work I'm doing and suggest where things may end up going.

This document is a work in progress. You have been warned.

Build
-----

This expects my bibtex database to be copied/symlinked to report.bib.

	mkdir -p tikzcache
	pdflatex -shell-escape report.tex
	bibtex report
	pdflatex -shell-escape report.tex
	pdflatex -shell-escape report.tex

The following (possibly less-standard) LaTeX libraries are required:

* TikZ
