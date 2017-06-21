LATEX=pdflatex

.PHONY=clean clean-all

all: note.pdf clean

note.pdf: note.tex
	while ($(LATEX) note.tex ; \
	grep -q "Rerun to get cross" note.log ) do true ; \
	done

clean:
	rm -f note.aux  note.log
	rm -rf auto

clean-all: clean
	rm note.pdf
