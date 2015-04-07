all: paper.pdf

paper.pdf: paper.tex tex-inputs/*.tex bibliography.bib

%.pdf: %.tex
	pdflatex "$*"
	pdflatex "$*"
	bibtex "$*"
	pdflatex "$*"
	pdflatex "$*"

clean:
	rm -f paper.pdf

.PHONY: all clean