SHELL = /bin/sh
PDFLATEX = pdflatex

TARGETS = java c python

.PHONY: all clean allclean $(TARGETS)

all: $(TARGETS)

$(TARGETS):
	$(PDFLATEX) $@
	$(PDFLATEX) $@

clean:
	rm -f *.log *.aux *.out *.toc

allclean: clean
	rm -f $(addsuffix .pdf, $(TARGETS))
