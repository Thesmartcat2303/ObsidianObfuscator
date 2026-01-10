# Obsidian Obfuscator

> **Owners:** TheSmartCat, Mano, NguoiAnhEm

![Obsidian](https://raw.githubusercontent.com/Thesmartcat2303/ObsidianObfuscator/refs/heads/main/example.png)

**Obsidian Obfuscator** is a specialized, closed-source tool designed to protect Python source code. It combines advanced AST manipulation, multiple encoding layers, and runtime checks to prevent reverse engineering, debugging, and unauthorized tampering.

---

## 🔒 Closed Source
> **Note:** Obsidian is currently a closed-source project.  
> The source code is not publicly available at this time.

---

## 🔗 Contact & Support
- **Telegram Channel:** [TheSmartCat2303](https://telegram.me/thesmartcat2303)
- **Zalo Community:** [Join Group](https://zalo.me/g/vzbrod229)
- **Facebook (TheSmartCat):** [Thesmartcat.2303](https://www.facebook.com/Thesmartcat.2303)
- **Facebook (Mano):** [Sang Phung](https://www.facebook.com/sang.phung.85570/)


## 🎥 Introduction
For a detailed overview and demonstration of Obsidian's capabilities, watch our introductory video:  
👉 [**Obsidian Obfuscator Demo**](https://youtu.be/kaocSndVph0)

---

## ✨ Features
- **High-level obfuscation** techniques
- Protection against code analysis and debugging
- **Requests Library Protection** – Complete rewrite of the Requests library into a secure, hook-resistant implementation
- **Anti-Hooking Security** – Prevents library hooking through dynamic import redirection and call obfuscation
- **Strong Request Protection** – Encrypted network calls and anti-tampering request validation
- Designed for Python applications
- Regular updates and improvements

### 🛡️ Core Protection
- **Multi-Layer Encoding:** Wraps code using Marshal, Zlib, BZ2, and Base85/64 encoding to completely hide the original logic.
- **AST Obfuscation:** deeply modifies the AST of the Python code, restructuring logic and control flows to make static analysis nearly impossible.
- **Variable Renaming:** Automatically renames variables and functions to random Unicode or confusing strings.

### 🚫 Anti-Reverse Engineering
- **Anti-PYCDC (Decompiler Crash):** Specifically engineered to crash common Python decompilers like `pycdc` and `uncompyle6` using malformed bytecode and recursion techniques.
- **Anti-Debugging:** Detects debugging environments (e.g., checks `sys.gettrace`) and terminates execution if analysis is detected.
- **Anti-Tamper:** Verifies the integrity of the script and critical functions (like `open`, `os.system`) at runtime. If modification is detected, the script can self-destruct.

### 🔐 Advanced Security Features
- **Library Hooking Protection**: Implements custom import loaders and runtime integrity checks to prevent hooking attacks
- **Requests Rewrite Engine**: Entirely reimplements the Requests library with built-in obfuscation layers
- **Secure HTTP Stack**: Custom HTTP adapter with encrypted payloads and randomized header patterns
- **Anti-Debugging Measures**: Runtime detection of debugging tools and analysis environments
- **Dynamic Code Mutation**: Continuously alters request paths and signatures during execution

---
