SHELL = /bin/sh
PDFLATEX = pdflatex

MAIN = table
TEXFILES = $(MAIN).tex

.PHONY: all pdf clean allclean

all: pdf

pdf: $(TEXFILES)
	$(PDFLATEX) $(MAIN)
	$(PDFLATEX) $(MAIN)

clean:
	rm -f *.log *.aux *.out *.toc

allclean: clean
	rm -f $(MAIN).pdf
