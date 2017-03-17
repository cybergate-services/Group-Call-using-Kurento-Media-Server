# Group-Call-using-Kurento-Media-Server
Scalable solutions that cater to the ever increasing demand for modes of communication is made possible with the advent of Cloud Technology.One of the drawbacks of WebRTC framework is, as the number of peers increase there is a bandwidth overhead at the client
side which sends media to all the other peers. One of the ways to overcome the bandwidth overhead at the client side is to send media through a server. This application uses Kurento Media Server, a Multipoint Control Units (MCU) which is responsible
for routing media to clients connected to a session. To make the application scalable to meet the requirements of increasing
number of clients, the application is deployed as a cluster of media servers which distributes the load equally among them and cater to the
clients. The media servers are deployed in cloud and clustered using a haproxy load balancing server.

## Implementation
 The following classes are used for implementing the application
 * MediaClient class gets the user name and session and registers it
 * MediaServer class is used for managing rooms and sessions during the call
 * Room class stores information about virtual conference rooms and participants connected to it.
 * RoomManager class dynamically allocates and removes room when participants enter and leave room
 * UserRegistry class registers users by name and by session ids to application.
 * UserSession class is used to maintain client sessions and gather ICE candidates to establish communication between client and server.
 
## Installation

It is a MAVEN project and runs on TOMCAT 7 or above. Needs jdk 7 and jre to run the application.

## API Reference

https://webrtc.org/native-code/native-apis/ <br>
http://doc-kurento.readthedocs.io/en/stable/mastering/kurento_API.html
