# 🎭 EscapeArtist — Interactive OS Command Injection Bypass Cheatsheet

**EscapeArtist** is a dynamic, client-side utility designed for security researchers, penetration testers, and CTF players. Unlike static cheatsheets, it dynamically generates syntactically valid command injection bypasses based on your specific target command, allowed wrappers, and target shell environment.

Built for authorized ethical hacking, red teaming, and educational research.

🌐 **Live Demo:** [https://giriaryan694-a11y.github.io/EscapeArtist/](https://giriaryan694-a11y.github.io/EscapeArtist/)

---

## 🚀 Features

- **Dynamic Payload Generation:** Generates bypasses tailored to your exact target command (e.g., `cat /etc/passwd`, `whoami`) rather than generic placeholders.
- **Multi-Shell Targeting:** Dedicated support for **Linux (Bash/Sh)**, **Windows CMD**, and **PowerShell**. Includes a sub-toggle to filter results specifically for CMD-only or PS-only environments.
- **Allowed Command Chaining:** Simulate real-world scenarios where input is appended to a legitimate command (e.g., `ping 127.0.0.1`) by specifying an "Allowed" prefix.
- **Comprehensive Bypass Categories:**
  - 🔗 **Command Chaining:** Semicolons, pipes, AND/OR operators, subshells, and background execution.
  - 🧊 **Context Escaping:** Quote breakouts, string execution, and `.NET` process invocation.
  - ⬜ **Whitespace Bypass:** `$IFS`, brace expansion, tabs, URL-encoded spaces, and environment variable extraction.
  - 🔐 **Encoding & Obfuscation:** Base64, Hex, Octal, PowerShell `-EncodedCommand`, and char-code arrays.
  - 🗣️ **Quote Manipulation:** Empty quotes, caret escapes, backtick escaping, and mixed quoting.
  - 🔄 **Alternative Executors:** Python, Perl, PHP, Ruby, Node.js, and native OS alternatives.
  - 🏠 **LOLBIN & CLM Bypasses:** `pcalua`, `wsl`, `mshta`, `wmic`, `certutil`, and Constrained Language Mode evasions.
- **URL Encoding Toggle:** Instantly encode payloads for HTTP-based injection testing.
- **Zero Dependencies:** Pure HTML/CSS/JS. Runs entirely in the browser—no backend, no tracking, safe for air-gapped environments.
- **Instant Search & Filtering:** Real-time filtering of generated techniques by keyword.

---

## 🛠️ Usage

1. **Select Target OS:** Choose Linux, Windows, or Both.
   - *If Windows/Both is selected*, use the **Shell Target** sub-toggle to filter between CMD, PowerShell, or Both.
2. **Enter Target Command:** Input the command you want to execute (e.g., `cat /etc/passwd`).
3. **(Optional) Set Allowed Prefix:** If the application appends your input to a safe command, enter that command here (e.g., `ping 127.0.0.1`).
4. **Hit Generate:** View categorized bypass techniques with one-click copy functionality.
5. **Toggle URL Encode:** Enable this if injecting via GET parameters or form bodies.


## ⚠️ Disclaimer

> **This tool is provided for authorized security testing, CTF challenges, and educational purposes only.**
>
> Unauthorized access to computer systems is illegal. Always obtain explicit written permission before testing any system. The author assumes no liability for misuse of this tool. Use responsibly and ethically.

---

## 📄 License

MIT License — Feel free to use, modify, and distribute for legitimate security research.

---

**Built by [Aryan Giri](https://github.com/giriaryan694-a11y)** | Cybersec Research & CTF Tooling
