# Automation and DevOps, Associate (JNCIA-DevOps)

## Junos Automation Stack and DevOps Concepts

### Continuous Delivery
+ Continuous Delivery is required for Continuous Deployment.
+ Continuous Delivery means that software is deployed on demand when there is a new software build.
+ **Feedback : Continuous Delivery ensures code is ready to deploy at any time (with actual deploy not necessarily happening in a fully automated way), and Continuous Deployment includes the stage of automated deployment.**

### The waterfall model of software development
+ One phase of development must be completed before the next phase can start.
+ This method lacks flexibility.
+ **Feedback : With the waterfall model, the next phase only starts after finishing the previous one. When requirements change and a need to develop new functionality appears, the waterfall model shows its weakness. It is not flexible enough and requires a lot of time before new functionality can be brought to production.**

### Manifesto of Agile Software Development
+ Customer collaboration is preferred over contract negotiations.
+ Working software is preferred over comprehensive documentation.
+ **Feedback : The “Manifesto” formulated the main values of Agile as follows: individuals and interactions over processes and tools; working software over comprehensive documentation; customer collaboration over contract negotiation; and responding to change over following a plan.**

### DevOps
+ DevOps is a methodology used to develop software or systems.
+ DevOps is a methodology that allows for frequent, quick modifications.
+ **Feedback : DevOps is a combination of technologies, design concepts, mentalities, and ideals that enable high performing IT teams to move fast while maintaining stability. DevOps creates a tight loop of product release and feedback. With DevOps, changes in functionality happen frequently and are moved to production fast.**

+ to lower cost
+ to improve quality
+ **Feedback : Among other advantages, DevOps gives you consistency, security, stability and reliability, all of which contribute to increased speed, decreased cost of management per device, and decreased number of configuration errors.**

### Infrastructure as Code workflow
+ Code > Version Control > Code Review > Integrate > Deploy
+ **Feedback : A typical IaC workflow is as follows: the device code is created and then stored in a version control system; next, the device code goes through an automated code review process; it is then integrated back into the master code branch; and finallay is deployed out to the network device.**

### Automation Tools (require an agent)
+ Chef
+ Puppet
+ **Feedback : To use Puppet with Junos devices, you need to install the jpuppet module on the Junos device. Similarly, to use Chef for Junos OS, the Chef client must first be installed on the Junos device.**

### NETCONF connections over SSH (default port) *
+ 830