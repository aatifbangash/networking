### LAN/Subnet
List of the nodes/devices/computer connect with one another via same router.

#### Route
is the main device in the lan. It allow all the nodes to connect to the internet. it has two ips private (also called default gateway) and public ip. Router DHCP server to assign private ip addresses to all nodes connected to it via data cable or wifi.

#### DHCP (Dynamic Host Configuration Protocol) server
It is like a DNS in the router. It resolve Private IP address to Mac address of the network interface of the nodes. Mac address is the physical unique code/address of every network interface.

#### Nodes
Smart phones, tablets, laptops, computers, printers, etc are connected with the router are considered the nodes of the network. They can communicate with one another via private ip addresses. The request (having the Address of the target) will first goes to the router and router check for the target in the DHCP server and send request to the target and response back.

#### Port forwarding
The node out of the subnet can also request allowed to the subnet/lan via subnet public ip but for that the port forwarding need to be configured in the router.