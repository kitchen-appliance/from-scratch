This program converts ACII formated hexcode from an input file into the
corresponding integer values and writes them to the output file.
It uses Linux syscalls.

usage: htoi [input file] [output file] (without brackets)

### Syntax
* A hexcode has a minimum length of 1 ASCII encoded character and a maximum
  length of 16 ASCII encoded characters.
* Hexcodes are separated by each others and comments by any number of ASCII
  space ` ` characters and ASCII newline characters (0x0A).
* Valid hexcode characters are `0 1 2 3 4 5 6 7 8 9 A a B b C c D d E e F f`.
* Comments begin with `#` and end with a newline.
