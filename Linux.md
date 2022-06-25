# Linux
- Components
  - Hardware
  - Kernel
  - Shell
  - Application
  - Users

## What is Shell
-  It is an environment in which we can run our 
   -  commands, 
   -  shell scripts, 
   -  and programs. 
- It is an interface between user and kernel that hides all complexities of functions of the kernel from the user. 
- It is used to execute commands. 

## Different types of shells
- C shell
- Korn Shell
- BASH
- Bourne Shell

## What is BASH
- Bourne Again Shell
- Command line Editor
- convience to use

## What is Kernel
- A kernel is considered the main component of Linux OS. It is simply a resource manager that acts as a bridge between hardware and software.
- Memory Management
- Process Management
- Storage Management
- Device Management

## Linux User Mod
- Command line
- GUI

## swap space
- RAM Memory

## Process States in Linux
- New/Ready
- Running
- Blocked/Wait
- Terminated/Completed
- Zombie

## VI Editor
- Command Mode/Regular Mode
- Insertion Mode/Edit Mode
- Ex Mode/Replacement Mode

## file permissions in Linux
- Read(r)
- write(w)
- execute(x)

## What do you mean by the daemons
- Daemons is Background Process
  - Line printing daemon(controls the print spooling process)

## load average in Linux
- ```top``` ```uptime```
- It tells you the load that the system has been under

## Linux Networking
- /etc/resolv.conf
  - It is used to configure DNS name servers
  - The DNS server is then used to resolve the hostname of the IP address.
- /etc/hosts
  - It is used to map or translate any hostname or domain name to its relevant IP address.

## NIC
- Network interface Card
- Load Balancing
- Failover
- increase uptime

##  Network bonding
- NIC
  - default Mode is 0
  - Mode 0 (balance-rr)
  - Mode-1 (active-backup)
  - Mode-2 (balance-xor)
  - Mode-3 (broadcast)
  - Mode-4 (802.3ad)
  - Mode-5 (balance-tlb)
  - Mode-6 (balance-alb)

## Ports
- DNS	53
- SMTP	25
- FTP	20
- SSH	22
- DHCP	67
- squid	3128

## standard streams in Linux.
- Standard Input (stdin)
- Standard Output (stdout)
- Standard Error (stderr)

## Linux Commands
- ```netstat```(display all network connections on a system)
- ```ping```
  - (Packet Internet Groper)
  - verify connectivity at an IP -level to a second TCP/IP device, and name resolution. 
- ```/etc/inittab```(check the default run level)
- ```$ du -sh /var/log/*``` (size of file or directory)
- ```wc```( Word Count )
- ```grep [options] pattern [files] ```
  - Search Command
- ```netstat -ntlp``` (check all the listening ports and services of your machin)
- memory status
  - ```cat /proc/meminfo```
  - ```vmstat```
  - ```top```
  - ```htop```

## Linux directory commands
- ```pwd```
- ```ls```
- ```cd```
- ```mkdir```
- ```rmdir```

