.PHONY: all clean

all: paper.pdf

paper.pdf: paper.md paper.bib
	pandoc $< \
		--number-sections \
		-V colorlinks=true \
		-V linkcolor=blue \
		--citeproc \
		--bibliography=paper.bib \
		-o $@

clean:
	rm -f paper.pdf
