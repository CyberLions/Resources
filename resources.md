#### todo:
- include references to commonly used tools (e.g. `john`, `hashcat`, `tshark` etc just so beginners know where to start)

# Introductory Sites
###### Explanation, preparation tips, etc
* https://www.wraysec.com/2015/11/02/how-to-win-the-ncl/

# Learning Resources
General bash/intro:  
* [OverTheWire Wargames](http://overthewire.org/wargames/)
* [SmashTheStack](http://smashthestack.org/index.html#)
* [CodeAcademy: command line](https://www.codecademy.com/learn/learn-the-command-line)
* [Learn to Hack](https://hackcenter.com/sign-in)
* [Open-source cybersecurity learning](https://www.cybrary.it/)
* [Embedded Security CTF](https://microcorruption.com/login)

Crypto:  
* [Crypto Training Challenges](https://cryptopals.com/)

Web Exploits:  
* [infosecinstitute](http://ctf.infosecinstitute.com/)
* [Breaker101 web security course](https://breaker101.com/)

Reversing:  
* [Lena tutorials for reversing](https://tuts4you.com/download.php?list.17)
* [Reverse Engineering for Beginners (free ebook)](https://beginners.re/)
  * [corresponding beginners.re challenges](https://challenges.re/)
* [BiW reversing - Tutorials](http://www.reversing.be/index.php?topic=tutorials)
* [BiW reversing - Crackmes](http://www.reversing.be/index.php?topic=crackmes)
* [OpenRCE - Articles](http://www.openrce.org/articles/)
  
Libraries (the info depot kind):  
* [VX Heaven virus library](http://vxheaven.org/)
* [PLASMA hardware identification library](http://www.plasma-online.de/)
* [Sandpile x86 processor information](http://www.sandpile.org/)
* [Open-source hardware IP cores](https://opencores.org/)
* [FPGA CPUs and MISCs](http://www.fpgacpu.org/links.html)

# Various Helpful Online Tools
There are a lot of powerful, free tools online which you can easily use instead of having to download or learn software packages. Really helpful if you're rushed for time and can't go looking around for the best software to install or how to use it.

### Web Exploitation
- SSL/cert checker (for use in open-source google-fu challenges). Parts of this website will also show the `openssl` commands used so you can learn what's happening
  - https://www.sslshopper.com/ssl-checker.html
- Another ssl checker. Much deeper than the previous one (notable benefit: shows the size of the cert chain)
  - https://www.ssllabs.com/ssltest/analyze.html

### Binary Exploitation
- Retargetable Decompiler: a powerful decompiler and disassembler for executables. Works quite well (files under 10MB) and can show disassembled executable as code or branch diagrams
  - https://retdec.com/
  
### Binary Disassembly
- ODA - the online disassembler: a binary disassembler that is a good resource for reversing on the go
  - https://www.onlinedisassembler.com/odaweb/

### Password Cracking
- Keep in mind Kali Linux has a few wordlists included at `/usr/share/wordlists/`
- Good repos for more wordlists
  - https://github.com/danielmiessler/SecLists/tree/master/Passwords
- Cracked password hashdumps
  - http://siph0n.net/hashdump.php
  
### VulnHub CTFs
- Vulnerable virtual machines that give you a hands on approach to learning digital security. Similar to actual competitions with the added benefit that you can do them at your own leisure.
  - https://www.vulnhub.com/entry/skydog-2016-catch-me-if-you-can,166/
  - https://www.vulnhub.com/entry/mr-robot-1,151/
  - https://www.vulnhub.com/entry/sickos-11,132/
  
