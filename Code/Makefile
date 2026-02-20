TEX := State_of_the_Art.tex
PDF := State_of_the_Art.pdf
PNG_BASE := State_of_the_Art
DPI ?= 1200

.PHONY: all pdf png clean

all: pdf png

pdf:
	latexmk -pdf -interaction=nonstopmode -halt-on-error $(TEX)

png: pdf
	pdftocairo -png -r $(DPI) $(PDF) $(PNG_BASE)

eps: pdf
	pdftops -eps $(PDF) $(PNG_BASE).eps

clean:
	latexmk -C $(TEX)
	rm -f $(PNG_BASE)-*.png
	rm -f $(PNG_BASE).eps
