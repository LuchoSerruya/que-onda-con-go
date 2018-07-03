# specify your main target here:
all: informe.pdf clean

# specify the main file and all the files that you are including
SOURCE=informe.tex references.bib 

%.pdf: %.tex $(SOURCE)
	pdflatex $*
	biber $*
	pdflatex $*
	pdflatex $*

clean:
	rm -f *.bak *~ *.log *.blg *.bbl *.aux *.toc *.cut *.out *.tmp *.tpm *.adx *.adx.hyp *.idx *.ilg *.ind \
	*.and *.glg *.glo *.gls *.wdx *.wnd *.wrd *.wdv *.ldx *.lnd *.rdx *.rnd *.xdv *.fdb *.fdb_latexmk *.fls \
	*.synctex.gz *.run.xml *.bcf

realclean: clean
	rm -f *.dvi *.ps *.pdf *.bcf
