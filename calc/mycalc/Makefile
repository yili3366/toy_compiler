all:
	yacc -dv mycalc.y
	lex mycalc.l
	cc -o mycalc y.tab.c lex.yy.c
.PHONY: clean
clean:
	rm -fr *.c *.h *.output mycalc
