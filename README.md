2.)
c)PB6, PB7; 3
f)I2C Speed Mode [Fast Mode]

3.)
c)48
f)6,144V



Komentar:
Uporabila sva NUCLEO, ker nobena ploščica STM ni bila na voljo.
Sprva nisva videla sprememb v STM, kar je bila napaka vezave, to sva hitro popravila.

Tiskarski škrati:
3.)
d) Na koncu "#define ADS1115_ADDRESS 0x??" ne sme biti ";",
saj povzroči napake v User Code Begin 3.

e) "usigned" mora biti "unsigned",
"init16_t" mora biti "int16_t".

g) ADSWrite mora biti "ADSwrite",
"...Master_Recieve" mora biti "...Master_Receive".
