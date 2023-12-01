README outline:

What is HTTPS?
Definition: HTTPS (Hypertext Transfer Protocol Secure) is an internet communication protocol that protects the integrity and confidentiality of data between the user's computer and the site.
Use of SSL/TLS: Uses SSL (Secure Sockets Layer) or TLS (Transport Layer Security) to encrypt communications.
Importance: Essential for protecting sensitive transactions, such as online banking and shopping. It also secures browsing on public Wi-Fi networks.
The 2 Main Elements of SSL
Encryption:
Encrypts data transmitted over the network, making it unreadable to anyone who intercepts it.
Protects data integrity, preventing tampering during transmission.
Authentication:
Verifies the identity of the server to the user.
Uses digital certificates to ensure the server you're connecting to is legitimate.
HAProxy SSL Termination on Ubuntu 16.04
Definition of SSL Termination: The process of decrypting SSL/TLS encrypted traffic at the load balancer, allowing traffic to be unencrypted between the load balancer and backend servers.
Setting Up in HAProxy:
Install HAProxy.
Configure HAProxy to handle incoming SSL connections and forward them as regular HTTP requests to the backend servers.
Update the HAProxy configuration file (/etc/haproxy/haproxy.cfg) with SSL certificate details.
SSL Termination
Benefits:
Reduces CPU load on backend servers.
Centralizes SSL management at the load balancer.
Security Considerations:
Ensures encrypted transport outside the organization’s network.
Requires secure, trusted internal network as traffic between the load balancer and servers is unencrypted.
Bash Function
Usage: Automate and simplify SSL and HTTPS management tasks.
Example: Create a bash script to check SSL certificate expiration dates.
man or help: awk and dig
awk:
A powerful scripting language for text processing.
Example use: Parsing log files for SSL-related errors.
dig:
DNS lookup utility.
Use to verify that DNS records are correctly pointing to your HTTPS-enabled servers.
Learning Objectives
General Understanding:
Explain HTTPS and the dual role of SSL in providing encryption and authentication.
Understand the purpose of encrypting web traffic for security and privacy.
Explain SSL termination and its application in network architecture.
Practical Skills:
Configure HAProxy for SSL termination on Ubuntu 16.04.
Use awk and dig for managing and troubleshooting network configurations.
