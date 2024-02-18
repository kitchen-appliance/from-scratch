## Information

This program converts ACII formated hexcode from an input file into the
corresponding integer values and writes them to the output file.
It is written in little endian x86-64 hexcode and uses x86-64 Linux syscalls.

### Files

* **htoi.hex**   The hexcode of the program formatted so the program will
                 output itself when given as an input file.
* **htoi**       The program as an ELF binary using Linux syscalls.
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
   * Virtual address: 4001B8 (400000 + file offset 1B8)
   * Length : 657 Bytes
   * Maps the executable code from the file to memory
2. Read-only data (permission to read)
   * Virtual address: 4010E8 (401000 + file offset E8)
   * Length : 209 Bytes
   * Maps the read-only data (error messages) to memory
3. Read-write data (permission to read and write)
   * Virtual address: 402000
   * Length: 4096 Bytes (one page)
   * Reserves one page of data for stat structure and output
