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