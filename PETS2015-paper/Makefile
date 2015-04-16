all: tor-censorship-usability.pdf

tor-censorship-usability.pdf: tor-censorship-usability.tex bibliography.bib

%.pdf: %.tex
	pdflatex "$*"
	pdflatex "$*"
	bibtex "$*"
	pdflatex "$*"
	pdflatex "$*"

clean:
	rm -f tor-censorship-usability.pdf

.PHONY: all clean
