---
layout: default
title: TryHackMe Notes
---

# TryHackMe Notes

## Box: Simple CTF

- Found port 21 open → Anonymous FTP allowed
- Enumerated `/ftp/secret.txt` → contained base64 flag
- Used `gobuster` to brute-force `/admin`

## Box: Vulnversity

- UDP port 69 (TFTP) open
- Used nmap with `-sU -p 69`
- Reverse shell with netcat worked on port 4444
