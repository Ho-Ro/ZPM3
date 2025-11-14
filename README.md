# ZPM3

ZPM3 is a Z80 coded CP/M 3.0 compatible BDOS replacement.

## ZPM3 source code

The source code can be downloaded from [ZPM3S.ARC](http://cpmarchives.classiccmp.org/cpm/mirrors/www.triton.vg/tesseract/pds/093/zpm3s.arc) in Volume 93 of [Tesseract RCPM+](http://cpmarchives.classiccmp.org/cpm/mirrors/www.triton.vg/TesseractRCPM+Catalog.html).

```
Contents of ZPM3S.ARC
=====================
autotog.com        427  Toggles automatic command recall (if enabled)
autotog.z80       3745  /
bdos.sub           445  A script to build RESBDOS.SPR and BNKBDOS.SPR
bios.txt         11357  Description of some BIOS functions
bnkbdos3.spr     13504  Banked portion of ZPM3 (CP/M 3 BDOS)
bzpm0.z80         3095  Source code of banked ZPM3 (CP/M 3 BDOS)
bzpm1.z80        44602        /
bzpm2.z80        45917       /
bzpm3.z80        40911      /
bzpm4.z80        40283     /
bzpm5.z80        40805    /
bzpm6.z80        43625   /
bzpm7.z80        40439  /
clrhist.com         19  A program to clear the CP/M 3 input history
clrhist.z80       1702  /
makedos.com       2133  Install ZPM3 when you can't do GENCPM
makedos.txt       4237  /
resbdos3.spr      1984  Resident portion of ZPM3 (CP/M 3 BDOS)
rzpm0.z80        36554  Source code of resident ZPM3 (CP/M 3 BDOS)
scb.txt          16257  Description of System Control Block fields
setz3.com          235  Set environment for ZCPR3 features
setz3.z80         2171  /
test152.c         4306  Check calls to BDOS function 152
test152.com       6907  / (Parse File Name)
version.not        825  Manifest
zpm3.txt         21212  Description of ZPM3
zpm3fix.txt       7194  Description of patches by Jon Saxton
zpm3ldr.rel       3072  A CP/M 3 loader capable of handling a CPM3.SYS
zpm3ldr.txt       3094  / larger than 16 kilobytes
zpm3ldr.z80      46841  Disassembly of ZPM3LDR.REL
zpm3s.txt          761  Brief description of this archive
        ====  ========
Total     31    488659
```

## ZPM3 building

The directory `zpm3s` contains the ZPM3 source code that can be assembled and linked on a CP/M system. I provided a `Makefile` for a cross-build under Linux with the support of [ZXCC](https://github.com/Ho-Ro/ZXCC), a CP/M 2/3 emulator for cross-compiling and running CP/M tools under Microsoft Windows and Linux/Unix/macOS.

