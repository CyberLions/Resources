# Computer Setup for CTF Challenges and Cybersecurity

* [Windows](#windows) (ok)
* [Mac](#mac) (better)
* [Linux](#linux) (best)

<a name="windows"></a>
## Windows

If you're running Windows, there may a few different things you'll have to do to setup for a CTF.

### [Access Bash from Windows 10](http://www.howtogeek.com/249966/how-to-install-and-use-the-linux-bash-shell-on-windows-10/)
This is pretty important for you to do, but it probably won't be the only thing you'll have to do. Windows command prompt (DOS) isn't great by itself for a bunch of reasons, so Win10 introduced access to a Bash command line. Setting this up will allow you access to standard GNU utils from your host operating system, so you'll use it if you want to test something quickly without spinning up a full VM (for example, running a quick python script or using `hashcat` for a cracking easy passwords).  

Note: even if you set up Bash access, you'll still need a Linux architecture (i.e. virtual image) to run Linux executables. This should only really be a problem once you're doing Reversing challenges - which are pretty difficult - so this isn't something you'll need to worry about when starting off.

### Virtual Machine
You can also choose to run a virtual machine from your computer. A virtual machine program will virtualize an operating system as a program, allowing you to "open" an Ubuntu or Kali Linux image as though it's just another application on your host computer.  
* [VirtualBox](https://www.virtualbox.org/wiki/Downloads) is a popular free virtual machine software
* [VMWare Workstation](http://www.vmware.com/products/workstation.html) is pretty good, but it is paid

<a name="mac"></a>
## Mac OS

If you're running OS X, there are a few different things you can do to prepare.

### Mac Package Manager
This option is probably the best if you'll be getting more interested in cybersecurity or even programming in general. By installing a package manager on Mac, you'll be able to deal with installed packages on your host operating system more easily (and as a side result you'll learn command line better!). You also won't have to deal with running a potentially slow virtual machine for the duration of a competition. There are two popular package managers for Mac:  
* [Homebrew](http://brew.sh/) - which I recommend - deals with packages slightly better and typically has more packages and more updated versions of packages for installation. Once you have it installed, you can run something like `brew install hashcat` or `brew install wireshark` to have Homebrew install the packages and their dependencies easily.  
* or [MacPorts](https://www.macports.org/). Once you have this one installed you can install packages with `sudo port install [package]`  

Note: if you do use a package manager, you'll still need a Linux architecture (i.e. virtual image) to run Linux executables. This should only really be a problem once you're doing Reversing challenges - which are pretty difficult - so this isn't something you'll need to worry about when starting off.

### Virtual Machine
You can also choose to run a virtual machine from your computer. A virtual machine program will virtualize an operating system as a program, allowing you to "open" an Ubuntu or Kali Linux image as though it's just another application on your host computer.  
* [VirtualBox](https://www.virtualbox.org/wiki/Downloads) is a popular free virtual machine software
* [VMWare Fusion](http://www.vmware.com/products/fusion/fusion-evaluation.html) is pretty good, but it is paid (can obtain a cheap license through PSU as a student though!)

<a name="linux"></a>
## Linux

If you're already on Linux you're almost done!

### Kali Linux
This OS is the go-to for pentesting and security work. It's based off of Debian, so it uses the `apt-get` package manager, and it comes with a full suite of pentesting tools installed. If you're running a virtual machine from a different operating system for cybersecurity, Kali should be your first pick.

### Ubuntu
This is a pretty standard, fully-featured Linux distro. It also uses the `apt-get` package manager. If you're using it in relation to pentesting, there are a bunch of tools you should immediately install, like `jon`, `hashcat`, `wireshark`, etc.  
* [The Katoolin project by LionSec](https://github.com/LionSec/katoolin) is a script that will allow you to install all Kali tools on Ubuntu. You don't necessarily have to use it but it can be a good springboard for manually installing tools if you want.

### Arch Linux
If you're running Arch you probably know what you need.
