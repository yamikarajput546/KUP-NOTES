### What is the GNU project?
GNU stands for GNU's not Unix. 
The GNU project is a mass collaborative initiative for the development of free software. 
The original purpose of the GNU project was the creation of a free operating system. Free, in a software context, does not necessarily mean free of cost. 
The freedom referred to is the ability of anyone who wishes to run, copy, distribute, study, change and improve the software.

| Linux  - | Unix |
|  - | --------------------------- |
| Linux is open source and is developed by Linux community of developers. |Unix was developed by AT&T Bell labs and is not open source.|
| Linux is free to use. |Unix is licensed OS.|
| Ext2, Ext3, Ext4, Jfs, ReiserFS, Xfs, Btrfs, FAT, FAT32, NTFS. | s, gpfs, hfs, hfs+, ufs, xfs, zfs.|
| Linux is used in wide varieties from desktop, servers, smartphones to mainframes. | Unix is mostly used on servers, workstations or PCs.|
| Distros are Ubuntu, Debian GNU, Arch Linux, etc.| SunOS, Solaris, SCO UNIX, AIX, HP/UX, ULTRIX etc.|

### What are different distros of linux and their purpose?
Debian,
Linux Mint,
Ubuntu,
Elementary OS,
Fedora,
Elementary OS.

### When should I go for Ubuntu & when for other systems?


Each distribution can have a different focus - Your choice of distribution will depend on what you are trying to accomplish.

Many distributions available to choose - Commercial and non-commercial. Commercial Linux distributions are backed by corporations, and you can buy support from    them. You have Linux distributions that are designed for server use, others that are designed for desktop use. Some are focused on research and science, others    are focused on multimedia production.
  
### What is BIOS and system integrity checks?
BIOS is short for Basic Input-Output system. It’s low-level software that resides in a chip on your computer’s motherboard. The BIOS loads when your computer starts up, and the BIOS is responsible for waking up your computer’s hardware components, ensures they’re functioning properly, and then runs the bootloader that boots Windows or whatever other operating system you have installed.

 System integrity check :It is a parameter that is responsible for checking the status of all security detectors and devices before arming. Checking is disabled by default.
This function is mandatory for professional security systems. It does not allow activating the arming mode if the window is not closed in the room, the detector lid is open, or communication with one of the devices is lost.


### What is UEFI? Difference between UEFI and BIOS?
UEFI stands for Unified Extensible Firmware Interface. It does the same job as a BIOS, but with one basic difference: it stores all data about initialization and startup in an .efi file, instead of storing it on the firmware.
1. UEFI supports drive sizes upto 9 zettabytes, whereas BIOS only supports 2.2 terabytes.
2. UEFI provides faster boot time.
3. UEFI has discrete driver support, while BIOS has drive support stored in its ROM, so updating BIOS firmware is a bit difficult.
4. UEFI offers security like "Secure Boot", which prevents the computer from booting from unauthorized/unsigned applications.


### Getty Command
getty short for “get tty” is a Unix program running on a host computer that manages physical or virtual terminals to allow multi-user access. 

Linux provides virtual terminal(tty) which is similar to the regular Linux terminal. agetty command opens a virtual terminal(tty port), prompts for a login name and invokes the /bin/login command. 

### init 
The init is a daemon process which starts as soon as the computer starts and continue running till, it is shutdown. In-fact init is the first process that starts when a computer boots, making it the parent of all other running processes directly or indirectly and hence typically it is assigned “pid=1“.
### Init command
init [OPTIONS...] COMMAND
Send control commands to the init daemon.
Commands:\

0 Power-off the machine \
6 Reboot the machine \
2, 3, 4, 5 Start runlevelX.target unit \
1, s, S Enter rescue mode \
q, Q Reload init daemon configuration \
u, U Reexecute init daemon \
Options:
--help Show this help
--no-wall Don't send wall message before halt/power-off/reboot \

### systemd
A systemd is a System Management Daemon named with UNIX convention to add ‘d‘ at the end of daemon.. Similar to init, systemd is the parent of all other processes directly or indirectly and is the first process that starts at boot hence typically assigned a “pid=1“.

### Difference between Systemd & init d.
A init process starts serially i.e., one task starts only after the last task startup was successful and it was loaded in the memory. This often resulted in delayed and long booting time. However, systemd was not designed for speed but for getting the things done neatly which in turns avoid all the UNnecessary delay.

### Uname commands
The command ‘uname‘ displays the information about the system.
Syntax: uname [OPTION]
1. -o option: It prints the name of the operating system.
2. -s option: It prints the kernel name.
3. -n option: It prints the hostname of the network node(current computer).
4. -r option: It prints the kernel release date.
5. -v option: It prints the version of the current kernel.
6. -m option: It prints the machine hardware name.
7. -p option: It prints the type of the processor.
8. -i option: It prints the platform of the hardware.


### What's the  mean of  systemd.unit(5)?
systemd.unit(5) for the common options of all unit configuration files. The common configuration items areconfigured in the generic [Unit] and [Install] sections. The service specific configuration options are configured in the [Service] section.













