# Objective
Configure RouterA so that PC1 and PC2 will be able to communicate with PC3 and PC4. Then log on to the console of PC1 and PC2, and ping PC3 and PC4. The configuration for RouterB, SwitchA, SwitchB, and all four PC hosts has already been completed.

Lab Topology
The topology for this lab contains three networks: the 10.1.1.4/30 wide area network (WAN) that contains the serial interfaces that connect RouterA and RouterB, the 192.168.100.0/24 local area network (LAN) that connects PC1 and PC2 to the FastEthernet 0/0 interface of RouterA, and the 192.168.200.0/24 LAN that connects PC3 and PC4 to the FastEthernet 0/0 interface of RouterB. Enhanced Interior Gateway Routing Protocol (EIGRP) is used to exchange routing table updates between RouterA and RouterB.

The lab topology displays information about the network devices in the lab. To access each of the devices from within the Simulator, select the device name from the Devices pane or open the lab topology and double-click a device to display that device’s console locally.

<img width="360" height="310" alt="Screenshot 2026-03-11 at 11 37 03 AM" src="https://github.com/user-attachments/assets/23063995-8965-4be0-9ee2-cf42b332f628" />

<img width="504" height="256" alt="Screenshot 2026-03-11 at 11 38 01 AM" src="https://github.com/user-attachments/assets/a99af604-fd76-43dc-991a-3984fe309fc1" />

The IP addresses and subnet masks used in this lab are shown in the tables below:

### IP ADDRESSES

<img width="504" height="151" alt="Screenshot 2026-03-11 at 11 39 36 AM" src="https://github.com/user-attachments/assets/f4d54641-6f4f-410f-99f8-23f71276ad41" />

## Lab Tasks
### Task 1: Configure the WAN Interface on RouterA
A video is available that demonstrates the steps used in Task 1 and Task 2 of this lab. Please select the demo video from Boson’s YouTube channel.

This portion of the lab documentation will describe the tasks you should perform. If you have difficulty with these steps, you can see all of the commands you should enter in the Solutions section later in this document.

1. On RouterA, configure the appropriate host name.

<img width="636" height="122" alt="Screenshot 2026-03-11 at 11 42 31 AM" src="https://github.com/user-attachments/assets/a9c25b50-9e38-4da3-92d2-19727835a0af" />

2. On RouterA, configure the Serial 0/0 interface with the appropriate IP address and subnet mask; refer to the IP Addresses table.

<img width="1866" height="212" alt="image" src="https://github.com/user-attachments/assets/5b5bf25e-5d0b-4d60-b688-dd29bb293450" />

3. On RouterA, configure the Serial 0/0 interface to provide clocking for the serial link that connects RouterA and RouterB. The clock speed should be 64 kilobits per second (Kbps).

<img width="1862" height="174" alt="image" src="https://github.com/user-attachments/assets/67eacffe-9b6c-465b-b9bf-1ce97b92b999" />

4. On RouterA, examine the state of Serial 0/0. Use the appropriate command from the Command Summary table.

<img width="1862" height="416" alt="image" src="https://github.com/user-attachments/assets/cb969088-1e24-46ba-accf-95eeb6dc9b10" />

5. On RouterA, enable the Serial 0/0 interface.

<img width="1864" height="238" alt="image" src="https://github.com/user-attachments/assets/958b66d0-d314-4148-b437-83ced7a66bac" />

6. Verify your configuration by issuing a ping from RouterA to RouterB's Serial 0/0 interface (10.1.1.6). The ping should be successful. If not, check your configuration and try again.

<img width="1870" height="242" alt="image" src="https://github.com/user-attachments/assets/78b56350-bf75-46b8-a28e-7cdc7784fefa" />


## Task 2: Configure the LAN Interface on RouterA
1. On RouterA, configure the FastEthernet 0/0 interface with the appropriate IP address and subnet mask; refer to the IP Addresses table.

<img width="1858" height="280" alt="image" src="https://github.com/user-attachments/assets/a3fafda9-70cc-4030-aa51-666c214cbcc8" />

2. Examine the state of FastEthernet 0/0. Use the appropriate command from the Command Summary table.

<img width="1868" height="412" alt="image" src="https://github.com/user-attachments/assets/b08426d5-d8e7-4fd7-b851-e551a02e3116" />

3. On RouterA, enable the FastEthernet 0/0 interface.

<img width="1856" height="244" alt="image" src="https://github.com/user-attachments/assets/c792d824-5e25-4322-8209-1e6c0c4e605a" />

4. From RouterA, ping PC1 (192.168.100.2) and PC2 (192.168.100.3). The pings should be successful. If not, check your configuration and try again.

<img width="1866" height="288" alt="image" src="https://github.com/user-attachments/assets/a1260cd2-bf50-4864-8b5d-899b9591756d" />

## Task 3: Configure and Troubleshoot the EIGRP Dynamic Routing Protocol on RouterA
All interfaces on RouterA should be configured and operational at this point. If you would like to view a video that shows the steps performed in Task 3 and Task 4, please select the appropriate video from Boson’s YouTube channel.

1. From PC1, ping PC3 (192.168.200.2) and PC4 (192.168.200.3). Are these pings successful? Why or why not?

<img width="1868" height="246" alt="image" src="https://github.com/user-attachments/assets/e84c930d-0280-483a-bb92-b3dbb1e9b9d7" />

2. What command could you use on RouterA to troubleshoot this problem?

<img width="1858" height="634" alt="image" src="https://github.com/user-attachments/assets/618c9b3d-b788-42d2-b90b-bf35ff13b06a" />

3. Can you see routes to the 192.168.200.0/24 network in the routing table on RouterA?

<img width="1860" height="114" alt="image" src="https://github.com/user-attachments/assets/e2910645-05c3-4f26-8a0e-0c2d44705a45" />

4. On RouterA, configure an EIGRP process; use an autonomous system number (ASN) of 100.

<img width="1856" height="206" alt="image" src="https://github.com/user-attachments/assets/3c28e967-0c0f-447c-82af-3010b4e0d6dd" />

5. On RouterA, configure EIGRP to announce all networks that are directly connected to RouterA.

<img width="1860" height="208" alt="image" src="https://github.com/user-attachments/assets/217e13f8-9c49-4f17-9180-b61fd89a1830" />

## Task 4: Verify Network Connectivity
1. From PC1, ping PC3 (192.168.200.2) and PC4 (192.168.200.3). Are the pings successful?

<img width="1856" height="200" alt="image" src="https://github.com/user-attachments/assets/4b1fff5b-bf72-40e1-81f6-35add9fcb821" />

2. If the pings from PC1 to PC3 and PC4 failed before and are now successful, briefly explain why this is so.

<img width="1854" height="490" alt="image" src="https://github.com/user-attachments/assets/75cf08aa-202a-4291-8051-5419ff14b5fd" />
