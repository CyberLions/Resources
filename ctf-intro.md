# Common Competiton Categories
###### Important Topics to Learn Before Competing

### Cryptography / Crypto
This challenge can be all over the place. Usually the challenge will give you some ciphertext (and sometimes a hint for the encryption method) and ask for the plaintext. There are many different encryption algorithms, and it's tough enough to cover the basics in a full college course (let alone a single readme). These are some basic sticking points for the crypto challenges:
* Know and recognize different common encryption methods like rot13 and base64
* Get familiar with Python's `hmac`,  `PyCrypto`, `base64`, and other modules
* Simple Python or Bash scripting can come in handy sometimes (e.g. text which is encoded hundreds of times with base64, or text which is iteratively encoded with rot13 and caesar) - really, know how to write loops
* The key to quick decoding is usually googling (this is usually faster than writing your own code or finding a module's specific function to do the work), e.g.
	* "base64 decoder"
	* "rot13 or rotation decoder"
	* "rc4 decoder"
* A crypto class will come in handy for recognizing encryption methods used in harder challenges. Short of that, keep Google in mind and remember that they don't usually want you to write much of your own code for this category (you may be able to find a common stream cipher's decoder online)


### Log Analysis
They'll give you a file with a LOT of lines (don't try opening them; you'll just slow your computer down).
* Be proficient with command line tools for parsing large files:
	* `grep` (keep in mind the `-o` and `--color` flags)
	* `sort` (use in conjunction with `uniq` to cut out duplicates)
	* `uniq` (with `-c` is usually helpful)
	* `wc -l` counts lines of output
	* `tail`, `head`, and `less` are great for examining parts of large output
* Always try to look over enough lines of the logfiles to have an idea of how they've structured them for a particular challenge. Smart regexes are a huge part of the battle of this challenge.
* Python can come in handy if you need a more programmatic way to analyze output (or if your regex skills are lacking)


### Packet Capture / Packet Analysis / Network Traffic Analysis
They give you a .pcap and a bunch of questions. Know your .pcaps.
* Wireshark is a must. Get comfortable with using it
* `tshark` is fine too if you prefer command line interfaces
* Learn how to use the filters to cut down on the number of packets you need to look through


### Binary Exploitation / Reversing / Reverse Engineering / Enumeration and Exploitation
Careful here! These types of challenges have a fairly high learning curve. With some challenges it's feasible to google your way to tools and tips that can help solve a given problem. These challenges may require a more broad and deep knowledge. You'll typically be given a binary file (Linux) or sometimes an .exe, and told to "find the key". Scripting may work for some of the simpler binaries, but eventually you'll find a disassembler (and some smart interpretations) is the best way to go for these challenges.
* First and foremost, proficiency with a decompiler/disassembler is necessary for this challenge.
	* Ida Pro is awesome for disassembly (costs money, but in the future this club may be able to get some licenses?)
	* `radare2` is a popular open-source command line alternative; [www.retdec.com] is a great online resource but doesn't support files over 10MB
	* `readelf`, `objdump`, and `hexdump` are GNU utilities that are quite helpful on a small scale
	* `strings` and `grep -a` are more coreutils that are great for searching through binaries without disassembling (usually good for initial probing of a binary, or for the first parts of a large challenge)
	* `xxd` can sometimes be useful as an alternative to `hexdump`
* Be *comfortable* with C/++ (not just passing knowledge, be able to write it too)
* Helpful to recognize assembly (don't usually need to code it, but be able to read different characteristics like `eax`, `mov`, `jmp`, etc)
* Some knowledge of memory layout (stack and heap), how functions are created and destroyed (stack frames)
* Understand bitwise operations (quick google should help if you're iffy with this point):
	* `&&` is logical AND, but `&` is bitwise AND
	* `^` is bitwise XOR
	* `||` is logical OR, but `|` is bitwise OR
* Recognize pointers, and how code uses pointers in relation to arrays (array indexing)
* Be comfortable with working in binary, decimal, or hex (hex especially will help when reading memory locations)
* Could be helpful to get a hex editor for editing binaries (or [pipe `vim` through `xxd`](http://vi.stackexchange.com/questions/2232/how-can-i-use-vim-as-a-hex-editor), which is what I do)


### Web Exploitation
They'll give you a website and tell you to find a certain vulnerability. Sometimes they'll point you in a certain direction, sometimes not.
* Be proficient with Javascript (primarily), and recognize HTML/CSS
* Check out Chrome's Developer Console, and/or Firebug for Firefox. Both of these let you interact with your browser more powerfully (e.g. manage cookies) which are sometimes the crux of challenges in this category
* Understand common vulnerabilites, like SQL attacks and buffer overflow
* Some knowledge on how common web encryption methods are used (SHA, TLS/SSL, certificates, etc)


### Password Cracking
In this category, you're typically given some users and their hashed passwords. A hint for custom wordlists are usually given for the tougher ones.
* Kali is a must! It has wordlists bundled in `usr/share/wordlists`!
* `hashcat` and `john` (the ripper) are both quite powerful tools for cracking. Get good with one or the other
* Understand rules that these tools use - they're important for cracking tougher pws
* Come up with ideas for creating custom wordlists. Usually the challenge has some kind of hint (e.g. these people all like movies, so you would create a wordlist of all movies)