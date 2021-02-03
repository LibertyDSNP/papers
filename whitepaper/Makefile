PROJECT=dsnp_whitepaper
TEX=pdflatex
LATEXFLAGS+=	-file-line-error -halt-on-error -interaction nonstopmode
BIBTEX=bibtex
BUILDTEX=$(TEX) $(LATEXFLAGS) $(PROJECT).tex

all:	clean
	$(BUILDTEX)
	$(BIBTEX) $(PROJECT)
	$(BUILDTEX)
	$(BUILDTEX)

clean-all: clean
	rm -f *.dvi *.ps *.eps *.pdf *.toc

clean:
	rm -f *.log *.bak *.aux *.bbl *.blg *.idx *.toc *.out *~ *.fls *-blx.bib *.run.xml

