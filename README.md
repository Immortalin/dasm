# dasm

DOM assembler-like language

## this is just a sketch of an idea

What if we could do this:

```asm

Greet     DDIV 
H1        DH1
S         DSTR "Hello World"
LINK      DATTR href "http://asm.org"
A         DA

main:     mov [Greet],[H1]
          mov [H1],S
          mov CX,[A]
          add CX,[LINK]
          add [Greet],CX
          int RENDER
          END main
          
```

