# Design and Implementation of an Enterprise Network for a University Campus

## Networking simulation software used:
Cisco Packet Tracer 8.2.2

## Scenario & Requirements:
Albion University is a large university which has two campuses situated 20 miles apart. The university’s students and staff are distributed in 4 faculties; these include the faculties of Health and Sciences; Business; Engineering/Computing and Art/Design. Each member of staff has a PC and students have access to PCs in the labs. Create a network topology with the main components to support the following:

•	**Main Campus**

  Building A: Administrative staff in the departments of management, HR and finance. The admin staff PCs are distributed in the building offices, and it is expected that they will share some networking equipment (Hint: use of VLANs is expected here). The Faculty of Business is also situated in this building.

  Building B: Faculty of Engineering and Computing and Faculty of Art and Design.
  
  Building C: Students’ labs and IT department. The IT department hosts the University Web server and other servers 

•	**Smaller campus:** 

  Faculty of Health and Sciences (staff and students’ labs are situated on separate floors)

•	**Cloud**

  There is also an email server hosted externally on the cloud.



•	Each department/faculty is expected to be on its own separate IP network.

•	The switches should be configured with appropriate VLANs and security settings.

•	RIPv2 will be used to provide routing for the routers in the internal network and static routing for the external server.

•	The devices in building A will be expected to acquire dynamic IP addresses from a router-based DHCP server.


## Technologies Implemented:
1.	Creating a network topology using Cisco Packet Tracer.
   
2.	Hierarchical Network Design.
   
3.	Connecting Networking devices with Correct cabling.
  
4.	Creating VLANs and assigning ports VLAN numbers.
   
5.	Subnetting and IP Addressing.
    
6.	Configuring Inter-VLAN Routing (Router on a stick).
    
7.	Configuring DHCP Server (Router as the DHCP Server).
    
8.	Configuring SSH for secure Remote access.
    
9.	Configuring RIPv2 as the routing protocol.
    
10.	Configuring switchport security or Port-Security on the switches.
    
11.	Host Device Configurations.
    
12.	Test and Verifying Network Communication.

## Network Layout:

![image](https://github.com/user-attachments/assets/b0c39c38-883e-4e83-b976-d98044fc5b74)

## Configuration:

Enabling all necessary ports on the main campus router, smaller campus and cloud routers:

Main campus router

![image](https://github.com/user-attachments/assets/ee2b356b-4f57-4452-a564-2e2bef9e0b52)

Smaller Campus router

![image](https://github.com/user-attachments/assets/a820c142-b331-4d3d-8e12-92d0246fa508)

Cloud

![image](https://github.com/user-attachments/assets/c6a12960-00dd-45d5-932e-83c313be5496)

Configuring clock rate for serial ports on the main campus router:

![image](https://github.com/user-attachments/assets/94b79a04-5bee-4f23-a3e5-3bdd1dbadc89)

Configuring VLANS on all department and faculty switches:

Administration switch

![image](https://github.com/user-attachments/assets/db2f649a-2750-4032-b1c3-6b77837717c3)

HR switch

![image](https://github.com/user-attachments/assets/6f8846ca-c460-4bb2-832b-d27c97c654fd)

Finance switch

![image](https://github.com/user-attachments/assets/aa79ecda-1c7c-4951-808e-eaca35629421)

Business switch

![image](https://github.com/user-attachments/assets/87932f6c-f368-4fd3-b7bd-3e64c41c41af)

E&C switch

![image](https://github.com/user-attachments/assets/3673bec0-f696-421d-92fb-0d8b3a4f8e32)

A&D switch

![image](https://github.com/user-attachments/assets/ca910e55-98df-4779-ab04-b00ecf18139c)

Student lab switch

![image](https://github.com/user-attachments/assets/46427bba-9798-4a32-ac37-45aaae254794)

IT department switch

![image](https://github.com/user-attachments/assets/b946824f-939b-42d2-b050-cdede11a4cbd)

H&S staff switch

![image](https://github.com/user-attachments/assets/b61aa20c-a712-4dfc-bd7c-9c6dc9f88f8c)

H&S student lab switch

![image](https://github.com/user-attachments/assets/e70f7135-1b45-4380-9aaf-cd5f6002469c)

Configuring VLANS and trunk on the main campus layer 3 switch:

![image](https://github.com/user-attachments/assets/445564f8-fc1a-47be-a12c-f7831a838fc1)

![image](https://github.com/user-attachments/assets/c1bfa57e-fcdc-496f-bbc5-fd66038f3494)

![image](https://github.com/user-attachments/assets/a3b34f80-cbe5-478b-8365-2c59063ec0a6)

![image](https://github.com/user-attachments/assets/379a5712-4c01-46e2-94f1-b2581c34b0be)

Configuring VLANS and trunk on the smaller campus layer 3 switch:

![image](https://github.com/user-attachments/assets/9c05cb2e-8c87-4f13-b161-c4f50502c2d8)

Configuring IP addresses on router interfaces:

Main campus router

![image](https://github.com/user-attachments/assets/bf2f6c90-eab4-4a1e-9dda-0dac850c8e9a)

Smaller campus router

![image](https://github.com/user-attachments/assets/595d4f41-39c0-4506-b888-de7163ed2688)

Cloud

![image](https://github.com/user-attachments/assets/60c8046b-e843-4a22-989d-7666cb45eab2)

Configuring and testing cloud server:

![image](https://github.com/user-attachments/assets/c70cc5dd-768b-472d-b243-7fe197f0a35e)

Server has successful connection to default gateway

![image](https://github.com/user-attachments/assets/4bf2594c-cfff-482c-b19c-282b5ab294cc)

Configuring inter VLAN routing and DHCP on the main campus router:

![image](https://github.com/user-attachments/assets/031daacb-eee0-4bbf-b5cc-f62b88962213)

![image](https://github.com/user-attachments/assets/7fef8609-d558-4e0a-a55a-423d20cdc13c)

Configuring inter VLAN routing and DHCP on the smaller campus router:

![image](https://github.com/user-attachments/assets/142c61b8-e26c-4512-81e4-d01ca8028714)

![image](https://github.com/user-attachments/assets/202c72ad-f5f0-4053-b9a4-b87f15858098)

Ensuring clients are receiving IP addresses via DHCP:

![image](https://github.com/user-attachments/assets/be484026-daac-4dd1-aed7-41e7f77a608b)

Ensuring clients (on the same campus) can communicate between VLANS by pinging a PC in VLAN 70 from a PC in VLAN 10:

![image](https://github.com/user-attachments/assets/e9c51b67-e47e-4d8d-a878-23174addd819)

Communication between campuses is still not available as we still need to configure RIPv2

![image](https://github.com/user-attachments/assets/1c7b91ca-14d3-4396-9e55-c6dca69b5a16)

Configuring RIPv2 on all routers:

Main campus router

![image](https://github.com/user-attachments/assets/4a219f97-0106-4b7c-9b54-23c9a4f744b3)

Small campus router

![image](https://github.com/user-attachments/assets/5d19e483-dac2-4117-96a7-c07e3224f2f1)

Cloud router

![image](https://github.com/user-attachments/assets/4b951fb9-8c7a-40ea-856f-7c0909efc9d8)


Ensuring successful communication between campuses:

Successful ping from a PC on the main campus (VLAN 20) to a PC on the smaller campus (VLAN 90)

![image](https://github.com/user-attachments/assets/302f6ead-936d-4d0f-9fe5-5e834ccfc2f6)

Successful ping from a PC on the main campus (VLAN 20) to the cloud server 

![image](https://github.com/user-attachments/assets/18d29388-effa-4fc0-9aaf-a40d86ed1bef)

## Final network layout:

![image](https://github.com/user-attachments/assets/b757dcfa-b4f4-472f-81dd-1e87daf11733)

