clean:
	rm -r _minted-* *.aux *.log *.idx *.out *.nav *.toc *.vrb *.snm

%.tex: %.mlt
	caml-tex -s igor -p -v '#' -o $@ $<

%.pdf: %.tex
	pdflatex -jobname=$* -shell-escape '\newif\ifsoln\input{$*}'
	pdflatex -jobname=$* -shell-escape '\newif\ifsoln\input{$*}'

%_soln.pdf: %.tex
	pdflatex -jobname=$*_soln -shell-escape '\newif\ifsoln \solntrue\input{$*}'
	pdflatex -jobname=$*_soln -shell-escape '\newif\ifsoln \solntrue\input{$*}'


