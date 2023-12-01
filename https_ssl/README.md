What is HTTPS?
HTTPS (Hypertext Transfer Protocol Secure) is an internet communication protocol that protects the integrity and confidentiality of data between the user's computer and the site. It is the secure version of HTTP, the protocol over which data is sent between your browser and the website you are connected to.

Key Aspects:
Data Encryption: This means that while the user is browsing a website, nobody can "listen" to their conversations, track their activities across multiple pages, or steal their information.
Data Integrity: Data cannot be tampered with or corrupted during transfer, intentionally or otherwise, without being detected.
Authentication: Proves that your users communicate with the intended website. It protects against man-in-the-middle attacks and builds user trust, which translates into other business benefits.
The 2 Main Elements that SSL Provides
SSL (Secure Sockets Layer), now commonly referred to as TLS (Transport Layer Security), provides two main security elements:

Encryption: It keeps the data exchanged on the internet private and secure. When data is sent or received over the internet, SSL ensures it's encrypted, making it unreadable to everyone except the intended recipient.

Authentication and Trust: SSL provides authentication to a website. It verifies that the server you're connected to is actually the correct server. This is done using SSL certificates which are issued by Certificate Authorities (CAs). This helps users trust that they are in fact communicating with the actual website they intended to.

HAProxy SSL Termination on Ubuntu 16.04
SSL Termination refers to the process of terminating the SSL encryption at a load balancer or server, instead of at the web server. This can improve performance and manage SSL certificates in a centralized location.

HAProxy SSL Termination
HAProxy can be configured to perform SSL termination, which means it will handle the SSL encryption and decryption, offloading this task from the web servers.
To set up SSL termination with HAProxy on Ubuntu 16.04, you typically need to:
Install HAProxy.
Obtain an SSL certificate and configure HAProxy to use it.
Configure HAProxy to listen on HTTPS and forward decrypted traffic to your web servers.
SSL Termination
SSL Termination is the process of decrypting SSL/TLS encrypted traffic at an intermediary device, such as a load balancer, before passing it along to the web servers.

Benefits:
Reduces the load on web servers.
Simplifies SSL certificate management.
Can provide better performance for end users.
Bash Function
A bash function is a set of commands in a shell script grouped together. Functions are used to encapsulate a group of commands so they can be reused in the script.
