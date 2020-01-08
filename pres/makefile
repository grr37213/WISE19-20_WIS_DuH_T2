MAIN_NAME:=main
OUT_NAME:=btrg_music_genre_recog_pres.pdf

SRC_CONTENT := $(wildcard content/*.tex)
SRC := $(wildcard *.tex)

main: main.tex
	pdflatex main.tex
#	biber main
#	makeindex -s main.tex -t main.glg -o main.gls main.glo
#	makeindex -s main.ist -t main.alg -o main.acr main.acn
#	makeglossaries main
#	pdflatex main.tex
#do command twice because of tableofcontents (.toc file ) generation.
	mv $(MAIN_NAME).pdf $(OUT_NAME)	
	

clean:
	$(RM) $(MAIN_NAME).aux $(MAIN_NAME).log $(MAIN_NAME).out $(MAIN_NAME).toc
	$(RM) main.pdf $(OUT_NAME)
	$(RM) *.bbl *.bcf *.blg *.run.xml
	$(RM) *.acr *.glg *.ist *.alg *.acn *.gls *.glsdefs *.glo
	$(RM) *.lof
