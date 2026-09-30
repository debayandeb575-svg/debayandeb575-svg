HELLO 👋 

[![LinkedIn](https://shields.io)](https://www.linkedin.com/in/debayan-deb-705940432?utm_source=share_via&utm_content=profile&utm_medium=member_android)
[![Instagram](https://shields.io)](https://www.instagram.com/debayan.dev.9256?stkn=MW84cWVyb205c255eA==)

<div align="center">

# ⚡ Debayan Deb
### Systems & Applied Cryptography Engineer • Full-Stack Developer

[![GitHub Profile](https://img.shields.io/badge/GitHub-debayan--deb575--svg-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/debayan-deb575-svg)
[![Smart India Hackathon](https://img.shields.io/badge/SIH-2026-ff9900?style=for-the-badge&logo=target&logoColor=white)](https://github.com/debayan-deb575-svg/provenance-x)

<br/>

```x86asm
global _start
section .text
_start:
    xor    rax, rax                        ; Zero state corruption
    mov    rdi, [rel evidence_stream]      ; Load input binary buffer
    call   sha256_subtle_seal              ; Compute client-side deterministic digest
    cmp    rax, [rel verified_merkle_root] ; Assert cryptographic parity
    jne    abort_compromised_state         ; Terminate on integrity failure
