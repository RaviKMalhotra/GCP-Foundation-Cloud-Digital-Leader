# Belos is a list of all Networking Servicse in the GCP cloud
- Virtual Private Cloud -
- Cloud Load Balancing -
- Cloud CDN -
- Cloud DNS -
- Cloud Interconnect -
- Cloud VPN -
- Network Connectivity Center -
- Firewall Rules -
- Packet Mirroring -
- Private Google Access -
  Virtual Private Cloud (VPC): Create logically isolated networks for your resources.

- 1. Cloud Load Balancing: Distribute traffic across multiple instances to ensure high availability.
2. Cloud CDN (Content Delivery Network): Deliver content to users with low latency.
3. Cloud DNS: Scalable, reliable, and managed domain name system service.
4. Cloud Interconnect: Connect your on-premises network to GCP with high bandwidth.
5. Cloud VPN: Securely connect your on-premises network to your GCP VPC.
6. Network Connectivity Center: Centralized hub for managing network connectivity.
7. Traffic Director: Managed service mesh for load balancing and traffic management.
8. Network Intelligence Center: Monitor, troubleshoot, and optimize your network.
9. Firewall Rules: Control traffic to and from your instances.
10. Packet Mirroring: Capture and inspect network traffic for analysis.
11. Private Google Access: Access Google services from your VPC without using public IPs.
- 


# VPC in GCP
1. VPC network is a global resource with regional subnets.
2. By regional subnets, that means the subnet should belong to any of the desired region (geographical location).
3. Each VPC is logically isolated from each other.
4. You can create multiple VPCs as per the business requirements.
5. you cannot connect from a VM in one VPC to the other VM in the second VPC by default.
6. connectivity can be established between multiple VPCs using different services and techniques which we will explore in next topics.
7. 2 or more VPCs can be connected together using VPC peering.
8. Subnets can acts as either private or public subnets depending on the routing defined.
9. Firewall rules can be configured to allow or restrcit traffic within subnets.
10. Resources wtihin a VPC communicate via the standard IPv4 addresses, and there is a dedicated DNS service within the VPC to provide name resolution.


# Load Balancers in GCP
official documentation link --  [GCP Load Balancing documentation](https://cloud.google.com/load-balancing/docs/load-balancing-overview)

## What is Load Balancing?
Load balancing is the process of distributing incoming network traffic across multiple backend resources to ensure no single resource is overwhelmed. This helps improve the availability and reliability of your applications.

## Types of Load Balancers in GCP
GCP offers several types of load balancers, each designed for different use cases:

### 1. HTTP(S) Load Balancer:

Layer: Layer 7 (Application Layer)
Use Case: Distributes HTTP and HTTPS traffic to backend services.
Features: Global load balancing, SSL termination, URL-based routing, and more.

### 2. TCP/SSL Proxy Load Balancer:

Layer: Layer 4 (Transport Layer)
Use Case: Distributes TCP and SSL traffic.
Features: Global load balancing, SSL termination, and more.

### 3. Internal TCP/UDP Load Balancer:

Layer: Layer 4 (Transport Layer)
Use Case: Distributes TCP and UDP traffic within a VPC.
Features: Regional load balancing, high performance, and more.

### 4. Network Load Balancer: 

Layer: Layer 4 (Transport Layer)
Use Case: Distributes TCP, UDP, and other IP-based traffic.
Features: Global load balancing, direct server return, and more.

## Load Balancing Key Features

- Single Anycast IP: A single IP address is used for all backend instances, simplifying DNS management and providing a consistent 
  endpoint for clients1.
- Autoscaling: Automatically adjusts the number of backend instances based on traffic load, ensuring optimal performance and cost-efficiency1.
- Health Checks: Regularly monitors the health of backend instances and routes traffic only to healthy instances1.
- Global and Regional Load Balancing: Supports both global and regional load balancing, allowing you to distribute traffic across 
  multiple regions or within a single region

## Load Balancing Benefits

High Availability: Ensures your applications remain available even during high traffic periods or instance failures.
Scalability: Seamlessly scales your applications to handle varying traffic loads.
Security: Provides features like SSL termination and DDoS protection to secure your applications.

### Load Balancing Use Cases
Web Applications: Distribute HTTP(S) traffic across multiple instances to ensure high availability and performance.
APIs: Load balance API requests to backend services for better reliability and scalability.
Internal Applications: Use internal load balancers to distribute traffic within your VPC for internal applications and services.

1. Load Balancers are capable of distributing the traffic evenly across multiple GCE compute engines (VMs) in a single or multiple region.
2. Why you need a Load Balancer? There are many different use cases of having a LB in your network infrastructure. let's try to understand few of them.
  - Imagine you have a Windows Server which you want your outside Internet users to be able to connect. In this case rather than assigning the public IP address directly to the virtual machine, what you can do is, you can create a public load balancer, and map the windows VM behind the LB.
3. 
12. 
