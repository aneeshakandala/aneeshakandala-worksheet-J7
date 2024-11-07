## 1. What is inside a packet?
A packet has a header and a payload. The header stores the address of where to send the packet, and then the paylod stores the data or messgage. 

## 2. What is the purpose of an internet layer in the TCP/IP protocol? What do you, as a client, need to specify in this protocol?
The purpose of an internet layer is to interconnect networks; it describes the protocols for how networks connect with each other and the way that computers are identified. A client would haev to specify the destination IP address in order to send the data to the specified network location. 


## 3. What is the purpose of the transport layer in the TCP/IP protocol? What do you, as a client, need to specify in this protocol?
The purpose of the transport layer is to provide an abstraction for two processed running to appear as if they are able to directly communicate with each other. Additionally, the transport layer provdes ports (a mechanism) to differentiate communication that is for one process to another. A client would have to give the destination port number for this protcol to occur. 


## 4. What is the difference between SMTP and HTTP?
An SMPT is used to trasmit email messages and an HTTP is used to downlod web content/transmit information between a client and web server. 


## 5. What is the difference between an IP address and a domain name?
An IP address is the numerical identifier of a device on the internet while a domain name can be used to identify a networked device. Internet does not function on domain names, instead it functions off of IP addresses. 


## 6. How does the operating system use ports?
An operating system uses ports to divide up the data arriving from the network based on the destination process. There is also a relationship between ports and applications. 


## 7. Write code that creates a socket connection to ip address 123.45.678.900 at port 4040. Then, print a color to that socket’s output.
```
Socket sock = null;
sock = new Socket("123.45.678.900", 4040);
PrintWriter pw = new PrintWriter(sock.getOutputStream());
pw.println("blue");
pw.close();
sock.close();
```


## 8. What is the difference between a socket’s input stream and its output stream?
A socket's input stream reads data from the source, while output stram writes data. 


## 9. What is the difference between a Socket and a SocketServer?
The socket is connected to the server at an ipaddress or host and port-- a single connection. A server socket can accept more connections from other client sockets. 


## 10. How are threads useful with servers? How does a server manage to always be listening for sockets trying to connect?
Threads are useful because they allow for a singular server/core to execute multiple processes simultaneously. 
because a threaded socket starts a new thread for each threads so that the main thread can continue to listen to incoming connections 


