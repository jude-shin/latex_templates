SHELL = /bin/sh
PDFLATEX = pdflatex
BIBER = biber

MAIN = bibliography
TEXFILES = $(MAIN).tex
BIBFILES = references.bib

.PHONY: all bib clean allclean

all: bib

bib: $(TEXFILES) $(BIBFILES)
	$(PDFLATEX) $(MAIN)
	$(BIBER) $(MAIN)
	$(PDFLATEX) $(MAIN)
	$(PDFLATEX) $(MAIN)

clean:
	rm -f *.log *.aux *.out *.bcf *.bbl *.blg *.xml *.toc *.run.xml

allclean: clean
	rm -f $(MAIN).pdf
