# This is for building the whole site
#
# Mark A. Yoder 12-June-2018

hfiles=$(subst adoc,html,$(wildcard *.adoc))
dirs=$(wildcard 0*)

all: $(hfiles) book.pdf

clean:
	rm $(hfiles) book.pdf

%.html:%.adoc
	asciidoctor -v $^
	
%.pdf:%.adoc
	asciidoctor-pdf -v $^
	
