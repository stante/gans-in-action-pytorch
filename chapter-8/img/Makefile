IMAGES = discriminator.png architecture.png

all: $(IMAGES)

clean:
	rm -f *.png *.pdf *.log *.aux

%.png: %.pdf
	convert -define profile:skip=ICC -density 720 $< -filter point -quality 90 $@

%.pdf: %.tex
	pdflatex $<
