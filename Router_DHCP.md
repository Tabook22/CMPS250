

Router>enable <br>
Router#configur t<br>

Router(config)#hostname Nasser-Router<br>

Nasser-Router(config)#interface gigabitEthernet 0/0<br>
Nasser-Router(config-if)#ip<br>
Nasser-Router(config-if)#ip address<br>
Nasser-Router(config-if)#ip address 192.168.1.1 255.255.255.0<br>
Nasser-Router(config-if)#no sh<br>
Nasser-Router(config-if)#no shutdown <br>

## Configur DHCP<br>
Router#configur t<br>
Nasser-Router(config)#service dhcp<br>
Nasser-Router(config)#ip dhcp pool Net-Pool<br>
Nasser-Router(dhcp-config)#network 192.168.1.0 255.255.255.0<br>
Nasser-Router(dhcp-config)#default-router 192.168.1.1<br>
Nasser-Router(dhcp-config)#dns-server 192.168.1.2<br>
Nasser-Router(dhcp-config)#domain-name nasser.com<br>
Nasser-Router(dhcp-config)#ip dhcp excluded-address 192.168.1.1 192.168.1.10<br>
Nasser-Router(config)#exit<br>
Nasser-Router#w <br>

---

![](images/Dhcp_Router.png)
