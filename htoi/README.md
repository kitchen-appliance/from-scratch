## Information

This program converts ACII formated hexcode from an input file into the
corresponding integer values and writes them to the output file.
It is written in little endian x86-64 hexcode and uses x86-64 Linux syscalls.

### Files

* **htoi.hex**   The hexcode of the program formatted so the program will
                 output itself when given as an input file. (23571 Bytes long)
* **htoi**       The program as an ELF binary using Linux syscalls. (1097 Bytes
                 long)
* **README.md**  This file.

usage: htoi [input file] [output file] (without brackets)

### Syntax
* A hexcode has a minimum length of 1 ASCII encoded character and a maximum
  length of 16 ASCII encoded characters.
* Hexcodes are separated by each others and comments by any number of ASCII
  space ` ` characters and ASCII newline characters (0x0A).
* Valid hexcode characters are `0 1 2 3 4 5 6 7 8 9 A a B b C c D d E e F f`.
* Comments begin with `#` and end with a newline.

## Program description

For details please read htoi.hex. 

### ELF program header table

1. Program code (permission to read and execute)
   * Virtual address: 0x4001B8 (0x400000 + file offset 0x1B8)
   * Length : 657 Bytes
   * Maps the executable code from the file to memory
2. Read-only data (permission to read)
   * Virtual address: 0x4010E8 (0x401000 + file offset 0xE8)
   * Length : 209 Bytes
   * Maps the read-only data (error messages) to memory
3. Read-write data (permission to read and write)
   * Virtual address: 0x402000
   * Length: 4096 Bytes (one page)
   * Reserves one page of data for stat structure and output

### Code

The hexcode in htoi.hex is written using only digits and uppercase A-F, but it
is possible to write in lowercase a-f too.

Every instruction is written in its own line. The first line of comment is the
breakdown of every part of the instruction in my own naming convention. (see
from-scratch/intel-opcodes for more information). The second line describes what
the instruction does.
