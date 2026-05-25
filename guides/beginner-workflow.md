# Beginner CTF Workflow

A repeatable process for approaching CTF challenges when you are just starting out.

---

## Step 1 — Identify the Category

Read the challenge description carefully. Most CTFs label challenges by category: Web, Crypto, Forensics, Reverse Engineering, OSINT, or Misc. The description often contains hints about the technique required.

---

## Step 2 — Gather Information

Before attempting any solution, collect as much information as possible about the provided file or service.

```bash
# Identify the file type
file challenge_file

# Extract readable strings
strings challenge_file

# Extract metadata
exiftool challenge_file

# Scan for embedded files or signatures
binwalk challenge_file
```

---

## Step 3 — Research

- Search for the challenge type combined with "CTF" on Google
- Check if the challenge matches a known vulnerability pattern
- Look at past CTF writeups on [CTFtime.org](https://ctftime.org/writeups) for similar challenges

---

## Step 4 — Apply Tools

Use the appropriate tools for the category. Refer to the [tools reference](../tools/README.md) for a full list. For encoding or cipher problems, start with CyberChef's "Magic" mode.

---

## Step 5 — Ask for Help

- Use any available hints in the CTF platform
- Ask in the CTF's official Discord server
- Search for educational resources in the relevant section of this repository

---

## Daily Practice Routine

| Time | Activity |
|------|----------|
| 30 minutes | Solve one or two beginner challenges on PicoCTF |
| 20 minutes | Watch a CTF walkthrough video |
| 10 minutes | Review and document what you learned |

---

## Useful One-Liners

```bash
# Decode Base64
echo "SGVsbG8=" | base64 -d

# Search for a flag pattern in a file
strings file.bin | grep -i "flag{"

# Scan all ports on a target
nmap -sV -p- target_ip

# Extract embedded files from a binary
binwalk -e firmware.bin

# Check file type
file unknown_file

# Get image metadata
exiftool image.jpg
```
