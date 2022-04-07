NAME     = exemplo

TXT      = $(NAME).txt
PDF      = $(NAME).pdf

all: $(PDF)

$(PDF): $(TXT)
	preconv $^ | groff -dpaper=a4 | ps2pdf - $@

clean:
	rm -f $(PDF)

show: $(PDF)
	zathura $(PDF)

