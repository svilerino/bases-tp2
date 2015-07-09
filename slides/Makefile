.PHONY: all
LATEX=pdflatex
ARCHIVOS=slides.tex
all: slides.pdf	

slides.pdf: $(ARCHIVOS)
	reset
	@echo "Compiling informe in latex..."
#se hace 2 veces el latex para que cargue bien la TOC y redirije todo a loginforme para no imprimir 23098230982309823 lineas en el makefile.
	$(LATEX) slides.tex
	$(LATEX) slides.tex
	#okular slides.pdf
	evince slides.pdf &
clean: 
	@echo "Cleaning informe"	
	- rm -f *.loginforme
	- rm -f *.log
	- rm -f *.toc
	- rm -f *.aux
	- rm -f *.out
	- rm -f *.pdf
	- rm -f *.dvi
	- rm -f *.snm
	- rm -f *.nav
	- rm -f *~
