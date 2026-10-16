# Assembly game of life

A x86 Assembly implementation of Conway's game of life. The program reads the initial configuration either from standard input or from a file named `in.txt`. Afterwards, it outputs the resulting state after n iterations.

## Features and technology

- *Written exclusively in x86 Assembly:* the logic is written in assembly, with I/O using stdlib functions.
- *Two I/O options:* you can either provide the initial state from the terminal or from an input file.

## Structure

- `StandardInput.s` / `Citire.s`: Main program, reading the configuration and handling the logic.
- `FileInput.s`: Version reading from `in.txt` and writing outputs to `out.txt`.
- `matrice.s`: File handling the matrix visualisation.
- `test.c`: A basic C test file.

## Compilation

```
   as StandardInput.s -o StandardInput.o
   gcc -m32 StandardInput.o -o game_of_life
```

## Licence

GPL3
