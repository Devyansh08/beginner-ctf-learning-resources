# 🗺️ Beginner CTF Workflow

A practical workflow for approaching CTF challenges as a beginner.

---

## When You Get a Challenge

### Step 1 — Identify the Category
- Is it Web, Crypto, Forensics, RE, OSINT, or Misc?
- Read the challenge description carefully for hints

### Step 2 — Gather Information
```bash
# For files
file challenge_file          # Identify file type
strings challenge_file       # Extract readable strings
exiftool challenge_file      # Extract metadata
binwalk challenge_file       # Scan for embedded files
```

### Step 3 — Research
- Google the challenge type + "CTF"
- Check if it matches a known vulnerability pattern
- Look at similar past CTF writeups on CTFtime.org

### Step 4 — Try Tools
- Use CyberChef for encoding/decoding
- Use appropriate category tools (see tools/ folder)

### Step 5 — Ask for Help
- Check hint (if available)
- Ask on CTF Discord
- Look at educational resources in this repo

---

## Daily Practice Routine

```
30 min — Solve 1-2 beginner challenges on PicoCTF
20 min — Watch a CTF walkthrough video
10 min — Review what you learned
```

---

## Useful One-Liners

```bash
# Decode base64
echo "SGVsbG8=" | base64 -d

# Find hidden text in image
strings image.png | grep flag

# Scan for open ports
nmap -sV -p- target_ip

# Extract files from binary
binwalk -e firmware.bin

# Check file type
file unknown_file
```
