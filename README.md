# Ex. No: 6 Identifying MAC and IP Addresses Using Packet Tracer
# Date:19.09.2025
________________________________________
# Objective
To use Cisco Packet Tracer simulation mode to capture and analyze MAC and IP address information for both local and remote network communication.
________________________________________
# Apparatus/Tools Required
•	Cisco Packet Tracer<br>
•	Pre-configured network topology (as provided in the activity file)<br>
•	PCs, switches, router, hub, and wireless access point (as per given setup)<br>
________________________________________
# Network Topology Diagram
# Description:
•	The topology contains a local network (172.16.31.0/24) connected to a remote network (10.10.10.0/24) via a router.<br>
•	Devices include PCs, switches, hub, and wireless AP.<br>
(Insert screenshot of your Packet Tracer setup here)<br>
________________________________________
# IP Addressing Table
(Example – actual values from simulation)<br>
Device	IPv4 Address	Subnet Mask	MAC Address<br>
PC-A	172.16.31.5	255.255.255.0	00D0:D311:C788<br>
PC-B	172.16.31.2	255.255.255.0	000C:85CC:1DA7<br>
Router (G0/0)	172.16.31.1	255.255.255.0	00D0:BA8E:741A<br>
PC-Remote	10.10.10.2	255.255.255.0	00D0:588C:2401<br>
________________________________________
# Procedure
# Part 1: Local Network Communication
1.	Click PC-A (172.16.31.5) and open the Command Prompt.<br>
2.	Enter ping 172.16.31.2.<br>
3.	Switch to Simulation Mode and repeat the ping.<br>
4.	When the PDU appears, click it and record: Destination MAC, Source MAC, Source IP, Destination IP, and the device name.<br>
5.	Use Capture/Forward to follow the PDU through the network until it reaches PC-B.<br>
6.	Record the information in a table.<br>
7.	Repeat the above process for:<br>
o	Ping from 172.16.31.3 to 172.16.31.2<br>
o	Ping from 172.16.31.5 to 172.16.31.4<br>
Part 2: Remote Network Communication<br>
1.	From PC-A (172.16.31.5), enter ping 10.10.10.2.<br>
2.	Switch to Simulation Mode and repeat the ping.<br>
3.	When the PDU appears, note the Destination MAC, Source MAC, Source IP, and Destination IP.<br>
4.	Follow the PDU step-by-step until it reaches the remote PC.<br>
5.	Observe how MAC addresses change at the router while IP addresses remain constant end-to-end.<br>
________________________________________
# Example Data Recording Table
At Device	Dest. MAC	Src MAC	Src IPv4	Dest IPv4<br>
172.16.31.5	000C:85CC:1DA7	00D0:D311:C788	172.16.31.5	172.16.31.2<br>
Switch1	000C:85CC:1DA7	00D0:D311:C788	N/A	N/A<br>
172.16.31.2	00D0:D311:C788	000C:85CC:1DA7	172.16.31.2	172.16.31.5<br>
________________________________________
# Output (Screenshots)
•	PDU details for local communication<br>(Pinging from 172.16.31.5 to 172.16.31.2)


![WhatsApp Image 2025-09-19 at 09 22 09_b9a2d3dd](https://github.com/user-attachments/assets/4055baef-a4ed-4f93-9457-525c6d9524ae)

![WhatsApp Image 2025-09-19 at 09 22 26_1cc91b96](https://github.com/user-attachments/assets/96b15133-5d0d-44bb-9d84-5a37bfc75976)

•	PDU details for remote communication (Pinging from 172.16.31.5 to 10.10.10.2<br>

![WhatsApp Image 2025-09-19 at 09 22 25_07ca6c62](https://github.com/user-attachments/assets/302cadf3-7cab-482f-a93b-35b770b38f24)

![WhatsApp Image 2025-09-19 at 09 22 25_b912679b](https://github.com/user-attachments/assets/c1e21d38-4029-4263-8cda-4db795fa6896)


•	Tables showing MAC/IP changes through each device<br>
Local Communication(From 172.16.31.5 to 172.16.31.2)

![WhatsApp Image 2025-09-19 at 09 27 45_3ec536b0](https://github.com/user-attachments/assets/b6f8b114-5c38-448e-8320-67101eb45710)

Remote Communication(From 172.16.31.5 to 10.10.10.2)

![WhatsApp Image 2025-09-19 at 09 28 37_9cb987d0](https://github.com/user-attachments/assets/97902765-bc07-424e-9bf5-22dcc0d0b387)

________________________________________
# Result
Successfully captured and analyzed MAC and IP addresses for both local and remote communications. Verified that MAC addresses change at each hop while IP addresses remain constant from source to destination.

