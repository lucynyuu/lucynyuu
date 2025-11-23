<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github.com/lucynyuu/lucynyuu/assets/126999070/a0b4baa4-6b53-4908-8e0f-0528d379d898">
  <source media="(prefers-color-scheme: light)" srcset="https://github.com/lucynyuu/lucynyuu/assets/126999070/b3da3b68-22c0-4215-976f-2dec2d3f9c75">
  <img alt="Change the text colour based on theme" src="https://github.com/lucynyuu/lucynyuu/assets/126999070/b3da3b68-22c0-4215-976f-2dec2d3f9c75">
</picture>

++++++++++[>+++++++++++>++++++++++<<-]>--.+++++++++.>-.<++++.-----------.+++++++++++.----..

**c**, x86asm, c++, and sometimes pascal. Learning Rust 🦀

### Programming peaked at C99

```asm
section .data
bytes:
    db 0xFE, 0x05
    dd 0
    db 0xEB, 0xF9

section .text
    global _start

_start:
    mov rax, 9
    xor rdi, rdi
    mov rsi, 4096
    mov rdx, 7
    mov r10, 34
    mov r8, -1
    xor r9, r9
    syscall

    mov r12, rax

    lea rsi, [rel bytes]
    mov rdi, r12
    mov rcx, 8

.copy:
    movsb
    loop .copy

    lea rbx, [r12 + 0]
    lea rcx, [r12 + 2]
    sub rbx, rcx
    mov [r12 + 2], ebx

    jmp     r12
```

<!--[1]: https://cdn.discordapp.com/attachments/676226832856776714/1023823772140179516/Nyuu.png-->

<!--
**lucynyuu/lucynyuu** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
