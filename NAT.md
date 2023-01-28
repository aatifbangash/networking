### NAT (Network address translation)
It is a table in the network routes. It is used when user request for the server but server is out of the subnet/lan. In order to understand it first we have to understand request flow from client to server.

##### Client and Server are in the same subnet/lan.
* If user request from client 192.168.0.2 to the server 192.168.0.3 for the data.
* The request will go to the router 192.168.0.1 (public IP 66.68.1.1). The Router will check if the server 192.168.0.3 is within the same subnet/lan it will route the request to that node, get the response and send that response back to the client 192.168.0.2

##### Client and Server are not in the same subnet/lan.
* If user request from client 192.168.0.2 to the server 44.68.0.5 for the data.
* The request will go to the router 192.168.0.1 (public IP 66.68.1.1). The Router will check and will found that the server xxxx is out of the subnet. It will add the following entry to the NAT table of the router.
* > SOURCE_IP --> ROUTER_PUBLIC_IP --> SERVER_IP
* > 192.168.0.2 --> 66.68.1.1 --> 44.68.0.5
* Send request to the server 44.68.0.5
* Once response/acknowledgment received from the server to the router on the router public ip. 
* It will be checked in the NAT of the router that what was the source ip of the node.
* Deliver response at the source node via source ip.