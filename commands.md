# 50 Linux Commands You Should Know
    
`ls` - list the files and directories in the current directory
```bash
ls
```
    
`cd` - change the current directory
```bash
cd dir_name
```

```bash
cd /root
```

```bash
cd /var
```

```bash
cd /var/lib
```
    
`mkdir` - create a new directory    
```bash
mkdir sumitNotes
```

```bash
mkdir sumitNotes, folder1, folder2
```

`rmdir` - remove a directory
```bash
rmdir sumitNotes
```

```bash
rmdir folder1, folder2
```
    
    
`pwd` - print the current working directory    
```bash
pwd
```

`notepad` - open *sumit.py* file in notepad
```bash
notepad sumit.py
```

`code` - create or open *sumit.py* file in VS-Code
```bash
code sumit.py
```

`vim` - create or open *sumit.html* file in vim editor in linux then edit file after work complete then (press `esc` key and for (save `:wq`) (without save `:q!`) and press `enter` for exit file)

```bash
vim sumit.html
```

`cp` - copy files or directories in 

```bash
cp example.txt folder2/
```

```bash
cp example.txt index.txt
```
    
    
`mv` - move or rename files or directories

```bash
mv example.txt backup/
```

`rm` - remove files or directories
    
```bash
rm example.txt
```
    
    
`touch` - create a new empty file or update the timestamp of an existing file
    
```bash
touch shayan.txt
```
    
    
`cat` - concatenate and display files
    
```bash
cat example.txt
```
    
    
`man` - manual for a command
    
```bash
man ls
```
    
    
`htop` - an interactive process viewer and system monitor
    
```bash
htop
```

`ls -lart` - View files with permissions
```bash
ls -lart
```

`chmod` - change the permissions of a file or directory
    
```bash
# https://chmod-calculator.com/

# The first digit represents the owner of the file/directory
# The second digit represents the group that the file/directory belongs to
# The third digit represents all other users
# 0 (no permission)
# 1 (execute only)
# 2 (write only)
# 3 (write and execute)
# 4 (read only)
# 5 (read and execute)
# 6 (read and write)
# 7 (read, write, and execute)

chmod 700 example.txt
```
    
`sudo apt update` - Update all pakage directory
```bash
sudo apt update
```

`sudo apt install` - for install any application

```bash
sudo apt install apache2
```

`chown` - change the owner of a file or directory
    
```bash 
chown new_owner example.txt
```

```bash 
chown www-data example.txt
```

```bash 
chown www-data:www-data example.txt
```

`tar` - create or extract compressed archive files
    
```bash
# x: extract files from an archive
# t: list the contents of an archive
# r: append files to an existing archive
# z: use gzip compression
# j: use bzip2 compression
# cf: create file
#xf: extract file
tar cf archive.tar file1 file2 file3
```

`gzip` - compress files
    
```bash
gzip file.txt
```
    
    
`gunzip` - decompress compressed files

```bash
gunzip file.txt.gz
```
   
`ssh` - connect to a remote server securely
    
```
ssh username@server_address
```
    
    
`scp` - securely copy files between systems
    
```
scp myfile.txt user@remotehost:/home/user/
```
    
`ping` - test network connectivity
    
```
ping 8.8.8.8
```
    

`ifconfig` - display or configure network interfaces
    
`apt install net-tools`

``` 
ifconfig
```
    
`netstat` - display network connection information
    
```bash
netstat
```
    
    
`route` - view or configure network routing tables
    
```bash
route [options] [add/delete/show]
```
    
    
`top` - display system resource usage and processes
    
```bash
top
```
    
    
`ps` - display information about current running processes
    
```bash
ps
```
    
```bash
ps -ef
```
    

```bash
ps -ef | grep sbin
```

```bash
ps aux
```    
    
`kill` - terminate a process
    
```bash
kill [PID]
```
    
    
`systemctl` - control system services and settings
    
```bash
# Start the nginx service
systemctl start nginx

# Check the status of the nginx service
systemctl status nginx

# restart of the nginx service
systemctl restart nginx

# Stop the nginx service
systemctl stop nginx
```
    
    
`service` - control system services
    
```bash
service apache2 start
```

`useradd` - add a new user to the system
    
```bash
useradd sumit
```
    
    
`passwd` - change the password for a user
    
```bash
passwd sumit
```
    
    
`userdel` - delete a user from the system
    
```bash
userdel sumit
```
    
    
`su` - switch user to become another user
    
```bash
su amit
```
    
    
-   sudo - execute a command as another user or with elevated privileges
    
    ```
    sudo
    ```
    
    
-   uptime - display system uptime and load average
    
    ```
    uptime
    ```
    
    
-   df - display disk space usage
    
    ```
    df
    ```
    
    
-   du - display disk usage by file or directory
    
    ```
    du
    ```
    
    
-   mount - mount a file system
    
    ```
    sudo mount /dev/sdb1 /mnt/usb
    ```
    
    
-   umount - unmount a file system
    
    ```
    sudo umount /mnt/usb
    ```
    
    
-   date - display or set the system date and time
    
    ```
    date
    ```
    
    
-   whoami - display the current user name
    
    ```
    whoami
    ```
    
    
-   which - locate a program or command in the system path
    
    ```
    ls
    ```
    
    
-   finger - displays all the information about user
    
    ```
    finger sumit
    ```
    
    
-   uname - display system information
    
    ```
    uname
    uname -a
    ```
    
    
-   history - display a list of previously executed commands
    
    ```
    history
    ```
    
    
-   echo - display text or variables to the console
    
    ```
    echo 'Best for learn coding in shikohabad'
    ```
    
    
-   tee - redirect output to both a file and the console
    
    ```
    $ ls | tee file.txt
    ```
    
    
-   locate - locate any file on the system
    
    ```
    locate file.txt
    ```
    
    
-   sort - sort lines of text in a file or input
    
    ```
    cat file.txt
    banana
    orange
    apple
    sort file.txt
    apple
    banana
    orange
    ```
    
    
-   uniq - remove duplicate lines from a file or input
    
    ```
    cat file.txt
    apple
    orange
    banana
    apple
    banana
    uniq file.txt
    apple
    orange
    banana
    ```
    
    
-   head/tail - display the first/last few lines of a file or input
    
    ```
    #display first 10 lines
    head file.txt
    
    #display last 10 lines
    tail file.txt
    ```