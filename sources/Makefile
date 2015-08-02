LATEX=lualatex

LATEX_OPTS=-interaction=nonstopmode -halt-on-error

all: document

document: az-ules-muveszete.pdf

az-ules-muveszete.pdf: az-ules-muveszete_pages.pdf
	pdfnup az-ules-muveszete_pages.pdf '1,2,3,4,5,6' --paper a4paper --nup 3x1 --landscape --frame false --outfile az-ules-muveszete.pdf

az-ules-muveszete_pages.pdf:
	$(LATEX) $(LATEX_OPTS) az-ules-muveszete_pages.tex

