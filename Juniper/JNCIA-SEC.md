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
