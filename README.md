**Lasan JS** <sub>*2024 Aug 20 @ 8:45:08 p.m.*</sub>

```html
<p>{{ print `Hey 😽 It's my GitHub`; }}</p>
```

<details>
    <summary>Old README</summary>

```asm
; I will modify this content after I create and publish my own programming language

section .data                           
    message db "There is nothing for you to see here yet and I will put something on later", 0
    message_length equ $ - message

section .text
    global _start

_start:
    mov rax, 1
    mov rdi, 1
    mov rsi, message
    mov rdx, message_length
    syscall
    
    mov rax, 60
    mov rdi, 0
    syscall
```

</details>
