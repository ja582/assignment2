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

#### chmod
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

`chmod <value> file_name.extension`

An example:

![file permission changed](/img/chmod.png)
   
  
 #### chown
chown is similar to chmod except it will fix file ownership on an entire directory or a file.

To simply use chown, type `chown <user_name> *<file extension>` in terminal to set all the said file extension to a user on the system's name.

# 

#How Internet Works by Hanna Yafremava



![example](/img/pic2.jpg) 


## **DNS** (Domain Name System) - it maintains a directory of domain names and translates them to Internet Protocol (IP) addresses.
## **IP** (Internet Protocol)-  unique number for every machine using the internet (computer, phone, router, etc.) 
##  This unique number is written as a string of numbers separated by periods. 
##  There are two standards for IP addresses: IP Version 4 (IPv4) and IP Version 6 (IPv6).
##  IP address helps all internet devices to connect, find, send, and exchange information with other internet devices. 
## **Domain Name** - readable form of IP address and the part of a network address that identifies it as belonging to a particular domain (website). Example: www.example.com.
## **Top Level Domains (TLD)** - the last part of the domain name. The TLD is the letters immediately following the final dot in an Internet address. 
## (Example: .org, .com. .edu, etc.)   
## Examples and meaning of TLD
## .edu       Educational organization (most US universities)
## .k12       US school site (not all US schools use this)
## .ac         Academic institution (outside of US)
## .sch        School site (some schools outside of the US use this)
## .com       Company (usually .co in the UK)
## .org        Any organization
## .gov       Government agency
## .net        Network
## .mil        Military institution
   
   ![example](/img/pic1.jpg)
   

## ****How to read web address:**** 
## Each page on the internet has a unique address that is identified by the URL. URL - Uniform Resource Locator.
## Knowing what each of the basic elements are in a URL will help to identify the type of website and its purpose.
## Example: _http://www.njit.edu_
## 1. http - HyperText Transfer Protocol - The website is a hypertext document.  
## Hypertext is a nonlinear system of writing that allows users to access text and multimedia features through multiple pathways.
## 2. www - World Wide Web - Website that is on the World Wide Web. 
## WWW - an information space where documents and other web resources are identified by Uniform Resource Locators, which may be interlinked by hypertext, and are accessible over the Internet.
## 3. njit is Domain Name - identifies and calls up the specific computer on the Web that stores the information you requested. 
## 4. .edu is TLD - Indicates the type of source for a web site.


## Second example:
   
   ![example](/img/pic3.png)


## **HTTP and HTTPS**

## **How a web server can respond to requests through HTTP:**
## Web browsers and servers communicate via TCP/IP. 
## Hypertext Transfer Protocol (HTTP) is the standard application protocol on top of TCP/IP supporting web browser requests and server responses.
## Also, web browsers use DNS to work with URLs.
## These protocol standards help different brands of web browsers to communicate with different brands of web servers without requiring special logic for each combination.
## In addition, web browser and server connections normally run through a series of intermediate network routers
## _Steps of a basic web browsing session:_
## 1.The user specifies a URL in their browser
## 2.The browser initiates a TCP connection to the web server or server pool (using port 80 by default) via its IP address as published in DNS. 
## As part of this process, the browser also makes DNS lookup requests to convert the URL to an IP address.
## 3. After the server completes acknowledgment of its side of the TCP connection, the browser sends HTTP requests to the server to retrieve the content.
## 4. After the server replies with content for the page, the browser retrieves it from the HTTP packets and displays it accordingly.



## **HTTPS** 

## Hyper Text Transfer Protocol Secure (HTTPS) - a protocol for securing the communication between two systems, the browser and the web server.
`![alt text](image location)`
![example](/img/https-communication.jpg) 

## Secure Sockets Layer (SSL) - a protocol which creates a secure connection over a computer network.
## The latest version of SSL is called Transport Layer Security (TLS)

## **Difference Between HTTP and HTTPS**
## 1. HTTP - Unsecured information exchange protocol / HTTPS - Secured information exchange protocol
## 2. HTTP sends data over port 80 and HTTPS uses port 443
## 3. HTTPS transfers data in encrypted format while HTTP transfers data in hypertext format.
## 4. HTTP works at the application layer, while HTTPS works at the transport layer
## 5. HTTP URL starts with HTTP:// , and the HTTPS URL starts with HTTPS://











##Sources: http://www.networksolutions.com/support/what-is-a-domain-name-server-dns-and-how-does-it-work/
##https://www.awordtothewiseandcommonsense.com/how-to-read-a-url.html
##https://en.wikipedia.org/wiki/World_Wide_Web
##https://www.lifewire.com/web-browsers-and-web-servers-communicate-817764
##https://www.tutorialsteacher.com/https/what-is-https
##https://www.webinspector.com/blog/website-security-check/what-is-https-and-why-switching-to-https/
##https://visual.ly/community/infographic/computers/how-internet-works-0