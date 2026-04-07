# Neural Network Textbook Makefile

TEX = xelatex
BIB = biber
MAIN = main

.PHONY: all clean pdf

all: pdf

pdf: $(MAIN).pdf

$(MAIN).pdf: $(MAIN).tex
	$(TEX) $(MAIN)
	$(BIB) $(MAIN)
	$(TEX) $(MAIN)
	$(TEX) $(MAIN)

clean:
	rm -f *.aux *.bbl *.blg *.log *.out *.toc *.lof *.lot *.synctex.gz *.fls *.fdb_latexmk

cleanall: clean
	rm -f $(MAIN).pdf
