## In this lab, you will explore router concepts and learn how routers enable separate networks to communicate with each other.

Lab 1.1 – Router Fundamentals
Objective
This lab corresponds to Module 1: Network Fundamentals in Boson’s CCNA Curriculum. A router forwards packets among computer networks. Routers create separate broadcast domains. Each device that is connected to a router resides in a separate broadcast domain. In this lab, you will explore router concepts and learn how routers enable separate networks to communicate with each other.

The routers in this lab have basic Open Shortest Path First (OSPF) and Dynamic Host Configuration Protocol (DHCP) configurations.

Lab Topology
The lab topology displays information about the network devices in the lab.

<img width="898" height="904" alt="image" src="https://github.com/user-attachments/assets/487152fe-56be-451f-82a7-2e6ea011babc" />

## Conections
<img width="572" height="1288" alt="image" src="https://github.com/user-attachments/assets/5bc2a2d2-1eab-4462-8ccc-4d4aa33850b5" />

<img width="2002" height="1038" alt="image" src="https://github.com/user-attachments/assets/06277fa8-d080-4e26-b951-33059073675c" />

## Lab Tasks
### Task 1: Explore a Broadcast Domain
A broadcast domain is a network segment where all devices receive a copy of a broadcast sent out by a device within the network segment. For example, if a broadcast domain contains 100 devices, each of the 100 devices will receive a copy of a broadcast that is sent by a device within the broadcast domain.

In this task, you will explore how a router behaves within a connected broadcast domain.

From Host2, verify that pings to Host1 (192.0.2.3) are successful. What role does Router2 play in the communications between Host1 and Host2?

From Host2, verify that pings to Router1’s FastEthernet 1/0 interface (192.0.2.1) are successful. Did Router2 have to make a forwarding decision for this ping?

From Host2, attempt to ping Router2’s Loopback 0 interface (2.2.2.2) and FastEthernet 0/0 interface (203.0.113.2). Are the pings successful? Why or why not?

From Host2, attempt to ping Router1’s FastEthernet 0/0 interface (203.0.113.1). Without examining any device configurations, why do you think the ping succeeds?

Task 2: Explore a Router’s Role in a Broadcast Domain
In this task, you will learn how Cisco routers make packet-forwarding decisions from the edge of a broadcast domain.

From Router2, attempt to ping Router1’s Loopback 0 interface (1.1.1.1). Why does the ping succeed?

From Router2, attempt to ping Router1’s FastEthernet 1/0 interface (192.0.2.1). Why does the ping succeed?

From Host1, attempt to ping Router1’s FastEthernet 1/0 interface (192.0.2.1). Why does this ping succeed? How is it different from the successful ping from Router2?

From Host1, attempt to ping Router2’s FastEthernet 0/0 interface (203.0.113.2). Why does this ping succeed?
