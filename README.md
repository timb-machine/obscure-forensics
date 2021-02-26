# obscure-forensics

# SAP

## ECC

# IBM

## HTTP Server

## WebSphere

## AIX

* Get the version

```uname -a && oslevel -s```

* Get packages

```lslpp -Lc```

* Display crash log

```errpt -a```

* Review audit log

```/usr/sbin/auditpr -v < </path/to/binary>```

* Grab the logs

```tar cvf logs.tar.gz /var/log```

* Dump the running memory (requires a reboot)

```sysdumpstart```

* Dump kernel modules

```genkex```

* List running process

```ps -aef```

* Generate a process tree

```proctree```

* Show process stack

```procstack <PID>```

* List open files

```procfiles -n <PID>```

* Show network connections

```netstat -an```

* Determine who owns a socket (you can also use sockinfo in kdb)

```netstat -Ana && rmsock <socket address> <socket type>```

* Examine running process data

```find /proc```

* Dump a process

```gencore <PID>```

* Create a debug process dump

```snapcore -r <core file name> <program name>```

* Grab the users

```tar cvf users.tar.gz /etc/passwd /etc/group /etc/security```

* Find world writeable files

```find / -perm -o+w -ls```

* Find group writeable files

```find / -perm -o+w -ls```

* Find setUID files

```find / -perm -u+s -ls```

* Find getUID files

```find / -perm -g+s -ls```

* Capture the most likely admin modified files (this will be big)

```tar cvf admin-modified.tar.gz /etc /var /opt /usr/local /home /tmp```

* Kernel debugger

```kdb```

* Userland debugger

```dbx <binary> <core>```

* Trace a process

```truss```

## z/OS

## MQ

## DB/2

## Oracle

### Solaris

### RDBMS

## Cisco

### Cisco IOS

### Cisco ASA

### FTDs

### Webex
