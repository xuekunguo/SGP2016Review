NAME=OntheFlyCutting

all: $(NAME).pdf

$(NAME).pdf: *.tex Content/* Material/* Makefile
	pdflatex $(NAME)
	open $(NAME).pdf

bib:
	pdflatex $(NAME)
	bibtex $(NAME)
	pdflatex $(NAME)
	pdflatex $(NAME)
	open $(NAME).pdf

clean:
	rm -f $(NAME).pdf $(NAME).ps $(NAME).dvi $(NAME).blg $(NAME).bbl $(NAME).brf $(NAME).lbl $(NAME).aux $(NAME).log *~
