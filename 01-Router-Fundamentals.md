## In this lab, you will explore router concepts and learn how routers enable separate networks to communicate with each other.

Lab 1.1 – Router Fundamentals
Objective
This lab corresponds to Module 1: Network Fundamentals in Boson’s CCNA Curriculum. A router forwards packets among computer networks. Routers create separate broadcast domains. Each device that is connected to a router resides in a separate broadcast domain. In this lab, you will explore router concepts and learn how routers enable separate networks to communicate with each other.

The routers in this lab have basic Open Shortest Path First (OSPF) and Dynamic Host Configuration Protocol (DHCP) configurations.

Lab Topology
The lab topology displays information about the network devices in the lab.

<img width="216" height="226" alt="Screenshot 2026-03-11 at 11 04 04 AM" src="https://github.com/user-attachments/assets/a72e3159-d05b-411d-8c8b-df334a353038" />

## Conections

<img width="144" height="335" alt="Screenshot 2026-03-11 at 11 06 22 AM" src="https://github.com/user-attachments/assets/a0e339de-0085-4551-b00c-dbb8df624f13" />

<img width="432" height="228" alt="Screenshot 2026-03-11 at 11 07 50 AM" src="https://github.com/user-attachments/assets/400d80d4-96e2-43da-8828-84a792d90d50" />

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
