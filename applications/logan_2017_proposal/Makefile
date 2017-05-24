.PHONY : clean

CC=pdflatex
FILES=cover_letter.pdf proposal.pdf

all: $(FILES) composite.pdf

clean:
	rm *.aux *.log $(FILES) composite.pdf

cover_letter.pdf: cover_letter.tex
	$(CC) cover_letter.tex

proposal.pdf: proposal.tex
	$(CC) proposal.tex

composite.pdf: $(FILES)
	pdfunite $(FILES) composite.pdf
