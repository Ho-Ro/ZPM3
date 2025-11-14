# Linux Makefile to build the zpm3 system


GENCPM3 = zxcc gencpm3
LINK =    zxcc link
LOAD =    zxcc load
MAC =     zxcc mac
PIP =     zxcc pip
ZSM4 =    zxcc zsm4



.PHONY: all
all: bnkbdos3.spr resbdos3.spr autotog.com clrhist.com


bnkbdos3.spr: bnkbdos3.rel
	$(LINK) bnkbdos3[b]

resbdos3.spr: resbdos3.rel
	$(LINK) resbdos3[b]


bnkbdos3.rel: bzpm0.z80 bzpm1.z80 bzpm2.z80 bzpm3.z80 bzpm4.z80 bzpm5.z80 bzpm6.z80 bzpm7.z80
	$(ZSM4) bnkbdos3=bzpm0.z80

resbdos3.rel: rzpm0.z80
	$(ZSM4) resbdos3=rzpm0.z80


autotog.com: autotog.rel
	$(LINK) autotog

autotog.rel: autotog.z80
	$(ZSM4) =autotog.z80


clrhist.com: clrhist.rel
	$(LINK) clrhist

clrhist.rel: clrhist.z80
	$(ZSM4) =clrhist.z80


.PHONY: clean
clean:
	rm -f *~ *.rel *.sym *.lis

