# 💡 General CTF Tips & Tricks

Hard-won tips from experienced CTF players.

---

## 🧠 Mindset

- **Don't give up too fast** — most challenges are solvable with the right approach
- **Google everything** — CTF skills are about knowing what to search
- **Write writeups** — documenting solutions reinforces learning
- **Collaborate** — CTF is a team sport

---

## 🔍 Always Check These First

- [ ] `file` command on every unknown file
- [ ] `strings` on every binary
- [ ] `exiftool` on every image
- [ ] Page source (Ctrl+U) on every web challenge
- [ ] HTTP headers and cookies
- [ ] Check for hidden directories (`/robots.txt`, `/.git/`)

---

## 🚩 Flag Format Hints

Most CTFs use a flag format like:
- `flag{...}`
- `CTF{...}`
- `picoCTF{...}`

Always grep for these patterns:
```bash
strings file | grep -i "flag{"
strings file | grep -i "ctf{"
```

---

## 🌐 Web Security Tips

- Always check page source first
- Try basic SQLi: `' OR 1=1--`
- Try XSS: `<script>alert(1)</script>`
- Check cookies in DevTools
- Use Burp Suite to intercept requests

---

## 🔑 Crypto Tips

- Unknown encoding? Try CyberChef "Magic" mode
- Long string of letters/numbers? Probably Base64 or Hex
- Repeating pattern? Might be XOR or Vigenere
- Numbers only? Could be ASCII codes

---

## 🖥️ Forensics Tips

- Use `binwalk -e` to extract embedded files
- Use `steghide extract -sf image.jpg` for steganography
- Open PCAP files in Wireshark, filter by `http` or `ftp`
- Look for unusual file extensions

---

## ⚙️ Reverse Engineering Tips

- Always run `strings` first
- Use `ltrace` and `strace` before disassembling
- Look for hardcoded passwords or keys
- Use Ghidra's decompiler view for C-like pseudocode

---

## 📚 Resources for Getting Unstuck

- [CTFtime writeups](https://ctftime.org/writeups)
- [Google: challenge_name CTF writeup]
- Ask on CTF Discord servers
- Take a break and come back fresh
