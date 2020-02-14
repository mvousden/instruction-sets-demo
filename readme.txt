About
===

This repository provides a disassembly example, and shows how C-source is
compiled into a series of machine instructions. This repository contains the
following files:

 - in.c: a simple source file that, when compiled, returns 10.

 - dump_no_opt: disassembly of the object file built via `gcc -Wall -c in.c`,
   with comments.

 - dump_opt: disassembly of the object file built via `gcc -Wall -O3 -c in.c`,
   with comments.

 - dump_no_opt_linked: disassembly of the executable file built via `gcc Wall
   -in.c`, without comments.

 - dump_opt_linked: disassembly of the executable file built via `gcc -Wall O3
   -in.c`, without comments.

Dumps made with `objdump -drwC`. Binaries built for elf64-x86-64.

gcc version 5.4.0
objdump version 2.26.1
