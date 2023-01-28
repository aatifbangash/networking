### DNS resolution
Suppose a user hit the https://google.com in the browser. The request will go through the following steps.
* First the URL (https://google.com) will resolve to the IP address of the server.
    * It will be checked in the browser cache to determine the IP address of the server
    * It will be checked in the hosts file of the operation system.
    * It will be checked in the network router. As some router also cache the IP address for the domain name.
    * If it is not found elsewhere than It will be searched in the public DNS servers.

Once the domain resolve to the IP address of the server the request will process further.