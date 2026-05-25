# CTF Tips and Tricks

Practical tips collected from experienced CTF players.

---

## General Approach

- Read the challenge description multiple times — the hint is usually there
- Do not spend more than 30 minutes stuck without searching for related writeups
- Document everything you try, even dead ends
- Writing solution writeups after a challenge significantly reinforces learning

---

## First Steps Checklist

For any unknown file or challenge, run through this checklist before diving deeper:

- [ ] Run `file` on every unknown file
- [ ] Run `strings` on every binary or unknown file
- [ ] Run `exiftool` on every image
- [ ] View page source on every web challenge (Ctrl+U)
- [ ] Inspect HTTP headers and cookies
- [ ] Check for common hidden paths: `/robots.txt`, `/.git/`, `/admin`

---

## Flag Format

Most CTFs use a recognizable flag format. Always search for these patterns:

```bash
strings file | grep -i "flag{"
strings file | grep -i "ctf{"
strings file | grep -iE "[A-Za-z0-9_]+\{[^}]+\}"
```

---

## Web Security

- View page source before using any tools
- Test basic SQL injection: `' OR 1=1--`
- Test basic XSS: `<script>alert(1)</script>`
- Check all cookies in browser DevTools
- Use Burp Suite to intercept and modify requests
- Look for hidden form fields and commented-out code

---

## Cryptography

- Unknown encoding? Try CyberChef "Magic" mode first
- Long string of letters and numbers: likely Base64 or hex
- Repeating structure: may be XOR or Vigenere cipher
- Sequence of numbers: may be ASCII character codes
- Compare cipher lengths to plaintext for classical cipher identification

---

## Digital Forensics

- Use `binwalk -e` to extract files embedded in other files
- Use `steghide extract -sf image.jpg` to extract hidden steganographic data
- Open PCAP files in Wireshark and filter by protocol: `http`, `ftp`, `dns`
- Use `zsteg image.png` for LSB steganography in PNG files
- Look for unusual file headers or mismatched extensions

---

## Reverse Engineering

- Always run `strings` before opening a disassembler
- Use `ltrace` and `strace` to observe program behavior before static analysis
- Look for hardcoded strings, passwords, or keys
- Use Ghidra's decompiler view for C-like pseudocode output
- Check for anti-debugging techniques if the program behaves differently under GDB

---

## Resources for Getting Unstuck

- [CTFtime Writeups](https://ctftime.org/writeups) — search by challenge name
- Google: `challenge_name CTF writeup`
- Ask in the competition's official Discord server
- Take a break and return with fresh eyes
