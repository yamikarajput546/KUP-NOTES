### WHat is squashfs file system?
Squashfs is a compressed read-only file system for Linux. 
Squashfs compresses files, inodes and directories, and supports block sizes from 4 KiB up to 1 MiB for greater compression. 
Squashfs is also the name of free software, licensed under the GPL, for accessing Squashfs filesystems.




### What are Linux Signals?
A signal is an event generated by the UNIX and Linux systems in response to some condition. Upon receipt of a signal, a process may take action.
A signal is just like an interrupt; when it is generated at the user level, a call is made to the kernel of the OS, which then acts accordingly.
There are two types of signals:
1.  Maskable: signals which can be changed or ignored by the user (e.g., Ctrl+C).
2.  Non-Maskable: signals which cannot be changed or ignored by the user. These typically occur when the user is signaled for non-recoverable hardware errors.
   


### What is the purpose of hidden files?
Files that exist on a computer, but don't appear when listing or exploring, are called hidden files. A hidden file is primarily used to help prevent important data from being accidentally deleted.
Hidden files should not be used to hide confidential information as any user may view them.

### Why ext4 file system is faster than other linux file systems?
1. File system repair time (fsck) in Ext4 is much faster than in Ext2 and Ext3. This is possible because ext4 labels unallocated block groups and inode table sections accordingly, which allows them to be skipped during a file system check.
2.  Delayed allocation allows the file system to postpone selection of the permanent location for newly written user data until the data is flushed to disk. This enables higher performance since it can allow for larger, more contiguous allocations, allowing the file system to make decisions with much better information.

### What is swap space or swap memory?
Swap space in Linux is used when the amount of physical memory (RAM) is full. If the system needs more memory resources and the RAM is full, inactive pages in memory are moved to the swap space. While swap space can help machines with a small amount of RAM, it should not be considered a replacement for more RAM
swap size : type the command: swapon -s.
ram and your swap space usage : free -m

### How to mount a file system?
On Linux and UNIX operating systems, you can use the mount command to attach (mount) file systems and removable devices such as USB flash drives at a particular mount point in the directory tree.
The umount command detaches (unmounts) the mounted file system from the directory tree.

### How to List Mounted File Systems
When used without any argument, the mount command will display all currently attached file systems:
Mount
To mount a file system on device we use mount commands.
For example:    mount [OPTION...] DEVICE_NAME DIRECTORY
### What is difference between sbin and /usr/sbin?
Both are same directory. It contains root binaries which are executable commands to perform perticular tasks. Since these are root level binaries it required root priviledges to run.
/sbin is symbolic link to /usr/sbin

### Cgroups:
Cgroups allow you to allocate resources — such as CPU time, system memory, network bandwidth, or combinations of these resources — among user-defined groups of tasks (processes) running on a system. You can monitor the cgroups you configure, deny cgroups access to certain resources, and even reconfigure your cgroups dynamically on a running system. The cgconfig (control group config) service can be configured to start up at boot time and reestablish your predefined cgroups, thus making them persistent across reboots.

### How to check which ports are being used by which process?

Using lsof command
lsof -i -P -n | grep -i "listen"

where,
-i : Look for listing ports
-P : Inhibits the conversion of port numbers to port names for network files.
-n : Do not use DNS name
Using netstat command
sudo netstat -tulpn | grep LISTEN

where,
-t : All TCP ports
-u : All UDP ports
-l : display listening server
-p : show PID & name
    