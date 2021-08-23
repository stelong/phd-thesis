thesis: bibliography.bib publications.bib thesis.tex classicthesis-config.tex chapters/*.tex frontback/*.tex
	pdflatex -shell-escape thesis
	bibtex thesis
	bibtex thesis1-blx
	bibtex thesis
	pdflatex -shell-escape thesis
	pdflatex -shell-escape thesis

partial:
	bibtex thesis
	pdflatex -shell-escape thesis

clean:
	rm -f *.aux chapters/*.aux frontback/*.aux *.bbl *.blg *-blx.* *.lof *.log *.lol *.lot *.out *.toc *.xml thesis.pdf

rebuild: clean thesis