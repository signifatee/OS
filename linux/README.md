# Linux distros:

1. Basic terms
Kernel - brain of the Linux OS. It controls the hardware and makes it interact with the applications.
Distribution - collection of software(programms) combined with a Linux kernel making up a Linux-based OS. Examples: Ubuntu, Fedora
Boot loader - program that boots the OS. Examples: GRUB and ISOLINUX
Service - program that runs as a background process. Examples: httpd, nfsd, ntpd, ftpd, named
Filesystem - Method for storing and organasing files. Examples: ext3, ext4, FAT, XFS, NTFS, Btrfs 
X Window SYstem - Graphical subsystem on nearly all Linux systems
Desktop Environment - Graphical UI on top of the OS. Examples: GNOME, KDE, Xfce, Fluxbox
Command line: Interface for typing commands on top of the OS
Shell: Command line interpreter that interprets the command line input and instrucs the OS to perform any necessary tasks and commands. Examples: bash, tcsh, zsh
UEFI(Unified Extensible Firmware Interface)- modern interface between the OS and the hardware. It's and analogy to BIOS.

2. Useful commands
man <command> - shows a manual to a certain command

3. Boot process
---
BIOS(Basic Input/Output system) initializes the screen and keyboard and tests the main memory? (POST). The BIOS software is stored in the ROM chip on the motherboard.
OR
UEFI
...
->
Master Boot Record (MBR) also known as First Sector of the Hard Disk, MBR size is 512 bytes
OR
GPT
...
->
Boot loader, which stores on one of the hard disks, is responsible for loading the kernel of the OS into RAM ans passes control to it
->
Kernels are almost always compressed, so the first job for them is to uncompress. After that it will check and analyze the system hardware and initialize ant hardware device drivers built into the kernel.
->
Initial RAM disk - inittramfs image
