NAME = ./bhaskara

MS   = $(NAME).ms
PDF  = $(NAME).pdf

all: $(PDF)

$(PDF): $(MS)
	groff -ms -U -e -p -KUTF-8 -Tdvi $^ | dvipdfm > $@

clean:
	rm -f $(PDF)

show: $(PDF)
	zathura $(PDF)

