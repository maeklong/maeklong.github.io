# Design, Associate (JNCDA)
# (JN0-1101)

## Customer Design Requirements

### Network Design
+ You should understand the state of the customer's current network.
+ You should analyze current and future network behavior.
+ **Feedback : When designing a network for a customer you should always understand the state of the customers current network. You should also analyze the current and future network behavior of the customer's network.**

### Juniper lifecycle service
+ Operate
+ Plan
+ Build
+ **Feedback : The three phases of Juniper's lifecycle service approach are plan, build, and operate.**

### the plan methodology
+ Access
+ Design
+ **Feedback : The two sub-phases of the plan methodology are access and design.**

### key RFP elements
+ Business requirements
+ Environmental requirements
+ **Feedback : The business and environmental requirements are key RFP elements.**

### business continuity RFP element
????

### environmental requirements RFP element
+ A detailed report that describes the facility specifications.
+ The number of users and workstation requirements.
+ **Feedback : The environmental requirements RFP element includes a detailed report that describes the facility specifications and the number of users and workstation requirements.**

### The connectivity and throughput requirements RFP element
+ Number of wireless connections needed
+ Traffic analysis
+ **Feedback : The modular requirements RFP element includes the number of wireless connections that are needed and a in-depth traffic analysis.**

### aspects of greenfield projects
+ New networks with few or no restraints to consider.
+ Next-generation networks created from the ground up.
+ **Feedback : Greenfield projects typically involve a new network in which legacy and existing applications do not need to be considered.**

### categories that customer requirements
+ Security
+ Availability
+ **Feedback : The six categories are security, availability, scalability, manageability, and performance**
+ Performance
+ Scalability
+ Manageability
+ **Feedback : The six categories are security, availability, scalability, manageability, and performance.**

### design proposals
+ You should keep your design proposal as simple as possible.
+ You should create the logical design before the physical design.
+ **Feedback : You should keep your design proposal as simple as possible. You should create the logical design before creating the physical design.**
+ Security should be considered throughout the design process.
+ You design proposal should be clearly documented.
+ **Feedback : Security should be considered at every step of the design proposal.**

### modularity in your network design
+ Modularity facilitates future growth and troubleshooting efforts.
+ Modularity provides hierarchical structure to your design.
+ **Feedback : Modularity is important because it helps with future growth and troubleshooting efforts as well as giving a hierarchical structure to your design.**

## Customer Organizational Structure

### business continuity
+ The prevention of interruption to mission-critical services.
+ The ability to reestablish full functionality quickly after a disaster.
+ **Feedback : Business continuity should involve prevention and recovery methods that are proactive. Reactive measures such as manually turning on a backup server, or manually loading backed up data are reactive disaster recovery methods.**

### business continuity planning
+ test the plan
+ formulate the plan
+ **Feedback : The steps of business continuity planning are, know your network, assess the risks, formulate the plan, and test the plan.**

### Know Your Network step
+ You should list all the functions and services in the network.
+ You should perform a business impact analysis.
+ **Feedback : In the Know Your Network step of the business continuity planning you should list all the functions and services of the network and perform a business impact analysis.**

### Assess the Risks step
+ You should perform a risk assessment.
+ **Feedback : In the Assess the Risks step of business continuity planning you should perform a risk assessment.**

### Formulate the Plan step
+ You should develop a plan of action to mitigate the risks.
+ **Feedback : In the Formulate the Plan step of business continuity planning you should develop a plan of action to mitigate the risks.**

### RFP response
+ Executive summary
+ A solution overview
+ technical specifications
+ **Feedback : An RFP response should include an executive summary, a solution overview, and technical specifications.**

### executive summary section
+ It is likely to be read by all decision makers.
+ It is an overview of Juniper's value proposition to the customer.
+ **Feedback : The executive summary section of an RFP is so important because it is likely to be read by all decision makers and it contains an overview of Juniper's value proposition to the customer.**
+ Identification of business benefits.
+ **Feedback : The steps of the Juniper recommended executive summary structure in an RFP are: Introduction of the customer's need or problem, identification of business benefits, overview of your proposed solution, and relevant supporting information outlining why the customer should choose your plan.**
+ Focus on organizational issues.
+ Keep it short and simple.
+ **Feedback : When writing an excutive summary of an RFP, you should give focus on the organizational issues of the customer and keep it short and simple. You should avoid a history of Juniper Networks and canned responses.**

### technical specifications section
+ It should contain the logical and physical topology design requirements.
+ It should contain the bill of materials.
+ **Feedback : The technical specifications section of an RFP should contain the logical and physical topology design requirements. It should also contain the bill of materials.**

### network design checklist
+ A process for understanding the customer's business and technical goals.
+ **Feedback : The first four steps of the recommended network design checklist are: A process for understanding the customer's business and technical goals, a validation process for analyzing customer's existing environment, the steps for designing a network topology, and a process for selecting protocols, address schemes, naming conventions, and so forth.**
+ The steps for designing a network topology
+ **???***
+  A process for selecting protocols, address schemes, naming conventions, and so forth.
+ **Feedback : The first four steps of the recommended network design checklist are: A process for understanding the customer's business and technical goals, a validation process for analyzing customer's existing environment, the steps for designing a network topology, and a process for selecting protocols, address schemes, naming conventions, and so forth.**

## Physical Design Considerations

### highly resilient network
+ Virtual Chassis for EX devices.
+ Redundant power supplies for network devices.
+ **Feedback : Virtual chassis for EX devices and redundant power supplies in network devices helps ensure that the network is highly resilient.**
+ Stateful failover for firewall platforms.
+ Chassis clusters for firewall platforms.
+ **Feedback : Stateful failover and chassis clusters for firewall platforms helps ensure that the network is highly resilient.**

### backup WAN link
+ When the users in the network rely on communication through VoIP.
+ When the cost of a second link is less than the cost of downtime.
+ **Feedback : You should add a backup WAN link when the users in the network rely on communication through VoIP and when the cost of a second link is less than the cost of the downtime. Note that you cannot combine both WAN link into a LAG to increase throughput because the backup WAN link is with a different provider.**

### physical device redundancy
+ When zero impact to users and applications is required during device failures.
+ When downtime is not acceptable for device upgrades.
+ **Feedback : You should add physical device redundancy to your network design when zero impact to users and applications is required during device failures and when downtime is not acceptable for device upgrades.**

### redundant power supplies are plugged into a single power source
+ The power redundancy requirements are not met as the single source of power could fail and the network devices will not stay powered on.
+ The redundant power supplies should be plugged into separate power sources.
+ **Feedback : Redundant power supplies should always be plugged into separate power sources. If both power supplies are plugged into the same power source, then the failure of the power source will bring down the network device.**

### VRRP
+ open standards protocol
+ provides redundancy through a virtual IP address
+ **Feedback : VRRP is an open standards protocol and provides redundancy through the use of a virtual IP address.**
+ The VRRP members can contain two different routing platforms.
+ **Feedback : VRRP do not need any special connections between the members. VRRP is an open standards protocol, which means the routing platforms can be different.**
+ The maximum number of routing devices in a VRRP group is two
+ **????**

### chassis cluster
+ The SRX model numbers must be the same to form a chassis cluster.
+ **Feedback : A chassis cluster must contain the same SRX models. Attempting to cluster an SRX340 and a SRX345 together will not work.**
+ The chassis cluster uses a fabric link between the two nodes.
+ The chassis cluster nodes can be located in different cities.
+ **Feedback : To form a chassis cluster you must use a fabric link between the two nodes and the two nodes can be located in different cities.**

### campus redundancy best practices
+ You must include highly available redundant connections for all applications in your design.
+ You need to include hardware redundancy in your design.
+ **Feedback : In campus redundancy, you must ensure that there is high availability for all applications and hardware redundancy must be part of your design.**
+ You need to include network redundancy in your design.
+ You need to include redundant wireless access points in your design.
+ **Feedback : In campus redundancy, you must ensure that there is network redundancy and redundant wireless access points in your design.**

### distance between the Ethernet switches
+ 100 meters
+ **???***

## Logical Design Considerations

### size and scope of a new network design
+ The number of users is important.
+ The type of devices is important.
+ **Feedback : When determining the size and scope of a new network design you should consider the number of users and the type of devices that will be accessing the network.**

### capacity and scaling of systems for a campus switching design
+ The average number of wireless devices that will be connecting to the network.
+ The average bandwidth usage of users.
+ **Feedback : When determining the capacity and scaling of systems in a campus design you should consider the average number of wireless devices that will be connecting to the network and the average bandwidth usage for the users.**

### large campus building with many users who are in different department
+ VLAN
+ **Feedback : The VLAN technology should be used to separate the users within different departments.**

### different groups must be tightly restricted
+ A Layer 4 firewall
+ **Feedback : You should use a firewall to restrict between the different groups.**

### redundant WAN links
+ **Feedback : Redundant WAN links can address the connectivity issue as a single WAN link could be flapping and causing the connectivity issues.**

### hub-and-spoke VPN
+ **Replace the hub-and-spoke VPN with an ADVPN.
Feedback : Deploying an ADVPN removes the hub device from the forwarding path in spoke-to-spoke communication. Full-meshed VPN does not work in this situation because of the management overhead a full mesh VPN places on the IT staff that has recently seen cutbacks.**

### SSL VPN
+ **Feedback : SSL VPNs allow remote home workers to access corporate resources securely.**
+ **allows remote home workers to access resources at the corporate headquarters securely**

### Junos Space
+ Network Director
+ **Feedback : The Network Director application can be used to manage VLANs on EX devices.**
+ Security Director: Logging and Reporting
+ **Feedback : You can use the Security Director: Logging and Reporting application to store and management events for SRX devices.**
+ Junos Space typically uses the eth0 interface to manage devices through the OOB network.
+ Junos Space typically uses the eth3 interface to manage devices through the in-band network.
+ **Feedback : Junos Space can use the eth0 and eth3 interface to manage devices. Typically the eth0 interface on a Junos Space device is used to manage devices through the OOB network. Typically the eth3 interface on a Junos Space device is used to manage devices through the in-band network.**
+ Connectivity Services Director
+ **Feedback : The Connectivity Services Director application can be used to manage L3 VPNs on MX devices.**

### Junos Space Security Director
+ centralized
+ **Feedback : The Junos Space Security Director application is a centralized management solution.**

### disaster recovery
+ Deploying a Data Center Interconnect.
+ **Feedback : Deploying a Data Center Interconnect between two data centers would ensure that the customer is completely prepared for a disaster recovery scenario.**

### Virtual Chassis
+ **Feedback : There is no need for STP with a virtual chassis.**

### virtual chassis fabric (VCF)
+ VCF uses a spine-and-leaf architecture.
+ Each connected host in a data center is no more than two hops away from every other host in a data center.
+ **Feedback : A VCF uses a spine-and-leaf architecture and each connected host is no more than two hops away from any other host.**

+ GRE
+ EVPN
+ **Feedback : You can use GRE and EVPN to stretch L2 traffic between two data centers over the DCI.**

## Industry Alternatives
+ VPLS
+ VRRP
+ **Feedback : VPLS and VRRP are open source protocols that can work with multiple different vendors.**

+ RSVP
+ LDP
+ **Feedback : VPLS and VRRP are open source protocols that can work with multiple different vendors.**

+ ISIS
+ LACP
+ **Feedback : ISIS and LACP are open source protocols that can work with multiple different vendors.**

### data-interchange format
+ JSON
+ **Feedback : You can use JSON to automate Junos OS platforms.**

### automate Junos OS platforms
+ PyEZ
+ **Feedback : You can use PyEZ to automate Junos OS platforms.**

### Junos operational scripts
+ A Junos operational script can be executed manually.
+ A Junos operational script can be executed automatically when a user logs in.
+ **Feedback : A Junos operational script can be executed manually in the CLI and when a user logs in.**

### Junos event policies
+ An event policy uses if-then-else logic.
+ You can execute Junos OS operational command for the action of an event policy.
+ **Feedback : Junos event policies use if-then-else logic and you can excute operational commands for the action of an event policy.**

### Junos event scripts
+ Junos event scripts are triggered automatically.
+ Junos event scripts can be used to monitor the overall status of the device.
+ **Feedback : Junos event scripts are triggered automatically and can be used to monitor the overall status of the device.**