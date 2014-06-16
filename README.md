SDN
===

Programming Assignment Solutions for Coursera SDN Course
Below are assignment descriptions from Nick Feamster's SDN Coursera

1) CustomTopo.py
Data center networks typically have a tree-like topology.
End-hosts connect to top-of-rack switches, which form the leaves 
(edges) of the tree; one or more core switches form the root; 
and one or more layers of aggregation switches form the middle of the tree. 
In a basic tree topology, each switch (except the core switch) has a single parent switch.  
Additional switches and links may be added to construct more complex tree topologies (e.g., fat tree)
in an effort to improve fault tolerance or increase inter-rack bandwidth.

In this assignment, your task is to create a simple tree topology.
You will assume each level i.e., core, aggregation, edge and host to be composed of 
a single layer of switches/hosts with a configurable fanout value (k). 

2) firewall.py , firewall-policies.csv
A Firewall is a network security system that is used to control the flow of ingress and egress traffic 
usually between a more secure local-area network (LAN) and a less secure wide-area network (WAN). 
The system analyses data packets for parameters like L2/L3 headers (i.e., MAC and IP address) or performs
deep packet inspection (DPI) for higher layer parameters (like application type and services etc) to filter network traffic.
A firewall acts as a barricade between a trusted, secure internal network and another network (e.g. the Internet)
which is supposed to be not very secure or trusted.

In this assignment, your task is to implement a layer 2 firewall that runs alongside the MAC learning
module on the POX OpenFlow controller. The firewall application is provided with a list of MAC address
pairs i.e., access control list (ACLs). When a connection establishes between the controller and the switch, 
the application installs flow rule entries in the OpenFlow table to disable all communication between each MAC pair. 

3) topologySlice.py, mininetSlice.py, videoSlice.py
