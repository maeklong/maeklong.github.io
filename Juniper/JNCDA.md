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
