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

+ Feedback should be analyzed at each stage of the process.
+ A goal is to make development, test, and production environments as identical as possible.
+ **Feedback : You need to gather feedback at all stages of production and delivery. Collect feedback from developers, operations, customers, and anyone else who may have information that can help you improve your flow or quality of product. A benefit of both Continuous Delivery and Continuous Deployment is that they contribute to making your development, test, and production environments as identical as possible.**

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

### NETCONF 
+ 830
+ **connections over SSH default port)** *

+ Java
+ Perl
+ **Feedback : JTAC supports both Java and Perl, and provides access to both on Juniper's website.**

### Junos automation
+ mgd
+ jsd
+ **Feedback : The processes most important to Junos automation are the management process (mgd) and JET service processes (jsd). The mgd process handles the automation requests involving the Junos XML API, YANG, the REST API, and some SNMP functions. The JET service process (jsd) handles automation requests that use the Juniper Extension Toolkit (JET) API.**



## XML/NETCONF

### on-box automation
+ Python
+ SLAX
+ **Feedback : Historically, XSLT and SLAX were the first languages specifically designed to work with the Junos XML API. Starting with Junos 16.1, Python can be used for the same task as well.**

### XML remote procedure call
+ router> show system name-resolution \| display xml rpc
+ **Feedback : You can determine the RPC by using the show interfaces ge-0/0/0 command with the \| display xml rpc command option at the end.**

### Programming Language
+ Python
+ Feedback : Python communicates with the Junos XML API both on-box and off-box.

### XML hierarchy
+ ```<example/>```
+ ```<example></example>```
+ Feedback : In some cases, there is no data to put between the opening and closing tags. In this case, you can combine the two tags into one using the shorthand notation.

### XML element nodes
+ An element node consists of everything between an opening and closing tag pair.
+ **Feedback : XML elements or everything within a matching start and end tag are represented as element nodes in a document object model.**

### XML document nodes
+ The document node is defined as the entire XML document.
+ **Feedback : The full XML document would be represented as a document node in a document object model.**

### NETCONF protocol
+ Messages
+ Transport
+ **Feedback : Messages and Transport are both layers of the NETCONF protocol.**
+ Operations
+ Content
+ **Feedback : Operations and Content are both layers of the NETCONF protocol.**

### gem install net-netconf command
+ Ruby
+ **Feedback : The gem install net-netconf command is used to install NETCONF for the Ruby programming language.**

### XPath

![](https://s3.amazonaws.com/crlearningpath/crcloud/assessment/1538677135815.png)
+ /configuration/interfaces/interface/unit/family/inet/address
+ **Feedback : You can specify the XML node you want to access by specifying each subhierarchy of XML, and separating them with a forward slash. This method is similar to the way you would specify multiple levels of subdirectories on a UNIX host.**

### Junos OS
+ Enable NETCONF using the set system services netconf ssh command.
+ **Feedback : To enable the Junos OS to accept NETCONF sessions on port 830, you need to issue the set system services netconf ssh command.**

## Data Serialization

### JSON
+ JSON is a lightweight data-interchange format; human-readable but easier for machines to parse.
+ **Feedback : JSON is a lightweight data-interchange format. JSON is human-readable, but easier for machines to parse.**
+ ```{"title": "The \"Big\" Router"}```
+ **Feedback : JSON strings can consist of any Unicode characters except for double quotes and backslashes. However, you can use double quotes and backslashes if you use the escape sequence first, so precede the characters to be escaped with a backslash as you would in C or Java.**

### JSON object
+ ```{```
+ **Feedback : JSON objects begin with and end with curly braces. A single object can contain a series of key-value pairs, separated by commas. An empty object (zero key-value pairs) is allowed. Keys in JSON are always of string type.**
![](https://s3.amazonaws.com/crlearningpath/crcloud/assessment/1538678731369.png)
+ JSON object
+ **Feedback : JSON objects begin with and end with curly braces. A single object can contain a series of key-value pairs, separated by commas.**

### JSON array
+ ```[```
+ **Feedback : An array in JSON is an ordered collection of values. Array structures begin and end with square brackets. Arrays contain zero, one or more values; array values are separated by commas.**

### JSON & YAML

+ JSON
+ YAML
+ **Feedback : JSON is a data serialization language most often used to move data between an Internet client and server. YAML is a Unicode-based data serialization language designed around common native data types found in agile programming languages.**
+ JSON uses a lowest common denominator model.
+ JSON is easier for a machine to parse than YAML.
+ **Feedback : JSON uses a lowest common denominator information model, ensuring any JSON data can be processed easily by every modern programming environment. YAML has simple-to-read files, but the language is more complex to generate and parse. In addition, YAML does not follow the lowest common denominator data types, and so requires more complex processing when crossing between different programming environments.**
+ All JSON data can convert to YAML data but not all YAML data can convert to JSON data.
+ **Feedback : JSON and YAML are similar enough that, in most cases, you can convert between the two languages. YAML, however, does not follow the lowest common denominator data types, and so requires more complex processing when crossing between different programming environments.**
+ JSON was designed for parsing speed over human readability.
+ YAML is designed around human readability over parsing speed.
+ **Feedback : Both JSON and YAML are human-readable. However, the foremost design goal of JSON is universality, so while the language is simple to generate and parse, there is a sacrifice of some human readability. In contrast, the highest priority of YAML is human readability and support for serializing arbitrary native data structures.**

### YAML mapping
+ ```hostname: router```
+ **Feedback : YAML mappings are sets of key-value pairs, equivalent to JSON objects.The keys and corresponding values are separated by a colon (:). In YAML, the strings do not require quotation marks.**

### YAML file
+  ```---```
+ **Feedback : Although not required, it is customary to start all YAML documents with three dashes ```---```.**

## Ansible

### command 
+ ansible-galaxy install Juniper.junos *
+ **install a Juniper Networks-created Ansible module**

### Ansible Galaxy module 
+ juniper_junos_rpc
+ **Feedback : Juniper junos rpc executes one or more RPCs and returns the result.**

### Junos Ansible modules
+ junos_rpc
+ junos_facts
+ **Feedback : "junos_rpc runs an arbitrary RPC over NetConf on a Junos device, and junos_facts collects facts from remote Junos devices."**

### Ansible inventory file
+ /etc/ansible/hosts
+ **default path including the default file name of the Ansible inventory file**

### Ansible host file
![](https://s3.amazonaws.com/crlearningpath/crcloud/assessment/1538679420996.png)
+ router1 and router2 are included in the routers group.
+ **Feedback : You can place different hosts in groups, using square bracket syntax. For example, you might want to differentiate by device family (such as srx, mx, ex).**

### playbook
+ YAML
+ **Feedback : Ansible playbooks are written in YAML and carry out the tasks defined in Python modules.**

![](https://s3.amazonaws.com/crlearningpath/crcloud/assessment/1538679503383.png)
+ The host variable must be defined in the inventory file.
+ The Juniper.junos modules will be executed locally on the control device.
+ **Feedback : Contained within this play are the requirements that the host variable must be defined in the inventory file and that the Juniper.junos modules will be executed locally on the control device.**

![](https://s3.amazonaws.com/crlearningpath/crcloud/assessment/1538679761631.png)
+ Ansible playbook
+ YAML file
+ **Feedback : A playbook contains one or more plays. A play is essentially a set of hosts and a set of tasks that must be performed on the hosts. The playbook file is formatted in YAML.**

![](https://s3.amazonaws.com/crlearningpath/crcloud/assessment/1538679885474.png)
+ 2
+ **Feedback : This play executes two tasks. Each task calls a module; junos_get facts and debug in this example.**

### Ansible & Junos device
+ Ansible uses NETCONF over SSH sessions.
+ Ansible requires all tasks to execute locally on the control server.
+ **Feedback : Ansible modulse are executed locally and connect using NETCONF over SSH to Junos devices, performing operations on them as needed.**
+ Ansible modules are executed on the control server.
+ **Feedback : The Juniper implementation of Ansible requires all tasks to run locally on the Ansible control server.**

## Python or PyEZ

### Python
+ to comment
+ **Feedback : Python uses the # symbol to indicate comments (alternatively, three quotes before and after the block of code might be used to indicate a multi-line comment).**

### Python operator
+ bitwise *
+ **The & and | characters represent bitwise**
+ The variables are compared to determine if they have the same value.
+ **Feedback : The == operator can be used determine if two variables contain equal values.**

### Python dictionary
+ It is identifiable by curly brackets ({}).
+ It is an unordered collection of key-value pairs.
+ **Feedback : A dictionary is an unordered collection of key, value-pairs and is identifiable by curly brackets ({}).**

### Python tuple
+ ```t = ("Juniper", "Junos", "MX")```
+ **Feedback : Tuples use parentheses instead of square brackets.**

### PyEZ
+ Python
+ **Feedback : PyEZ is a microframework used to operate Junos using Python. A microframework is a package or library that provides code that is useful for a larger application.**
+ PyEZ exception handling
+ **Feedback : These are examples of exceptions that PyEZ can catch.**
+ **ConnectAuthError, ConnectTimeout, and ConnectError**
+ Telnet
+ NETCONF over SSH
+ **Feedback : PyEZ can use a NETCONF over SSH, Telnet, or Serial Console connection to a Junos device.**

### PyEZ utils module
+ config *
+ **to write a PyEZ script that will modify the Junos configuration**

### PyEZ Python script
![](https://s3.amazonaws.com/crlearningpath/crcloud/assessment/1538680670475.png)
+ The script attempts to establish a NETCONF session to connect to the device.
+ The login is established outside of the operation of this script.
+ **Feedback : NETCONF is the default method of connecting to the device. Login is established with SSH.**

### Python interactive interpreter (shell)
+ ```bash$ python```
+ **Feedback : You can start the Python interactive interpreter, sometimes called the Python shell, just by typing python at the command prompt (sometimes you want to run a specific Python version, in this case you can type python2.7 for Python 2.7 or similarly for other versions).**

## REST API

### Advantage
+ The REST API uses simple tools that allow for fast prototyping.
+ Most programming languages include libraries for the REST API.
+ **Feedback : The REST API can be accessed using any program or programming language capable of generating HTTP requests. For a quick test, a Web browser (possibly with a suitable plugin), tools like Postman, or just the curl command line utility can be used. For actual programming, libraries have been developed for many languages that simplify the generation of REST API requests (such as the requests package for Python).**
+ REST
+ **Feedback : The Junos REST API enables Junos OS devices to participate in REST management system environments, allowing for the execution of Junos RPCs. Additionallly, the REST API provides GUI API explorer functionality.**

### communicate with a Junos device
+ REST
+ **Feedback : Typically, REST uses HTTP(S), and any object accessible from the API corresponds to a unique URL on the server.**
+ lighttpd
+ **Feedback : The lighttpd server terminates HTTP(S) connection and passes request to the request to the mod_juise plugin.**

### Port
+ 3000 *
+ **default HTTP port that is used by the REST API to connect to a Junos device**
+ You must enable the REST API Explorer tool and connect to the Junos device using the Explorer's default port of 3443.
+ **Feedback : To enable the REST API Explorer, issue the set system services rest enable-explorer configuration mode command. After you commit the configuration, navigate in a browser to the host name or IP address of your Junos device, appending the configured port number after the colon. The default port number is 3000 for HTTP and 3443 for HTTPS.**

### Protocol
+ IPv4 only
+ **Feedback : The Junos OS REST API currently only works with IPv4 transport.**
+ ```protocol://device:port/rpc/procedure```
+ **Feedback : protocol://device:port/rpc/procedure is a valid example of an HTTP GET method.**

### daemon
+ mgd
+ **Feedback : When a request is made, last daemon that would process the request is the mgd daemon. The MGD returns the data back to JUISE, which reformats the data for the lighttpd web server, which then passes the response back to the REST client.**