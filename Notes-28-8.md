What is public Ip?

A public IP (Internet Protocol) address is a unique number assigned to a device, connected to a computer network. This address allows devices to identify and communicate with each other across the internet. Public IPs are globally unique and are used to facilitate communication between devices on different networks, such as servers, routers, and individual devices like computers and smartphones.



what is private Ip?

 which are used within local networks to identify devices. These private IPs are not routable on the public internet and are typically used for communication within a local network, while a router or network gateway handles the translation between private and public IPs when data leaves the local network.

Monolithic vs Microservices
----------------------------------------------------

Monolithic Architecture:
-----------------------------
In a monolithic architecture, the entire application is built as a single unit. All components and functionalities of the application, such as user interfaces, business logic, and databases, are tightly integrated into a single codebase. This approach was common in traditional software development.

Advantages of Monolithic Architecture:

Simplicity in development and deployment.
Easier to maintain when the application is small.
Shared resources and code can lead to better performance in certain cases.

Disadvantages of Monolithic Architecture:

Scaling can be challenging, as the entire application needs to be scaled even if only one component requires more resources.
Development bottlenecks can occur as the codebase grows, making it harder for larger teams to work efficiently.
Updates or changes to one part of the application might require rebuilding and redeploying the entire monolith.

Microservices Architecture:
-----------------------------------
In a microservices architecture, an application is broken down into a collection of small, loosely coupled services that are independently deployable and manageable. Each service is responsible for a specific business capability and communicates with other services through well-defined APIs. These services can be developed, deployed, and scaled independently.

Advantages of Microservices Architecture:

Scalability is more efficient, as resources can be allocated to specific services that require them.
Independent development and deployment of services enable teams to work on different parts of the application simultaneously.
Easier technology adoption and maintenance, as services can be developed using different languages or technologies.
Fault isolation: If one service fails, it doesn't necessarily affect the entire application.

Disadvantages of Microservices Architecture:

Increased complexity in terms of communication between services and managing a distributed system.
Requires robust service discovery, load balancing, and monitoring mechanisms.
Testing and deployment can be more complex due to the distributed nature of the application.
Overhead in terms of inter-service communication and infrastructure management.

Choosing between monolithic and microservices architectures depends on factors such as the complexity of the application, the size of the development team, the required scalability, and the overall development and operational capabilities of the organization. While monolithic architectures can be simpler to start with, microservices can offer more flexibility and scalability as applications grow and evolve. However, adopting microservices also introduces additional challenges that need to be carefully considered and addressed.


How internet works?

The internet is a global network of interconnected computers and devices that communicate with each other using a standardized set of protocols and technologies. Here's a simplified overview of how the internet works:

1. **Devices and Computers:**
   The internet is composed of countless devices such as computers, servers, routers, smartphones, and more. Each of these devices is assigned a unique address called an IP (Internet Protocol) address, which is used to identify and locate them on the network.

2. **Data Transmission:**
   When you send data over the internet, it's broken down into smaller units called packets. These packets contain both the data being transmitted and control information like the source and destination IP addresses. This packet-based approach enables efficient and reliable data transmission.

3. **Routers and Switches:**
   Routers and switches are devices that play a critical role in directing data packets to their intended destinations. Routers determine the best path for a packet to travel from the source to the destination, and they make this decision based on the IP addresses in the packets.

4. **IP Addresses and DNS:**
   IP addresses are used to identify devices on the internet. When you type a website's domain name (e.g., www.example.com) into your browser, a Domain Name System (DNS) server translates that human-readable domain name into the corresponding IP address of the server hosting the website. This allows your device to connect to the correct server.

5. **Protocols:**
   Protocols are a set of rules and conventions that govern how data is formatted, transmitted, and received across the internet. One of the most important protocols is the TCP/IP (Transmission Control Protocol/Internet Protocol) suite. TCP ensures that data is reliably transmitted between devices, while IP handles addressing and routing.

6. **HTTP and Web Browsing:**
   The Hypertext Transfer Protocol (HTTP) is used for transferring web pages and other resources over the internet. When you enter a URL in your web browser, it sends an HTTP request to the server hosting the website. The server responds with the requested content, and your browser displays it.

7. **Encryption and Security:**
   To ensure privacy and security while transmitting sensitive information, protocols like HTTPS (HTTP Secure) use encryption to encode the data being sent between your device and the server. This prevents unauthorized parties from intercepting and understanding the data.

8. **Firewalls and Security Measures:**
   Firewalls are used to protect networks and devices from unauthorized access and potential cyber threats. They monitor and control incoming and outgoing network traffic based on predefined security rules.

9. **Content Distribution and Cloud Services:**
   Content delivery networks (CDNs) and cloud services play a role in distributing content efficiently. CDNs store copies of popular content in multiple locations, reducing the distance data needs to travel and improving loading times.

Overall, the internet is a complex network of interconnected devices, protocols, and technologies that work together to enable communication, data sharing, and access to online services and resources across the globe.


------------------------------------------------------------------------------------------------------------------------------------------------

Till 1995 we had only public IP. Then NAT comes into the picture.

before 1995 ISP were giving ipv4 address directly to laptop.

Private IP will be allocated by Modem at our home network

In office environments these will be allocated by LAN Network.

NAT --> Network Address Translation

Advantages of using Private IP:

Latency  - The response will be quick.
Security - It will not travel through the internet and will reside inside our network.

Humans can remember the names like wise systems can understand the IP addresses.

To maintain these IP addresses we have DNS.

DNS ( Domain Name System) - It has the IP addresses of the top level domains.

When we are browsing ISP is responsible to provide the IP of the domain.

These information ISP will fetch from DNS servers.

AAround the Globe these DNS servers were located at 13 places.

All the ISP providers will have common exchange point.

Monolithic vs Micro services
---------------------------------

In Monolithic, the application is big(It doesn't have multiple components)
A simple change also need to be deployed again
Maintainaance is big headache
Scalling issues

In Microservices, the applicaation is divided into multiple components.
communication happens through API's.
Fronend always calls backend through API calls, Backend will send data in JSON format and images.

Firewall
---------------
Inbound --> traffic coming to your server
	source: internet i.e any server outside
	destination: your Ec2 instance
Outbound --> traffic going out from your server
	source: your EC2 server
	destination: whatever you want to send
	
only port no 80 and 22 are allowed, 
0.0.0.0/0 --> everybody on the internet

