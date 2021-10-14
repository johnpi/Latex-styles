# Latex-styles
Useful Latex style files

unsrtcurrentbiology.bst : Bibliography style file for the journal Current Biology. 

USAGE: 
1. Copy it in the directory with the .tex files. 
2. In the .tex file use 
```
\usepackage[super,numbers,sort&compress]{natbib}
\bibliographystyle{unsrtcurrentbiology}
```
3. Cite using \cite{}

unsrtcurrentbiology_abbrv.bst : Bibliography style file for the journal Current Biology with modifications for abbreviating journal names.

USAGE: 
1. Copy it in the directory with the .tex files. 
2. In the .tex file use 
```
\usepackage[super,numbers,sort&compress]{natbib}
\bibliographystyle{unsrtcurrentbiology_abbrv}
```
3. Cite using \cite{}

To change the bibliography listing from [1], [2], ... to 1., 2., ... add this to the preample 
```
\makeatletter % changes the catcode of @ to 11
\renewcommand\@biblabel[1]{#1.}
\makeatother % changes the catcode of @ back to 12
```
