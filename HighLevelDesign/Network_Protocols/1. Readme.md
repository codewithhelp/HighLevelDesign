# Network Protocols
* Set of rules to enable communication between machines

## Application Protocols - **Clint Server**
```
Client makes request, and Server provides response
```

### HTTP 
### FTP - 2 Connections (Control connection, Data connection)

### SMTP (Simple Mail Transfer Protocol)
* Sending mail
### IMAP (Internet Message Access Protocol)
* Reaceiving mails from server and can access from multiple clients

### Web Sockets - Bi-Directional communication
* messaging app

---
## Application Protocols - **Peer to Peer**
```
Each node connects to each other
```
### WebRTC (Uses UDP/IP)
* live streaming & video calls



----


## **Transport Protocols**
## TCP/IP (Transmission control protocol)
* Handshake: client sends sync, server sends sync/ack, then client send ack to server
* client divides the messages into fragments and attach sequence number and sends to server, it maintains the order of packets
* ackowledge of each package
* maintains the connection
* **Disadvantages** Slow as compared to UDP, as it requires to maintain order, ack each message and maintains order
* **Advantage**: Reliable

## UDP/IP (User datagram protocol)
* No Handshake
* No order of packets
* no ackowledge of each package
* Very fast.


### Telnet  - Remote terminal connection



## HTTP vs HTTPS
HTTP: sends data in pain text
HTTPs:  
* sends data in encypted form
* uses internally TLS

HTTPs Steps
* step1: tcp handshake :  tcp ack, tcp ack/sync, tcp ack
* step2: certificate check : asynmetric encryption (public/private key)
* step3: key exchange : session key exchange
* step4: encrypted data transmission