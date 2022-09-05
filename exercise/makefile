.PHONY: command
command: step1-command.tex
	latex $^

.PHONY: step2
step2: step2.tex
	latex $^

.PHONY: algorithm
algorithm: step3-algo.tex
	latex $^

.PHONY: clean
clean:
	rm -rf *.aux *.log *.pdf *.gz *.dvi