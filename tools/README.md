# 🛠️ CTF Toolset Reference

A complete reference of tools used across CTF categories.

---

## By Category

### 🌐 Web Security
| Tool | Purpose | Download |
|------|---------|---------|
| Burp Suite | HTTP proxy & web testing | https://portswigger.net/burp |
| Postman | API testing | https://www.postman.com |
| curl | CLI HTTP requests | Built-in (Linux/Mac) |
| Browser DevTools | Inspect JS/requests | Built-in (F12) |
| sqlmap | Automated SQLi testing | https://sqlmap.org |
| ffuf | Web fuzzer | https://github.com/ffuf/ffuf |

### 🔑 Cryptography
| Tool | Purpose | Download |
|------|---------|---------|
| CyberChef | Encode/decode/transform | https://gchq.github.io/CyberChef/ |
| hashcat | Hash cracking | https://hashcat.net |
| John the Ripper | Password cracker | https://www.openwall.com/john/ |
| dCode | Cipher identifier | https://www.dcode.fr/en |

### 📡 Networking
| Tool | Purpose | Download |
|------|---------|---------|
| Wireshark | Packet capture/analysis | https://www.wireshark.org |
| nmap | Network scanner | https://nmap.org |
| netcat | TCP/UDP swiss army knife | Built-in (Linux) |
| tcpdump | CLI packet capture | Built-in (Linux) |

### ⚙️ Reverse Engineering
| Tool | Purpose | Download |
|------|---------|---------|
| Ghidra | Disassembler/decompiler | https://ghidra-sre.org |
| GDB | GNU debugger | Built-in (Linux) |
| x64dbg | Windows debugger | https://x64dbg.com |
| strings | Extract strings | Built-in (Linux) |
| file | Identify file type | Built-in (Linux) |
| ltrace / strace | Library/system call tracer | Built-in (Linux) |

### 🖥️ Digital Forensics
| Tool | Purpose | Download |
|------|---------|---------|
| Wireshark | PCAP analysis | https://www.wireshark.org |
| Autopsy | Disk forensics | https://www.autopsy.com |
| binwalk | Firmware/binary analysis | https://github.com/ReFirmLabs/binwalk |
| steghide | Steganography | https://steghide.sourceforge.net |
| foremost | File carving | apt install foremost |
| exiftool | Metadata extraction | https://exiftool.org |
| Volatility | Memory forensics | https://volatilityfoundation.org |
| zsteg | PNG/BMP stego | https://github.com/zed-0xff/zsteg |

### 🔍 OSINT
| Tool | Purpose | Download |
|------|---------|---------|
| exiftool | File metadata | https://exiftool.org |
| Sherlock | Username search | https://github.com/sherlock-project/sherlock |
| Maltego | Link analysis | https://www.maltego.com |
| theHarvester | Email/domain recon | https://github.com/laramies/theHarvester |

### ⛓️ Blockchain
| Tool | Purpose | Link |
|------|---------|------|
| Remix IDE | Solidity IDE | https://remix.ethereum.org |
| MetaMask | Ethereum wallet | https://metamask.io |
| Etherscan | Blockchain explorer | https://etherscan.io |
| Foundry | Smart contract toolkit | https://getfoundry.sh |

### 🐍 General / Scripting
| Tool | Purpose |
|------|---------|
| Python 3 | Scripting & automation |
| pwntools | CTF exploit library |
| Linux Terminal | Everything |

---

## 🚀 Quick Install Script (Linux/Kali)

```bash
# Update system
sudo apt update && sudo apt upgrade -y

# Essential tools
sudo apt install -y nmap netcat wireshark binwalk foremost steghide exiftool gdb ltrace strace strings

# Python tools
pip3 install pwntools pycryptodome requests

# Ghidra (download separately)
# https://ghidra-sre.org
```
