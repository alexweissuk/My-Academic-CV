# My-Academic-CV

This repository contains my academic CV, which was made using LaTex
and BibLaTeX, the latter because it makes splitting up papers,
chapters, etc. into separate sections very easy.

The files relating to my CV include a cv.pdf, cv.tex, and pure.bib.

This repository also includes the files apa-cv.bbx, apa-cv.cbx, and
apa-cv.dbx. These files consistute a slightly modified version of the
APA referencing class written by Philip Kime.

I made a slight modification to apa.cbx so that the references would
not include a letter after the year when there were multiple instances
of my work in the same year. The altered code are found in lines
21-23.

To get this to work, I moved the apa-cv.* files into the directory
that contains Philip Kime's apa.* files, which on my system is:

/usr/share/texlive/texmf-dist/tex/latex/biblatex-apa/

After updating texhash, I execute the following commands:

pdflatex cv
biber cv
pdflatex cv
pdflatex cv