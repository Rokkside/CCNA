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

