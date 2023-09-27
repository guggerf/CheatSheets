# Ubuntu Cheat Sheet

## System Information

Display system information
```bash
uname -a
```

Check Ubuntu version
```bash
lsb_release -a
```
Display hardware information
```
lshw
```
Show system uptime
```
uptime
```
## File and Directory Operations

# List files and directories
```
ls
```
Change directory
```
cd directory_name
```
Navigate to the home directory
```
cd ~
```
Create a new directory
```
mkdir directory_name
```
Remove a file
```
rm file_name
```
Remove a directory and its contents
```
rm -r directory_name
```
Copy a file
```
cp source_file destination
```
Copy a directory and its contents
```
cp -r source_directory destination
```
Move or rename a file/directory
```
mv old_name new_name
```
Display file content
```
cat file_name
```
View file content with pagination
```
less file_name
```

## User Management

Create a new user
```
sudo adduser username
```
Delete a user
```
sudo deluser username
```
Change a user's password
```
sudo passwd username
```
Switch to a different user
```
su username
```
List all users
```
cut -d: -f1 /etc/passwd
```

## Package Management

Update package list
```
sudo apt update
```
Upgrade installed packages
```
sudo apt upgrade
```
Install a package
```
sudo apt install package_name
```
Remove a package
```
sudo apt remove package_name
```
Search for packages
```
apt search package_name
```
All in one command
```
sudo apt update && sudo apt upgrade -y && sudo apt autoremove
```

## Network

Display network information
```
ifconfig
```
Display routing table
```
route
```
Check network connectivity
```
ping domain.com
```
Retrieve public IP address
```
curl ifconfig.me
```

## Process Management

List running processes
```
ps aux
```
Kill a process by PID
```
kill PID
```

## File Permissions

Change file permissions
```
chmod permissions file_name
```
Change directory permissions
```
chmod permissions directory_name
```

Permission modes can also be represented numerically, where each permission has a numeric value:

Read (r) = 4
Write (w) = 2
Execute (x) = 1
So, the permission mode 644 means *rw-r--r--*, and 755 means *rwxr-xr-x*.

## Disk Usage

Show disk space usage
```
df -h
```
Show directory space usage
```
du -h directory_name
```

## Archive and Compression

Create a tar archive
```
tar -cvf archive_name.tar files_or_directories
```
Extract files from a tar archive
```
tar -xvf archive_name.tar
```
Create a compressed gzip archive
```
tar -czvf archive_name.tar.gz files_or_directories
```
Extract files from a gzip archive
```
tar -xzvf archive_name.tar.gz
```

## Miscellaneous

Find files or directories
```
find /path/to/search -name "filename"
```
Shutdown the system
```
sudo shutdown -h now
```
Reboot the system
```
sudo shutdown -r now
```
or
```
sudo reboot
```
View system logs
```
cat /var/log/syslog
```
View manual pages (help)
```
man command_name
```
