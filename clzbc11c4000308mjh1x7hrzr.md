---
title: "My Journey with Basic Bash Commands in WSL Ubuntu"
datePublished: Thu Aug 01 2024 13:49:19 GMT+0000 (Coordinated Universal Time)
cuid: clzbc11c4000308mjh1x7hrzr
slug: my-journey-with-basic-bash-commands-in-wsl-ubuntu
tags: ubuntu, linux, basics, commands, wsl2, wsl-2, wsl-ubuntu

---

As I delved into the world of Linux through the Windows Subsystem for Linux (WSL), I quickly realized how essential it was to familiarize myself with terminal commands. Here's a collection of the commands I’ve used, along with explanations for each, which helped me navigate and manage my system effectively.

## 1\. Managing WSL

* `wsl -l -v`:
    
    * Lists installed WSL distributions with their version.
        
    * Example: Check which Linux distributions are available and their status.
        
* `wsl --version`:
    
    * Displays the version of WSL you are using.
        
    * Useful for ensuring you have the latest features.
        
* `wsl --update`:
    
    * Updates WSL to the latest version.
        
    * Important for accessing the latest features and improvements.
        
* `wsl --list --verbose`:
    
    * Similar to `wsl -l -v`, it lists installed distributions with additional information.
        
* `wsl -d Ubuntu`:
    
    * Launches the Ubuntu distribution in WSL.
        
    * Essential for starting your Linux environment.
        

## 2\. Exploring the File System

* `pwd`:
    
    * Prints the current working directory.
        
    * Use this command to know your location in the file system.
        
    * `pwd`
        
* `ls`:
    
    * Lists files and directories in the current directory.
        
    * You can add options like `-l` for a detailed view.
        
    * `ls`
        
* `lsblk`:
    
    * Lists block devices (like hard drives and partitions) and their mount points.
        
    * Useful for checking disk space and mounted drives.
        
* `cd`:
    
    * Changes the directory.
        
    * For example, `cd Desktop` moves you to the Desktop directory.
        
    * `cd ..` to come out of directory
        
* `mkdir demo`:
    
    * Creates a new directory named `demo`.
        
    * Use this to organize your files.
        

## 3\. Managing Files

* `touch demo.js`:
    
    * Creates an empty file named `demo.js`.
        
    * You can use it to create new files quickly.
        
* `cat demo.txt`:
    
    * Displays the contents of `demo.txt`.
        
    * Useful for quickly viewing file content without opening an editor.
        
* `mv demo.txt demo`:
    
    * Moves `demo.txt` into the `demo` directory.
        
    * This command is also used to rename files.
        
* `rm demo.js`:
    
    * Deletes the file `demo.js`.
        
    * Use with caution, as it permanently removes the file.
        

## 4\. Editing Files with `vi`

* `vi demo.txt`:
    
    * Opens `demo.txt` in the `vi` text editor.
        
    * If the file does not exist, it will create a new one.
        

### Basic `vi` Commands

1. **Enter Insert Mode**:
    
    * Press `i` to start adding text.
        
2. **Exit Insert Mode**:
    
    * Press `Esc` to return to Normal mode.
        
3. **Save Changes and Exit**:
    
    * Type `:wq` and press Enter to save changes and exit.
        
4. **Save Without Exiting**:
    
    * Type `:w` to save your changes.
        
5. **Exit Without Saving**:
    
    * Type `:q!` to exit without saving any changes.
        

## 5\. Installing and Updating Software

* `sudo apt-get update`:
    
    * Updates the package list for upgrades.
        
    * Always run this before installing new software to ensure you have the latest versions.
        
* `sudo apt install wsl`:
    
    * Installs WSL if it’s not already installed.
        
    * You might not need to run this if you’re already using WSL.
        

## 6\. System Information

* `lsb_release -a`:
    
    * Displays Linux distribution information, such as version and codename.
        
    * Helpful for identifying your OS version.
        
* `htop`:
    
    * Launches an interactive process viewer.
        
    * Great for monitoring system resource usage.
        
* `ip a`:
    
    * Displays network interface information.
        
    * Useful for checking IP addresses and network configurations.
        

## 7\. Command History

* `history`:
    
    * Displays a list of previously executed commands.
        
    * You can use this to review your command usage or re-run commands easily.