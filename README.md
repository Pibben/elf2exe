# elf2exe
Utility to convert a static ELF executable file into a DOS MZ executable

## Resources

* https://bytepointer.com/download.php?name=msdos_encyclopedia_article4_program_structure_exe_com.pdf
* https://bytepointer.com/resources/dos_programmers_ref_exe_format.htm
* http://www.delorie.com/djgpp/doc/exe/
* https://wiki.osdev.org/ELF_Tutorial

## Misc.
gcc -nostdlib -ffreestanding -fno-asynchronous-unwind-tables -Wl,--build-id=none -m32 -O2 -Wall -Wl,-T,tst.script tst.c -o tst
