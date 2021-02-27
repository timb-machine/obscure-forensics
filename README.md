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

* List the mounts

```mount```

* Clone the root volume group

```mksysb -i <filename>```

* Clone a partition to file (this is not generally advised for the root partition, unless you're planning to analyse it offline rather than bring it up elsewhere due to it creating an *exact* copy of the vulme, ODM and all)

```dd if=<device path> of=<filename>```

* Dealing with more complex logical volume setups

https://www.ibm.com/support/knowledgecenter/ssw_aix_72/devicemanagement/logvolstorcon.html

* Migrate an LPAR outright

https://www.ibm.com/support/pages/live-partition-mobility

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
