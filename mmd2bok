#!/bin/bash
cd latex
cp -rf ../template/* .
cp -rf ../contents/img .
#ls -al img
multimarkdown -t latex meta.txt ../contents/0-preface*.md -o preface.tex
multimarkdown -t latex meta.txt ../contents/1-chapter*.md -o chapters.tex
multimarkdown -t latex meta.txt ../contents/2-appendix*.md -o appendix.tex
cp template.tex OpenSourceBook.tex
#exit
xelatex OpenSourceBook.tex
xelatex OpenSourceBook.tex
xelatex OpenSourceBook.tex
cp OpenSourceBook.pdf ..
echo
echo
echo "Done!"
