# Security, Associate (JNCIA-SEC)
# (JN0-230)


## SRX Series Devices

### Mini-Physical Interface Modules (Mini-PIMs) on an SRX Series Services Gateway
+ DOCSIS
+ Serial
+ 1-Port Gigabit Ethernet Small Form-Factor Pluggable (SFP)
+ **Feedback : The SRX Series Services Gateways support the following Mini-Physical Interface Modules: 1-Port Small Form-Factor Pluggable (SFP), 1-Port Gigabit Ethernet Small Form-Factor Pluggable (SFP), ADSL2+, DOCSIS, G.SHDSL, Serial, T1/E1, and VDSL2.**
+ **are supported Mini-Physical Interface Modules (Mini-PIMs) on an SRX Series Services Gateways**

### PoE Support
+ SRX320
+ SRX650
+ **Feedback : PoE is supported on the SRX210, SRX240, SRX320, SRX550, and SRX650 devices.**

### default configuration on an SRX300
+ an untrust security zone
+ a DHCP client on ge-0/0/0
+ **Feedback : A default configuration includes two security zones (trust and untrust) as well as setting a DHCP client for interfaces ge-0/0/0 and ge0/0/7.**

### match criteria (to determine if a flow already exists for a packet)
+ source port
+ unique session token number for a given zone and virtual router
+ protocol
+ **Feedback : To determine if a flow exists for a packet, the NPU attempts to match the packet’s information to that of an existing session based on the following match criteria: source address, destination address, source port, destination port, protocol, and unique session token number for a given zone and virtual router**

### match criteria (options are available to be performed on the traffic)
+ permit
+ reject
+ deny
+ **Feedback : A set of actions to be performed in case of a match—permit, deny, or reject.**
+ **When traffic has met match criteria, what options are available to be performed on the traffic**

### Hypervisor Support
+ Hyper-V
+ KVM
+ **Feedback : VMware ESXi is also a supported hypervisor.**
+ **vSRX is available for**

## Junos Security Objects

### Services
+ screens
+ **Feedback : Regardless if the packet is matched or not, the next service to inspect the packet are screens.**
+ zones
+ policy
+ **Feedback : Screens and services ALGs are applied to both fast-path and first-packet processing.**
+ **services does fast-path processing skip**

### Addressing
+ 192.168.0.7/255.255.0.255
+ **Feedback : The wildcard mask determines which of the bits in the IP address A.B.C.D should be ignored. For example, the source IP address 192.168.0.11/255.255.0.255 in a security policy implies that the security policy match criteria can discard the third octet in the IP address (conventionally represented as 192.168.*.11).**
+ **wildcard address for an address book entry**

### Zone
+ zone
+ **Feedback : A zone is a collection of one or more network segments sharing identical security requirements. To group network segments within a zone, you must assign logical interfaces from the device to a zone.**
+ **security component is a collection of one of more network segments sharing identical security requirements**

## Security Policies

### Policy
+ policy
+ **Feedback : Security policies enforce a set of rules for transit traffic, identifying which traffic can pass through the firewall and the actions taken on the traffic as it passes through the firewall. Security policies allow you to decide which users and data can enter and exit the network, as well as where, when, and how**
+ **a set of rules that tells a Junos security device how to treat transit traffic**
+ zone policies, global policies, default policy
+ **Feedback : The Junos OS evaluates traffic against security policies in a specific order. Once a rule that matches traffic has been found, the specified action is taken and policy evaluation ends. Policies are checked in the following order: zone policies, global policies, and the default policy.**
+ **order do Junos security devices examine policies for transit traffic**

### Policy Rule Ordering
+ Rules with more specific match criteria should be listed higher.
+ By default, new rules go to the end of the list.
+ **Feedback : Ordering is important. Rules with more specific match criteria should be listed higher in the order with all new rules (by default) go to the end of the list.**
+ **considering security policy rule ordering**

### security policy components
+ user-defined address object
+ application
+ **Feedback : Each security policy must contain a matching source address, destination address, and application.**

### unified security policies
+ A unified policy can be a global-based policy.
+ A unified policy can be a zone-based policy.
+ **Feedback : You can use both zone security policies and global security policies at the same time within a configuration. However, zone security policies are checked first before global policies.**

## Sky Advanced Threat Prevention

### GeoIP feature of Sky ATP
+ GeoIP uses dynamic address entries.
+ The SRX Series device needs connectivity with the Sky ATP cloud for GeoIP to function properly.
+ **Feedback : The GeoIP feature uses dyanamic address entries and the SRX needs connectivity to the Sky ATP cloud for GeoIP to function properly.**

### C&C threat prevention feature of Sky ATP
+ C&C threat prevention stops compromised hosts in your network from communicating with known C&C servers.
+ C&C threat prevention can stop hosts in your network from unwillingly participating in a DDoS attack.
+ **Feedback : C&C treat prevention stops your hosts from communicating with known C&C servers and stops hosts in your network from unwillingly participating in DDoS attacks.**

### E-mail protection of Sky ATP 
+ Sky ATP e-mail protection inspects SMTP traffic.
+ Sky ATP e-mail protection inspects IMAP traffic.
+ **Feedback : Sky ATP e-mail protection includes the SMTP and IMAP protocols.**

### HTTP file inspection
+ HTTP file inspection
+ **Feedback : Files downloaded from a webserver use HTTP and Sky ATP HTTP file inspection should be used to protect against malicious file transfer in this situation.**
+ **to protect against malicious files that might be download through Web-based e-mail**

## Network Address Translation

### Interface-based NAT
+ Interface-based NAT uses the outbound interface IP address to translate the source address of outgoing packets.
+ **Feedback : All packets subject to translation have their source IP address translated to the IP address on the egress interface. PAT is required to tell sessions from different hosts apart and is always enabled.**

### NAT & PAT
+ both first path and fast path processing
+ **Feedback : A Junos security device implements NAT and PAT in both first path and fast path processing. Note that destination NAT and source NAT occur separately in the first path packet flow.**
+ **When does a Junos security device implement NAT**

### Type of NAT
+ static
+ **Bidirectional initiation of translation is classified as which type of NAT**

### Types of source NAT
+ interface-based
+ pool-based
+ **Feedback : Interface-based source NAT: All packets subject to translation have their source IP address translated to the IP address on the egress interface. PAT is required to tell sessions from different hosts apart and is always enabled. Pool-based NAT: A dynamic mapping of the original source address to an address from a user-defined pool. This can be used with or without PAT.**


## IPsec

### Secure VPNs
+ integrity
+ source authentication
+ confidentiality
+ **Feedback : Three major security concerns exist for network security are integrity, source authentication, and confidentiality.**

### IPsec VPN tunnel
+ the VPN Wizard
+ **In the J-Web user interface, which feature is used to facilitate building IPsec VPN tunnels**

### IDs
+ proxy IDs
+ **You are configuring an SRX Series device to inter-operate with a third-party IPsec VPN endpoint that uses policies to create the VPN. In this scenario, what must be configured for the VPN to work**

### HMAC
+ pre-shared key must be known by both sides
+ adds a pre-shared key (PSK) to the hashing process
+ validates data integrity and verifies that the data came from the proper source
+ **Feedback : One method is to perform source authentication by using a Hashed Message Authentication Code (HMAC). The sender appends a secret preshared key to the data, then performs the hash function. For hashes to successfully match, the receiver must append the same key value to the data before performing the hash function. The key itself never transmits along with the data.**
+ **Hashed Message Authentication Code (HMAC) is a source authentication method based on which three procedures**
## Unified Threat Management

### Junos flow module services
+ interface I/O, security policy, TCP proxy, application proxy
+ **Feedback : As traffic travels inbound on an interface of the SRX Series device, security policies process the traffic. If the security policy contains a UTM policy, a TCP proxy is used to process the matching traffic. The TCP proxy is used for both a TCP client and TCP server, to terminate and originate a TCP session. The TCP proxy feeds the data stream to the application proxy.**
+ **the correct order for processing UTM traffic within the Junos flow module services**

### application control policies
+ Deploy a vSRX with the AppSecure suite in AWS and configure the AppFW.
+ **Feedback : Application Firewall (AppFW) refers to the ability to take the results from the App ID engine and leverage them to make an informed decision to permit, deny/ reject, or redirect the traffic.**
+ **A security administrator wants to deploy application control policies to allow or deny traffic based on dynamic applications in the organization's Amazon Web Services (AWS) deployment**

