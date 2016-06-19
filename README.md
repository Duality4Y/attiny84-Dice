# attiny84-Dice


this is a attiny84 dice build.
idea is to have a dice that throws numbers for you on a led "display"
numbers are randomly selected.
the dice has a tilt switch which allows you to throw by shaking the dice.

hardware folder contains a schematic for eagle-cad.
src contains the c source which goes through some numbers,
before deciding on a number.

the assembler source is in the asm folder.
it comes with a assembler binary. (for linux might I add)
``` gavrgasm dice.asm```
find assembler at: http://www.avr-asm-tutorial.net/gavrasm/index_en.html
compiling with scons script as follows:
``` scons ```
and to upload using a programmer predefined in the script (variable programmer)
``` scons upload=1 ```

want to compile for some other mcu ?
look for the mmcu and mcu variables in Sconstruct script.

want to use a different programmer ?
look for the programmer variable in the Sconstruct script.

want to upload to a avr that has the arduino bootloader ?
you can just select 'arduino' for the programmer.
