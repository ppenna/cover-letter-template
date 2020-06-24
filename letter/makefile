#
# Copyright(C) Pedro Henrique Penna <pedrohenriquepenna@gmail.com>
#
# All rights reserved.
#

LATEX = latexmk
LATEX_FLAGS = -shell-escape -e "\$$pdflatex=q/pdflatex -synctex=1 -interaction=nonstopmode/" -pdf

all: main.tex
	pdflatex -interaction=nonstopmode main.tex ; \
	bibtex main; \
	pdflatex -interaction=nonstopmode main.tex ;\
	pdflatex -interaction=nonstopmode main.tex

clean:
	rm -f *.aux *.bbl *.bcf *.blg
	rm -f *.fls *.log *.out *.xml
	rm -f *.toc *.fdb_latexmk *.gz
	rm -f *.glo *.ist *.acn
	rm -f *-blx.bib *.snm *.nav
