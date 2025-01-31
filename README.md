# NETWORK-PROJECT-03
Vic Modern Hotel Network Design
This project involves the design and implementation of the network for Vic Modern Hotel. The hotel consists of three floors, each hosting various departments with specific network requirements. The project includes configuring routers, VLANs, switches, WiFi networks, and other necessary devices to ensure smooth connectivity between departments and floors.

Project Overview
The network design includes the following features:

Three routers connecting each floor, placed in the IT department's server room.
Inter-router communication using serial DCE cables.
Unique network segments for each department on each floor, with different VLANs assigned.
WiFi networks for laptops and phones in each department.
Printers in each department for printing needs.
Proper IP addressing for each VLAN on every floor.
Network Layout
Floor 1 (Reception, Store, and Logistics):
Reception: VLAN 80, Network 192.168.8.0/24
Store: VLAN 70, Network 192.168.7.0/24
Logistics: VLAN 60, Network 192.168.6.0/24
Floor 2 (Finance, HR, and Sales/Marketing):
Finance: VLAN 50, Network 192.168.5.0/24
HR: VLAN 40, Network 192.168.4.0/24
Sales/Marketing: VLAN 30, Network 192.168.3.0/24
Floor 3 (IT and Admin):
IT: VLAN 20, Network 192.168.2.0/24
Admin: VLAN 10, Network 192.168.1.0/24
Network Design
1. Routers:
Three routers are connected to each floor's switch. The routers are placed in the IT department's server room, and they connect the three floors using serial DCE cables.
The network between the routers will be 10.10.10.0/30, 10.10.10.4/30, and 10.10.10.8/30.
2. VLAN Configuration:
Each department is assigned to a unique VLAN to ensure proper network segmentation and security:

Reception (VLAN 80) uses network 192.168.8.0/24.
Store (VLAN 70) uses network 192.168.7.0/24.
Logistics (VLAN 60) uses network 192.168.6.0/24.
Finance (VLAN 50) uses network 192.168.5.0/24.
HR (VLAN 40) uses network 192.168.4.0/24.
Sales/Marketing (VLAN 30) uses network 192.168.3.0/24.
IT (VLAN 20) uses network 192.168.2.0/24.
Admin (VLAN 10) uses network 192.168.1.0/24.
Each floor will have a dedicated switch, and all departments in the same floor will be connected to the respective VLAN on that floor’s switch.

3. Inter-floor Communication:
The routers on each floor will be connected to each other using serial DCE cables to ensure communication between the floors. This setup allows each floor to communicate with the others through routing protocols, such as RIP or OSPF.

4. WiFi Networks:
Each floor will have WiFi networks to provide wireless connectivity to laptops and phones. Each department on the floor will have its own wireless access point, ensuring employees can connect their mobile devices and laptops to the network seamlessly.

5. Printers:
Each department will have a printer. The printers will be connected to the local network in their respective VLANs. These devices will be accessible to all PCs and devices within the same department.

Technical Requirements
Devices Used:
Routers: Three routers will connect the floors and enable inter-floor communication.
Switches: One switch per floor to connect devices and configure VLANs.
PCs: Each department has multiple PCs connected to the switch.
Printers: One printer for each department.
WiFi Access Points: One per floor for wireless device connectivity.
Cables:
Ethernet cables for connecting PCs and printers to switches.
Serial DCE cables for inter-router connections.
IP Addressing Scheme:
First Floor:

Reception: 192.168.8.0/24
Store: 192.168.7.0/24
Logistics: 192.168.6.0/24
Second Floor:

Finance: 192.168.5.0/24
HR: 192.168.4.0/24
Sales/Marketing: 192.168.3.0/24
Third Floor:

IT: 192.168.2.0/24
Admin: 192.168.1.0/24
Router Configuration:
Each router will have interfaces connected to each floor's VLAN and a serial connection for inter-router communication. Static routes or dynamic routing protocols will be configured for inter-floor communication.
Testing and Validation
Once the network is set up and all devices are connected:

Ping Tests: PCs on different floors should be able to ping each other to ensure the routers are correctly routing traffic between floors.
WiFi Connectivity: Test wireless devices like laptops and phones to ensure they can connect to the network and access resources.
Printer Access: Verify that each department's PCs can print to their respective department’s printer.
Router Configuration Verification: Ensure that routing protocols (e.g., RIP or OSPF) are correctly configured to allow communication between the routers and VLANs.
Conclusion
The Vic Modern Hotel network design provides a robust and scalable network to connect the various departments on three floors. By using VLANs, WiFi networks, and carefully configured routing, the network ensures efficient communication, security, and scalability for all hotel operations.

Project Files
The project file is available in the repository:

Network Design File: vic_modern_hotel_network.pkt – Cisco Packet Tracer file containing the network topology and configurations.
Author Information
Name: Biswajit Sahoo
LinkedIn: Biswajit Sahoo LinkedIn
Email: biswajitsahoo152001@gmail.com
