
# generate pdf

pdflatex *.tex
bibtex *.aux
pdflatex *.tex
pdflatex *.tex

# delete temp files after the generating work done
del *.blg *.bbl *.aux *.log *.brf *.nlo *.out *.dvi *.ps *.lof *.toc *.fls *.fdb_latexmk *.pdfsync *.synctex*.gz *.ind *.ilg *.idx
