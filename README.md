# The Linux Programming Interface

Code based off the book.

The actual source doe belongs here: https://man7.org/tlpi/code/

## Building the /lib functions
### Manually
```bash
cd lib/
gcc    -c -o error_functions.o error_functions.c
gcc    -c -o get_num.o get_num.c
ar rs ../libtlpi.a *.o
```

### Using Make
```bash
cd lib/
make
```

## Building and linking to the book library example
Example uses the fileio chapter of the book
### Manually
```bash
cd fielio
gcc copy.c -I../lib ../libtlpi.a -o copy
```

### Using Make
```bash
cd fileio/
make copy
```

