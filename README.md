# SimpleCART
Cartridge project for ATARI XE computers based on ATF22V10C

This bank-switched cartridge occupies 8 KB of address space between $A000 and $BFFF. The cartridge memory is divided into 16 banks, 8 KB each. The 4 lowest bits of the DATA written to $D500-$D50F (mirrored) select the bank mapped to $A000-$BFFF. Writing to $D510-$D51F disables the cartridge. The 2 lowest bits of the DATA written to $D520-$D52F (mirrored) select the "side" of SST39SF020A/SST39SF040"

SST39SF010A - 128kB

SST39SF020A - 256kB (2 sides)

SST39SF040 - 512kB (4 sides)

E.g.

POKE 54528,5 - select bank: 5

POKE 54560,1 - select side: 1

POKE 54544,0 - disable CART

The presented solution can be used unlimitedly and freely without any legal obligations, especially in the field of educational, commercial and non-commercial activities.
