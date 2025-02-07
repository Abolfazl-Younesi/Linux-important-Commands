# 📌 Essential Linux Commands

A collection of important Linux commands is categorized for quick reference.

## 🚀 System Information & Monitoring

```bash
uname -a           # Show system information
hostname           # Display system hostname
uptime             # Show system uptime
whoami             # Show current user
who                # List logged-in users
top                # Display running processes
htop               # Interactive process viewer (requires installation)
ps aux             # List all running processes
free -h            # Show memory usage
df -h              # Show disk space usage
du -sh *           # Show disk usage per directory
vmstat 1           # Show system performance statistics
```

## 📂 File and Directory Management

```bash
ls -l              # List files with details
cd /path/to/dir    # Change directory
pwd                # Print current directory
mkdir newdir       # Create a new directory
rmdir mydir        # Remove an empty directory
rm -rf mydir       # Delete a directory and its contents
cp file1 file2     # Copy a file
mv file1 file2     # Move/rename a file
find / -name "file"  # Find a file by name
locate filename    # Quickly find a file (requires `mlocate` package)
```

## ✏️ File Viewing & Editing

```bash
cat file           # Display file content
tac file           # Display file content in reverse
less file          # View large files page by page
more file          # Similar to less but limited scrolling
nano file          # Edit a file in Nano editor
vim file           # Open a file in Vim editor
head -n 10 file    # Show first 10 lines of a file
tail -n 10 file    # Show last 10 lines of a file
tail -f logfile    # View live updates of a log file
```

## 👤 User Management

```bash
whoami             # Show current user
id                 # Show user ID and group ID
users              # List logged-in users
groups username    # Show groups of a user
sudo useradd newuser   # Add a new user
sudo passwd newuser    # Set a password for the new user
sudo usermod -aG sudo username  # Add user to sudo group
sudo deluser username   # Delete a user
```

## 🔐 Permissions & Ownership

```bash
ls -l              # Show file permissions
chmod 755 file     # Change file permissions
chmod -R 755 dir   # Change directory permissions recursively
chown user:group file  # Change file ownership
chown -R user:group dir  # Change directory ownership recursively
```

## 🌐 Networking & Internet

```bash
ping google.com        # Check network connectivity
curl -I google.com     # Fetch headers from a website
wget file-url          # Download a file
netstat -tulnp         # Show open network ports
ss -tulnp              # Modern alternative to netstat
ip a                  # Show IP addresses
nslookup google.com   # Get DNS info
traceroute google.com # Trace the path to a website
```

## ⚙️ Process Management

```bash
ps aux               # Show running processes
top                  # Monitor system processes
htop                 # Advanced process viewer (requires installation)
kill PID             # Kill a process by its PID
killall processname  # Kill all processes with a specific name
pkill processname    # Kill processes by name
bg                   # Resume a background job
fg                   # Bring background job to foreground
jobs                 # Show background jobs
```

## 📦 Package Management

### **Debian/Ubuntu (APT)**

```bash
sudo apt update          # Update package lists
sudo apt upgrade -y      # Upgrade all packages
sudo apt install package # Install a package
sudo apt remove package  # Remove a package
sudo apt autoremove -y   # Remove unused packages
```

### **RedHat/CentOS/Fedora (YUM/DNF)**

```bash
sudo yum update -y       # Update all packages (CentOS 7)
sudo dnf upgrade -y      # Update all packages (Fedora, CentOS 8+)
sudo yum install package # Install a package
sudo dnf remove package  # Remove a package
```

### **Arch Linux (Pacman)**

```bash
sudo pacman -Syu        # Update all packages
sudo pacman -S package  # Install a package
sudo pacman -R package  # Remove a package
```

## 💾 Disk Management

```bash
df -h                  # Show disk space usage
du -sh *               # Show space used by each directory
mount /dev/sdb1 /mnt   # Mount a disk
umount /mnt           # Unmount a disk
fdisk -l               # List partitions
lsblk                  # List block devices
```

## 📦 Compression & Archiving

```bash
tar -cvf archive.tar dir  # Create a tar archive
tar -xvf archive.tar      # Extract a tar archive
tar -czvf archive.tar.gz dir  # Create a compressed tar.gz archive
tar -xzvf archive.tar.gz  # Extract a tar.gz archive
zip -r archive.zip dir    # Create a zip file
unzip archive.zip         # Extract a zip file
```

## 🔄 System Shutdown & Reboot

```bash
shutdown -h now        # Shutdown the system immediately
shutdown -r now        # Reboot the system immediately
reboot                # Reboot system
poweroff              # Power off system
```

## 📢 Contributing

Feel free to fork this repo and submit pull requests with improvements or additional commands! 🚀

