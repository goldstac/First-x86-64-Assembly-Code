# My First Assembly Program

This is my very first program written in **x86-64 Assembly** for Linux.  
It demonstrates a minimal program that exits with a specific status code using a system call.

## Code

```asm
.global _start
.intel_syntax noprefix

_start:
    mov rax, 60   # syscall number for exit
    mov rdi, 70   # exit code
    syscall
