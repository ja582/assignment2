# Linux 
## What is Linux
Linux is a family of open-source and free operating systems built on the Linux kernel, by Linus Torvalds. 
Linux is built upon UNIX.
UNIX was an operating system back in the 60s and 70s used by programmers and employees. It was written in Assembly Language by AT&T.
The interesting key to UNIX was that it was portable and light enough to be ran on most computers, big or small. 
Due to an anti-trust suite that forbid AT&T to enter the software business, it would license out the source code of UNIX to other users and academic circles.
Overtime, UNIX became a standard rather than a used operating system. An operating system like macOS is defined as UNIX by its standards.
Linux is a derivative of UNIX. It was created to circumvent the proprietary UNIX, which is still trademarked.
Linux operating systems are allowed to be freely distributed, modified, and ran. 
One of the most popular versions of Linux is Ubuntu. 

You can look more into Ubuntu here:  [Ubuntu.com](https://www.ubuntu.com/)

## Some Linux Terminal Commands
Linux comes with a program known as the "terminal shell".
It allows you to manipulate and change files in the system with text commands.

1. `ls`
    - `ls` is a command that lists all contents in a directory. 
    - To simply use `ls`, type it into the linux terminal and use the following commands below for more options.
    
   
  A table of `ls` commands
   
 | option       | usage          | 
 | ------------- |:-------------:|
 | ls -a      | List all files including hidden files starting with a '.' |
 | ls -d | List directories.      |
 | ls -i | List the files's inode index number.   |
 | ls -l | List files with their permissions.    |
 | ls -la | List files and with the hidden files.     |
 | ls -lh | List files by long format with a readable file size.     |
 | ls -ls | List the files with long format and with file size .   |
 | ls -r | List files in a reverse order.      |
 | ls -s | Sort files by file size     |
 | ls -S | Sort by the file size      |
 | ls -t | Sort by the time & the date      |
 | ls -x | Sort the files by the extension name.     |
 
 2. `cd`
    - `cd` command allows the user to change the directory inside the Linux shell, allowing easy navigation. 
    - To use it properly, you must type `cd <directory>`. 
    
Example:    
![cd desktop](/img/cdDesktop.png)

To go to any other directory, just type something after `cd`.

### The vi Editor
The vi editor in Linux is a built in text-editor in the terminal shell. 

To start it up, do `vi <Filename>`. 


![opened file in vi](/img/viOpen.png)

From here you can use the keys on your keyboard:

`'h' to move one character to the left`

`'j' to move down character`

`'k' to move up one character`

`'l' to move one character to the right`


To edit a file, simply press `i` on your keyboard and write like so:

![edited file in vi](/img/viEdit.png)
  
Once you are done, simply press the `ESC` key and type `:wq` in the terminal to save and close your work.

## File Protocols and Permissions

### File Protocols and SSH

To transfer files to a computer (a local) to a server (a remote), you'll be using 2 file transfer protocols: FTP, and SFTP.

- **FTP** is the standard file transfer protocol. It is used to transfer a file from the local to the remote. 
FTP clients provide this functionality. It usually runs over TCP port 21 or 20. It has been around since the 1970s. 
It is less secure.

- **SFTP** is a completely different file transfer protocol, compared to FTP. 
SFTP functions the same as FTP, but instead it runs over an SSH session allowing it to be more secure. 
Uses TCP port 22.

- **SSH** is a network protocol for operating networks that allow services to connect securely over an unsecured network. 
Typical used in command-line applications that allow a user to securely send files from a local that may contain sensitive information to a sensitive remote.
Has strong encryption and provides several alternative options for strong authentication. 


### File Permissions
File permissions are what allows a user and computer to do to a file. Some files may only let you read, write, and execute. 
Sometimes a combination of the two.  

To read file permissions please us this image:

![file permissions table](/img/file_permissions.png)

A table of the most commonly used permission values:

| chmod value       | Definition          | 
 | ------------- |:-------------:|
 | 777      | (rwxrwxrwx) No permissions. You can do anything. |
 | 755| (rwxr-xr-x) The owner of the file may read, write, and execute the file. All other users can only read and execute.     |
 | 700 | (rwx------) The owner of the file may read, write, and execute. Nobody else can do anything to it. Useful for files that you want to use, keep private from other users.   |
 | 666 | (rw-rw-rw-) Any user may read and write to the file.    |
 | 644 | (rw-r--r--) The owner of the file may read and write a file. Other users may only read it.     |
 | 600 | (rw-------) The owner may read and write to the file. Nobody else has rights.    |

To simply change file permissions in terminal, simple type:

`chmod <value> file_name.extenstion`

An example:

![file permission changed](/img/chmod.png)
     
  
 