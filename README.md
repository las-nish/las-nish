```asm
section .data                           
    message db "There is nothing for you to see here yet and I will put something on later", 10, "Bye Bye :)", 10
    message_length equ $ - message

section .text
    global _start

_start:
    mov rax, 1
    mov rdi, 1
    mov rsi, message
    mov rdx, message_length
    syscall
    
    call    _exit

_exit:
    mov rax, 60
    mov rdi, 0
    syscall
```
