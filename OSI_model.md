### OSI MODEL
OSI model represent the flow of request/data from client to server. There are 7 layers are involved in the OSI model. Which are following.

1. Application
1. Presentation
1. Session
1. Transport
1. Network
1. Data
1. Physical

At the client it goes from top to bottom (1 - 7) and at the receiver end (server) it goes from bottom to to (7 - 1).

#### Lets understand the OSI model by example
Suppose user hit the a specific url (either POST or GET) from the client or browser. Then the following will happened to the request.
##### Application layer
It is the actual message/data from the application. This layer also attach the header to request.
##### Presentation layer
This layer encrypt the message if the ssl is active for the URL
##### Session layer
This layer add tag to the message. And resolve the domain name to IP of the target
##### Transport layer
This layer break the message into the segments add the source and target PORT to each segment.
##### Network layer
This divide each segment into the packets and add the source and target IP address to each packet.
##### Data layer
This layer further divide the packets into the fragments and add the MAC address to each fragment
##### Physical layer
This layer convert each fragment into the binary bits and send every bit to the target via data cable or signals.

### TCP/IP
The TCP/IP model used for the communication in the network. It is same as OSI model. But only difference is that it has 5 layers. 
* Application (Presentation and session are included in the application layer)
* Transport
* Network
* Data
* Physical