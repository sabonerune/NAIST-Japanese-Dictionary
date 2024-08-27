#TARGET=NAIST-jdic-ja
docdir = $(pkgdatadir)/doc
TEX =  NAIST-jdic-ja.tex
PDF =  NAIST-jdic-ja.pdf 
EXTRA_DIST = $(TEX) $(PDF)
SUFFIXES= .tex .dvi .pdf

all: $(PDF)

.tex.dvi:
	platex $<
	platex $<

.dvi.pdf:
	dvipdfmx $<

clean: 
	rm -f NAIST-jdic-ja.pdf NAIST-jdic-ja.dvi