IMAGES = discriminator.png architecture.png generator.png

.PHONY: clean

%.png: %.pdf
	convert -define profile:skip=ICC -density 720 $< -filter point -quality 90 $@

%.pdf: %.tex
	pdflatex $<

all: $(IMAGES)
clean:
	rm -f *.png *.pdf *.log *.aux

