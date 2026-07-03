# 🎭 EscapeArtist

**Interactive OS Command Injection Bypass Cheatsheet**

EscapeArtist is a dynamic, web-based utility designed for security researchers, penetration testers, and CTF players. Instead of relying on static lists, it dynamically generates syntactically valid command injection bypasses based on a specific target command and the character restrictions in place.

## 🌐 Live Demo

**[https://giriaryan694-a11y.github.io/EscapeArtist/](https://giriaryan694-a11y.github.io/EscapeArtist/)**

## 🚀 Features

- **Dynamic Payload Generation:** Input a target command (e.g., `cat /etc/passwd`, `ipconfig`) and instantly generate hundreds of bypass variations.
- **Interactive Filter Evasion:** Toggle blocked characters or strings (spaces, semicolons, quotes, slashes, etc.). The tool instantly filters out techniques that won't work and highlights the ones that will.
- **Cross-Platform Support:** Seamlessly switch between Linux, Windows CMD, and Windows PowerShell environments.
- **Context-Aware Alternatives:** Automatically suggests equivalent alternative commands (e.g., `Get-Content` instead of `cat`, `nl` instead of `cat`) based on the command category.
- **Syntactically Valid Payloads:** All chaining techniques use valid dummy prefixes (`echo`, `true`, `false`) so they execute successfully without syntax errors when tested locally.
- **Comprehensive Categories:**
  - Command Chaining & Separators
  - Context Escaping (Quote/String Execution)
  - Whitespace Bypass
  - Encoding & Obfuscation (Base64, Hex, Octal, PS EncodedCommand)
  - Quote & Escape Manipulation
  - Wildcard & Globbing (Valid `forfiles`/`Resolve-Path` techniques)
  - Variable & Environment Tricks
  - Alternative Commands & Executors (Python, Perl, Awk)
  - LOLBIN & CLM Bypasses (pcalua, mshta, wsl, ieexec)
  - Reverse & Indirect Execution
  - Blind / Time-Based Detection
  - Out-of-Band (OOB) Exfiltration
  - Null Byte & Termination
  - Redirection & File Descriptors

## ⚠️ Disclaimer

This tool is intended for authorized security testing, CTF challenges, and educational purposes only. Always obtain proper authorization before testing any systems.
```
