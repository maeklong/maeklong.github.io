# Cloud, Associate (JNCIA-Cloud)
# (JN0-211)

## Cloud Architectures

### Software Suites
+ OpenStack
+ vSphere
+ Kubernetes
+ **Feedback : OpenStack, vSphere, and Kubernetes are used in different roles in cloud architectures.**

### Secure VPN Technology
+ IPsec VPN
+ **Feedback : Access to private cloud environments is through private leased connections, or over the Internet through secure VPN access. IPsec VPN encrypts and hashes traffic as it traverses the putlic Internet.**

### Layer 2 Loop Prevention Protocols
+ MC-LAG
+ LACP
+ **Feedback : MC-LAG and LACP provide link and device redundancy without the need for Spanning Tree Protocol (STP)**

### VXLAN Tunnel
+ EVPN
+ **Feedback : Some of the most common tunneling technologies are MPLS over GRE and VXLAN, where EVPN is used to establish and maintain VXLAN tunnels.**

### SaaS
+ SaaS
+ **Feedback : Software as a Service, or SaaS, abstracts the underlying hardware and software configuration and focuses on providing application access to an end customer.**
+ **to deploy a website that can scale as needed**

### PaaS
+ PaaS
+ **Feedback : Platform as a Service, or PaaS, goes one step beyond IaaS by providing a requested operating system on which applications can be installed.**
+ **Type of service would allow you to provision five servers with Windows Server 2016 installed**

### Underlay Network
+ BGP
+ **Feedback : The scalability of Layer 3 protocols, especially with regards to BGP, is much higher than Layer 2 technologies, and can scale from tens of thousands to hundreds of thousands of host devices.**
+ IP Address
+ **Feedback : The underlay network does not have visibility into the tunneled customer data traffic. The underlay network routes data based on packet IP addressing.**

### Data Center Underlay Network
+ spine network device redundancy
+ fast failover
+ **Feedback : Redundancy and high availability are two key properties of a robust underlay network.**

### Private Cloud
+ Resources are dedicated to your organization.
+ Resources are accessed through a private connection.
+ **Feedback : Resources are not shared among multiple tenants, and access to the resources are through a private connection, as opposed to a general public connection.**
+ A private cloud has dedicated resources for individual customers.
+ A private cloud can be deployed in a service provider network.
+ **Feedback : Private cloud deployments allocate dedicated resources to an organization that are not shared among multiple tenants. Access to private cloud environments is through private leased connections, or over the Internet through secure VPN access. Unlike a public cloud deployment, only secure, authorized access to the resources is available.**
+ to protect sensitive data
+ to provide cloud-based services within an organization
+ **Feedback : With a private cloud, an organization retains control of the data and applications within the cloud environment. Often this is done to restrict access to sensitive information, or for internal security reasons. A private cloud within an organization often provides services to other business units or departments within the organization.**

### VMware NSX
+ QFX Series **
+ **Feedback : VMware NSX Layer 2 gateway services will be available on Juniper Networks QFX Series access switches, EX9200 line of programmable core/aggregation Ethernet switches, and MX Series 3D Universal Edge Routers. Deployed as a Virtual Tunnel End Point, or VTEP, each platform registers with VMware’s NSX controller and can be configured to provide Layer 2 gateway services to any virtual network. This allows the NSX controller to coordinate the creation of VXLAN tunnels between the hypervisor and the phy**

### Automation Script
+ vMX Series
+ MX Series
+ **Feedback : Included in Junos OS, the Junos Automation Toolkit is a suite of tools supported on all Juniper Networks switches, routers, and security devices.**

### ETSI Management and Orchestration (MANO) framework
+ virtualized network function manager (VNFM)
+ Network Functions Virtualization (NFV) orchestrator
+ **Feedback : Two of the key components of the ETSI NFV architectural framework are the NFV Orchestrator and VNF Manager, known as NFV MANO. Additional layers, such as service orchestration are also required for operators to enable true NFV services. Open Source software can facilitate the implementation of an ETSI aligned NFV architecture, provide practical and essential feedback to the ETSI ISG NFV and increase the likelihood of interoperability among NFV implementations.**