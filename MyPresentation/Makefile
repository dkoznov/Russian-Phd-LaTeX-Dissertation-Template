all:
	xelatex -shell-escape "\def\ishandout{1} \input{presentation.tex}"
full:
	xelatex -shell-escape "\def\ishandout{1} \input{presentation.tex}"
	bibtex -min-crossrefs=10 presentation
	xelatex -shell-escape "\def\ishandout{1} \input{presentation.tex}"
	xelatex -shell-escape "\def\ishandout{1} \input{presentation.tex}"
pause:
	xelatex -shell-escape presentation.tex
	bibtex -min-crossrefs=10 presentation
	xelatex -shell-escape presentation.tex
	xelatex -shell-escape presentation.tex
clean:
	rm  presentation*.{aux,log,nav,out,snm,toc,pdf}
