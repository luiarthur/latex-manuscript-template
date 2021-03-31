SHELL := /bin/bash

EntryFile = main

.PHONY: dev clean cleanall

all: dev

build:
	latexmk -pdf $(EntryFile).tex

dev:
	latexmk -pdf -pvc $(EntryFile).tex

clean:
	latexmk -c
	rm -f $(EntryFile).bbl

cleanall:
	latexmk -C
	rm -f *.{log,aux,nav,out,snm,toc,blg,bbl,fdb_latexmk,fls,synctex.gz}
