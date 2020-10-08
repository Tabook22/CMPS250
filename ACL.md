### ACL
A network access control list (ACL), is an extra layer of security, that acts as a firewall for controlling and filtering traffic in and out of one or more subnets (e.g., router and layer 3 switche).<br>
we can think about it as set of rules defined for controlling the network traffic and reducing network attack<br>

---

Once the access-list is built, then it should be applied to inbound or outbound of the interface:

* Inbound access lists – When an access list is applied on inbound packets of the interface then first the packets will processed according to the access list and then routed to the outbound interface.
* Outbound access lists – When an access list is applied on outbound packets of the interface then first the packet will be routed and then processed at the outbound interface.


---
There are two types of ACL:
* standard access lists. Allow you to evalute only the source IP address of a packet, it is not as powerfull as extended access lists, but they are less CPU overhead
* extended access lists. Allows you to evaluate source and destination IP address, the type of layer 3 protocol, source and destination port, and parameters. ACL is more complex compared with standard ACL.