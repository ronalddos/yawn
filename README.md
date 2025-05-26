# 🧙‍♂️ Yawn — Hacking while yawn.

*A lazy red team tool for offensive automation and intelligent parsing — with style.*

---

![yawn-logo](./assets/yawn-logo.png)

Yawn is a FOSS tool for offensive security, combining the power of a CLI with the expressiveness of an interactive TUI inspired by Vim. Its unique approach lies in merging a minimalist design with practical features that cover key phases of exploitation, data collection, and evidence generation for Red Team operations, penetration tests, and CTFs.

The project begins in **modern Python**, with a plugin-based modular architecture. Over time, critical components will be rewritten in **Rust**, starting with **PyO3** bindings, and evolving toward a fully native Rust core.

---

## 🧠 Philosophy

> The idea behind Yawn is simple:
> **"You don't have to look busy to be lethal."**

Yawn reflects the tired-yet-sharp routine of real-world Red Teamers: focused, effective, and efficient. The yawn isn't boredom — it's mastery.

---

## ✨ Key Features

* 🧩 **Plugin-based architecture** using simple decorators (`@plugin("inject-xss")`)
* 🧪 **Smart modules** for fuzzing, parsing, injection, and data collection
* 🧙 **Vim-style TUI** with commands like `:scan`, `:q`, `/xss`
* 🔒 **Stealth mode** with randomized delays, headers, and user agents
* 🧠 **Adaptive parsing** with highlighting of IOCs, payloads, CVEs
* 🐍 Built in Python, evolving with PyO3 → full Rust
* 📄 Exportable reports (Markdown, HTML, JSON)
* 🖥️ Terminal-first, productivity-focused design

---

## 🧩 Planned Modules

| Module     | Description                                               |
| ---------- | --------------------------------------------------------- |
| `scan`     | Basic port, directory, and header enumeration             |
| `fuzz`     | Automatic payload injection with wordlists                |
| `inject`   | Exploit XSS, SQLi, LFI, SSTI, and similar vulnerabilities |
| `parse`    | Log and response parser with syntax highlighting          |
| `loot`     | Extract tokens, headers, sensitive paths                  |
| `report`   | Generate evidence-rich reports                            |
| `cloak`    | Obfuscation and WAF evasion techniques                    |
| `enrich`   | Integrations with Shodan, VirusTotal, AbuseIPDB           |
| `proxy`    | Listener for XSS/SSRF callback capture                    |
| `listener` | Basic TCP reverse shell listener for PoCs                 |

---

## 🔍 Use Cases

### 🎯 **CTFs**

* Rapid fuzzing with custom payloads
* Real-time log parsing and IOC spotting
* Scriptable with clean, minimal output

### 🛠 **Penetration Tests & Bug Bounties**

* Evidence collection and formatted payload/response logs
* Silent execution with `--stealth`
* Fast report generation for clients or writeups

---

## 🧪 Technology Roadmap

1. CLI and TUI in Python
2. Plugin system with decorators (`@plugin("mod-name")`)
3. Native parsing and fuzzing logic
4. Packaging with `pipx`, `docker`, `pyinstaller`
5. Performance-critical modules rewritten with **Rust + PyO3**
6. WebAssembly plugin support (future)
7. Final core rewrite in Rust

---

## 📜 License

MIT — Do what you want, but remember: if you're sleepy... exploit anyway 😴
