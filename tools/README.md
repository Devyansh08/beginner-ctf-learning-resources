# Tools Reference

A categorized reference of tools commonly used in CTF competitions.

---

## Web Security

| Tool | Purpose | Link |
|------|---------|------|
| Burp Suite | HTTP proxy and web testing suite | https://portswigger.net/burp |
| sqlmap | Automated SQL injection testing | https://sqlmap.org |
| ffuf | Web fuzzer for directories and parameters | https://github.com/ffuf/ffuf |
| curl | Command-line HTTP client | Built-in on Linux/macOS |
| Postman | API testing and exploration | https://www.postman.com |

## Cryptography

| Tool | Purpose | Link |
|------|---------|------|
| CyberChef | Encode, decode, and transform data | https://gchq.github.io/CyberChef/ |
| hashcat | GPU-accelerated hash cracking | https://hashcat.net |
| John the Ripper | Password hash cracker | https://www.openwall.com/john/ |
| dCode | Identify and solve classical ciphers | https://www.dcode.fr/en |

## Networking

| Tool | Purpose | Link |
|------|---------|------|
| Wireshark | Packet capture and protocol analysis | https://www.wireshark.org |
| nmap | Network scanning and service detection | https://nmap.org |
| netcat | TCP/UDP data transfer utility | Built-in on Linux |
| tcpdump | Command-line packet capture | Built-in on Linux |

## Reverse Engineering

| Tool | Purpose | Link |
|------|---------|------|
| Ghidra | Disassembler and decompiler | https://ghidra-sre.org |
| GDB | GNU debugger | Built-in on Linux |
| x64dbg | Windows debugger | https://x64dbg.com |
| strings | Extract printable strings from binaries | Built-in on Linux |
| ltrace | Library call tracer | Built-in on Linux |
| strace | System call tracer | Built-in on Linux |

## Digital Forensics

| Tool | Purpose | Link |
|------|---------|------|
| Wireshark | PCAP analysis | https://www.wireshark.org |
| Autopsy | Disk forensics platform | https://www.autopsy.com |
| Volatility | Memory forensics framework | https://volatilityfoundation.org |
| binwalk | Firmware and binary analysis | https://github.com/ReFirmLabs/binwalk |
| steghide | Steganography tool | https://steghide.sourceforge.net |
| foremost | File carving | apt install foremost |
| exiftool | Metadata extraction | https://exiftool.org |
| zsteg | PNG and BMP steganography analysis | https://github.com/zed-0xff/zsteg |

## OSINT

| Tool | Purpose | Link |
|------|---------|------|
| exiftool | File and image metadata extraction | https://exiftool.org |
| Sherlock | Username search across platforms | https://github.com/sherlock-project/sherlock |
| theHarvester | Email and domain reconnaissance | https://github.com/laramies/theHarvester |
| Maltego | Visual link analysis | https://www.maltego.com |

## Blockchain

| Tool | Purpose | Link |
|------|---------|------|
| Remix IDE | Browser-based Solidity IDE | https://remix.ethereum.org |
| Foundry | Smart contract development toolkit | https://getfoundry.sh |
| Etherscan | Blockchain explorer | https://etherscan.io |
| MetaMask | Ethereum browser wallet | https://metamask.io |

## General

| Tool | Purpose |
|------|---------|
| Python 3 | Scripting and exploit automation |
| pwntools | CTF exploit development library |
| Linux terminal | Foundation for nearly all CTF work |

---

## Quick Install (Debian/Ubuntu/Kali)

```bash
# System tools
sudo apt update
sudo apt install -y nmap netcat wireshark binwalk foremost steghide exiftool gdb ltrace strace

# Python libraries
pip3 install pwntools pycryptodome requests

# Ghidra — download from https://ghidra-sre.org
```
