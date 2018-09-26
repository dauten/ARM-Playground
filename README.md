# ARM-Playground
Sample scripts to test ARM on a Raspberry Pi 3
Feel Free to use or Distrubute these to learn/teach others ARM if you think they'll be useful.
Some things taken from http://www.science.smith.edu/dftwiki/index.php/Tutorial:_Assembly_Language_with_the_Raspberry_Pi

## Compiler/Builder Cheatsheet
\*.c=C code file, not assembly but can be converted to assembly to study
\*.s=Assembly code file
\*.o=Object file
Convert C code to assembly code.  Exclude -fverbose-asm to exclude comments in compiled file
> gcc <input c file> -S -fverbose-asm -o <output assembly file>
  
Assemble assembly code file
> as <input assembly file> -o <output assembled object file>
  
Compile Assmbled object file into raw binary executable
> gcc <input assembled file name> -o <output binary executable>
