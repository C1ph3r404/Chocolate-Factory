# README.md — Chocolate Factory (TryHackMe)

## Quick summary
This repo contains my writeup for the **Chocolate Factory** TryHackMe box. Short version: found hidden data in an FTP image, cracked a SHA512crypt hash to get `charlie`'s password, used the web app to get `www-data`, grabbed `charlie`'s SSH private key, SSH'd in, and then used `sudo vi -c ':!/bin/sh' /dev/null` to escalate to root.

## Files
- `WriteUp.md` — full step-by-step walkthrough (this file)  
- `screenshots/` — evidence: nmap, steghide, hashcat, web shell, keys, and flags

## Tools used
- `nmap`, `ftp`, `steghide`, `base64`, `hashcat`, `nc` (netcat), `ssh`, `strings`

## Disclaimer
For educational purposes only. Don’t attack systems without permission.

---
