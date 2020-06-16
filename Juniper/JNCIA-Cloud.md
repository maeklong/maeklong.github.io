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
+ **two platforms share the same automation scripts**

### vMX
+ The vMX Series uses carrier-grade routing optimized for the x86 environment.
+ The vMX Series requires a license for production environments.
+ **Feedback : The vMX Virtual Router is a virtualized MX Series 3D Universal Edge Router that helps network operators of all types improve customer experience and profitability by increasing network and service agility and accelerating time to market for new services, while streamlining their operations environment. The vMX is available as licensed software for x86-based servers and on Amazon Web Services (AWS) and AWS GovCloud, where it can provide secure routing between AWS virtual path connections (VPCs),**

### vMX on KVM
+ a little (lite)
+ performance
+ **Feedback : vMX can be configured to run in two modes depending on the use case. Lite mode—Needs fewer resources in terms of CPU and memory to run at lower bandwidth. Performance mode—Needs higher resources in terms of CPU and memory to run at higher bandwidth.**

### Public Cloud
+ vMX
+ vSRX
+ **Feedback : The virtual SRX platform, or vSRX, is a virtualized version of the Juniper Networks SRX security gateway platform. It retains the same software components and functions as its hardware counterpart, with separate control and forwarding planes. It runs on a Juniper Linux guest OS, which can be installed on a Hypervisor as a virtual machine. Like the vSRX, the vMX has a virtualized control plane and a virtualized forwarding plane, which run separately. Unlike the vSRX, not only are these two compon**
+ ** Juniper Networks virtualized products are available for use in the public cloud**

### ETSI Management and Orchestration (MANO) framework
+ virtualized network function manager (VNFM)
+ Network Functions Virtualization (NFV) orchestrator
+ **Feedback : Two of the key components of the ETSI NFV architectural framework are the NFV Orchestrator and VNF Manager, known as NFV MANO. Additional layers, such as service orchestration are also required for operators to enable true NFV services. Open Source software can facilitate the implementation of an ETSI aligned NFV architecture, provide practical and essential feedback to the ETSI ISG NFV and increase the likelihood of interoperability among NFV implementations.**

### Service Scaling
+ **Feedback : Service scaling increases instances of an application providing scalability for important resources.**
+ **Whenever an application becomes popular, the resulting high-traffic load on the VNFs leads to user dissatisfaction**

### VNF
+ A VNF is a virtual entity that can be launched and managed.
+ **Feedback : Virtualized network functions (VNFs) include all virtual entities that can be launched and managed from the Juniper Device Manager (JDM)**

### NFV containers
+ NFV containers usually provide fewer functions than VM-based VNFs.
+ **Feedback : With container architecture, many services and functions of the original operating system are lost, as the operating system is no longer deployed with the services. The key focus of this software structure is to enable the desired services without the overhead of deploying a platform that provides a suite of services that may not be used. This introduces the concept of microservices. With microservices, resource requirements on the underlying host are greatly reduced, as are deployment times and**

### VNFs and NFV
+ VNFs include all virtual entities that can be launched and managed from the Juniper Device Manager.
+ NFV incorporates cloud and virtualization technologies to drive new network services with elastic scale and automation.
+ **Feedback : Virtualized network functions (VNFs) include all virtual entities that can be launched and managed from the Juniper Device Manager (JDM).**

### Network Service Activator
+ **Feedback : Network Activator initially provisions NFX250 Network Services Platforms (referred to as remote devices in this documentation), which reside at end users’ sites. The remote devices download a boot image and initial configuration files from servers hosting Network Activator, using a process that provides full authorization and authentication for all interactions. When initial provisioning is complete, the remote device communicates with a management server, which then starts to manage and monitor**

## SDN

### SDN controller
+ An SDN controller centralizes control and configuration of a network.
+ An SDN controller automates repetitive tasks in a network.
+ **Feedback : The Virtual Networking and SDN layer is where central policy, control, and automation of networking above the hardware or fabric layers takes place. Software Defined Networking operates on the network at the virtualized network and services level. An SDN controller has a different role than an orchestration platform. The primary role of an SDN controller is to automate repetitive tasks in a network environment.**

### OpenStack component
+ Keystone
+ **Feedback : Keystone provides identity management in an OpenStack environment. Users, applications, and API calls are all considered virtual users, and each requires authentication and authorization to access OpenStack services. Each API call is authenticated against the identity management system to ensure that the entity that is requesting a service is authorized.**
+ **OpenStack component is responsible for user authentication and authorization**

### OpenFlow controller-based software defined network
+ The forwarding plane of each device in the network is programmed by the controller.
+ **Feedback : In an OpenFlow network, all of the forwarding elements are directly programmable allowing switching decisions to be made centrally. This means forwarding policy no longer needs to be configured on individual devices and the hop-by-hop behavior can be abstracted and configuration can be made based on the desired network state.**

### VMware NSX controller and a Junos Layer 2 gateway
+ OVSDB
+ **Feedback : The management of the virtual switch is achieved via the OVS DataBase (OVSDB). The database contains information such as the set of logical switches that the OVS must handle, the list of associated physical ports, as well as configuration information as statistics for those ports. The Layer 2 gateway runs an OVSDB server. Typically,a local client and a client on the controller clusters connect to this server. Using OVSDB, the controller cluster can thus coordinate different parameters across the**

### vSRX Series and VMware NSX integration
+ You can add the vSRX virtual firewall as a security element in the VMware NSX environment.
+ **???**

### Junos Space application 
+ Network Director
+ **Feedback : Juniper provides a single pane-of-glass management solution with Junos Space Network Director, which manages both physical and virtual networking environments while integrating with management tools from Vmware. When virtual machines move from one location in the data center to another, Network Director is immediately aware of this change. In this way, a network administrator can now change the VLAN configurations on the virtual and physical switches.**

### Compute Hypervisor
+ ESXi
+ KVM
+ **Feedback : Typically, the servers running Contrail components are using the Linux operating system and a KVM hypervisor. As of Contrail Release 2.0 and greater, limited capability is provided for extending the Contrail compute node functionality to servers running the VMware ESXi virtualization platform.**

### Opensource Management Framework
+ OVSDB
+ **Feedback : Some Juniper Networks devices support Virtual Extensible LAN (VXLAN) and the Open vSwitch Database (OVSDB) management protocol. Support for VXLAN and OVSDB enables the Juniper Networks devices in a physical network to be integrated into a virtual network.**

### Deploying vSRX
+ Junos Space Security Director
+ VMware NSX Manager
+ **Feedback : The vSRX VM is deployed in conjunction with Juniper Networks Junos Space Security Director and VMware NSX Manager.**

### SDN Type
+ OpenFlow-based SDN
+ **Feedback : While the definition of SDN has been stretched over time, the original concept and its implementations based on the OpenFlow protocol remain. Often referred to as “Classic” or “Pure” SDN, the idea is to strip SDN down to its simplest form: the total separation of control and forwarding planes. The control plane is centralized in the SDN controller, while the forwarding plane remains distributed in a simplified forwarding element.**

### Contrail
+ private cloud networking
+ Network Functions Virtualization
+ **Feedback : Contrail, and the open source release of OpenContrail, is an open source SDN controller that integrates with OpenStack. It uses APIs to interact with the native OpenStack components, and places a Juniper Networks virtual router on each host in the network. The virtual router serves as the end point for the network overlay tunnels that interconnect physical hosts, and that connect physical hosts to gateway devices.**

## SDN WAN

### SDN WAN implementation
+ SDN WAN uses MPLS tunnels to connect POPs.
+ SDN WAN uses a centralized control plane.
+ **Feedback : The SDN WAN provides a centralized control plane for MPLS domains. The NorthStar Controller is a WAN SDN controller that automates the discovery and creation of traffic-engineered label switched paths across a service provider or large enterprise network.**

### NorthStar Controller
+ NorthStar
+ **Which SDN product is used to manage and optimize MPLS WAN connections?**
+ It is an SDN WAN controller.
+ **Which statement describes the role of the NorthStar Controller**
+ PCEP
+ **Feedback : Juniper Networks® NorthStar Controller is based on the Path Computation Element (PCE)architecture as defined in RFC 5440. It specifically leverages the “active stateful PCE” concept, which enables it to learn about the network and LSP path state via the Path Computation Element Protocol (PCEP) by communication with a client-side component present in the network devices themselves. The client is referred to as a Path Computation Client (PCC).**
+ RSVP-TE
+ **Feedback : The path setup is performed through RSVP-TE signaling, which is enabled in the network and allows labels to be assigned from an ingress router to the egress router.**
+ PCE
+ PCC
+ **Feedback : PCE: Path Computational Element. This component computes paths through the network and can apply constraints during the computation of those paths.The NorthStar controller performs this role. PCC: Path Computation Client. A path computation client is a software application that requests a path.**

### WANDL constructs topologies
+ Enters data manually.
+ Imports configuration files.
+ **Feedback : Device configuration files and saved command output information is imported into the server to create a model. Manual data file creation, which is more time-consuming, requires using a text editor to manually create the data files.**
+ SNMP
+ **Feedback : The WANDL IP/MPLSView server connects to production devices using SSH or telnet, and gathers information and statistics using CLI commands and SNMP polling.**
+ **SNMP does WANDL use to collect live network information**

## Cloud Monitoring

### Juniper Telemetry Interface
+ OpenConfig data model
+ **What is a supported data model for the Juniper Telemetry Interface**

### big data analytics and machine learning
+ AppFormix
+ **Feedback : AppFormix redefines state-of-the-art telemetry and management across software-defined infrastructure and application software layers, delivering realtime and historic monitoring, performance visibility, and dynamic optimization features to improve cloud orchestration, security, accounting, and planning for users.**

### transport monitoring data
+ UDP
+ **Which protocol is used to transport monitoring data in Juniper's open and extensible data model**