PDFS = chapter01.pdf chapter02.pdf chapter03.pdf chapter04.pdf chapter05.pdf chapter06.pdf chapter07.pdf chapter10.pdf chapter11.pdf chapter12.pdf chapter16.pdf

all: $(PDFS)

clean:
	rm -f *.log *.aux *.vrb *.toc
	

%.pdf : %.Rnw
	knitr $< 
	pdflatex $*
	pdflatex $*

