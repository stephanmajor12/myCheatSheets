#My Linux Cheat Sheet:

## Getting Started ##

## Go
- [Directory](https://github.com/stephanmajor12/myCheatSheets/blob/main/Linux-Commands/linuxCheatSheet.md#directory-commands)
- [Disk Management](https://github.com/stephanmajor12/myCheatSheets/blob/main/Linux-Commands/linuxCheatSheet.md#disk-management)
- [File Permissions](https://github.com/stephanmajor12/myCheatSheets/blob/main/Linux-Commands/linuxCheatSheet.md#file-permission-numbers)
- [Vim Reference](https://github.com/stephanmajor12/myCheatSheets/blob/main/Linux-Commands/linuxCheatSheet.md#vim-quick-ref)
- [Process Management](https://github.com/stephanmajor12/myCheatSheets/blob/main/Linux-Commands/linuxCheatSheet.md#process-management)
- [NetWorking](https://github.com/stephanmajor12/myCheatSheets/blob/main/Linux-Commands/linuxCheatSheet.md#networking)
### Directory Commands ###

```
pwd - Shows current Directory
mkdir *dir* - Creates a new Directory
cd *dir* - Changes Directory
cd .. - Go up a Directory
ls - List files
```

### Disk Management ###

```
mkfs -t FORMAT DEVICE - formats a dick,   Example: mkfs -t ext4 /dev/sda2
df <OPTIONS> <FILE> - shows how much space is free on file system,  Example: df -h file.txt
du <OPTIONS> <FILE> - shows you how much space a dir takes up,  Example: du -c -t 500M /home
mount <OPTIONS> <FILE> - lets you mount the file system as defined,     Example: mount -t ext4 /dev/sdb1 /var/db
umount DIRECTORY | DEVICE - to unmount, umount /media
```

### File Permission Numbers ###

```
4 - read(r)
2 - write(w)
1 - execute(x)
```

### Vim quick ref ###

```
:q - exit
:q! - force exit
:wqa - write(save) and quit all tabs
:sav[eas] file - save file as
:w - write but don't exit
~ - switch case
d - delete marked text
```

### Process Management ###

```
ps - show snapshot of processes
top - show real time processes
kill *pid* - kill process with id *pid*
pkill *name* - kill process with name *name*
killall *name* - kill all processes with names beginning *name*
```

### NetWorking ###
 
```
SSH username@ip-address or hostname - login into a remote linux machine
Ping hostname="" or ="" - pings host
Ssh-keygen -t ed25519 -C your@email.com - sends you an ssh key
Scp myfile.txt user@dest:/path - uploads a file to the server
Scp user@dest:/path/myfile.txt locapath - downloads file
Git clone git@github.com:examplerepo ??? clones a github repo into current dir.
```

End!
