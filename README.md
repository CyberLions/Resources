# Resources
This repository contains helpful external links to resources/tools to solve competition challenges

## todo:
- add links to other, fuller repos like this (Kevin found a few good ones?)
- include references to commonly used tools (e.g. `john`, `hashcat`, `tshark` etc just so beginners know where to start)

## Helpful Online Tools
There are a lot of powerful, free tools online which you can easily use instead of having to download or learn software packages. Really helpful if you're rushed for time and can't go looking around for the best software to install or how to use it.

### Web Exploitation
- SSL/cert checker (for use in open-source google-fu challenges). Parts of this website will also show the `openssl` commands used so you can learn what's happening
  - https://www.sslshopper.com/ssl-checker.html
- Another ssl checker. Much deeper than the previous one (notable benefit: shows the size of the cert chain)
  - https://www.ssllabs.com/ssltest/analyze.html

### Binary Exploitation
- Retargetable Decompiler: a powerful decompiler and disassembler for executables. Works quite well (files under 10MB) and can show disassembled executable as code or branch diagrams
  - https://retdec.com/

### Password Cracking
- Keep in mind Kali Linux has a few wordlists included at `/usr/share/wordlists/`
- Good repos for more wordlists
  - https://github.com/danielmiessler/SecLists/tree/master/Passwords
- Cracked password hashdumps
  - http://siph0n.net/hashdump.php
