# assignment2

#How Internet Works 


`![alt text](image location)`
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
   ![alt text](image location)`
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
   ![alt text](image location)`
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
