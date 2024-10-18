# Estudo de comandos NASM

 src="https://seeklogo.com/images/N/netwide-assembler-nasm-logo-EC5B1109AC-seeklogo.com.png" alt="eu não posso mais" width=100>

<img src="https://seeklogo.com/images/N/netwide-assembler-nasm-logo-EC5B1109AC-seeklogo.com.png" alt="eu não posso mais" width=196>

<img src="https://seeklogo.com/images/N/netwide-assembler-nasm-logo-EC5B1109AC-seeklogo.com.png" alt="eu não posso mais" width=289>

## primeiros comandos

* programa hello world

```assembly
global _start
    section .text
    _start:
        mov rax,1
        mov rdi,1
        mov rsi,message
        mov rdx, 13
        syscall
        mov rax,60
        xor rdi, rdi
        syscall

        section .data
        message:db 'Hello, World',10
```