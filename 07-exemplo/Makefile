SOURCE = ./formulas.ms

MS   = ${SOURCE}
PDF  = $(SOURCE:.ms=.pdf)

all: $(PDF)

$(PDF): $(MS)
	groff -ms -U -e -p -KUTF-8 -Tdvi -dpaper=a4 $^ | dvipdfm > $@

clean:
	rm -f $(PDF)

show: $(PDF)
	zathura $(PDF)

