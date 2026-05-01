# Simple-Network-2
To create a scalable and secure network by segmenting traffic into VLANs and enabling communication between them through routing.
🧱 Network Architecture
Based on the topology:

Multiple 2960 switches forming access and distribution layers

Router (2811) handling inter-VLAN routing

Multiple end devices (PCs) across departments

Trunk links between switches

Uplink to an external network (ISP simulation)

🌐 VLAN Configuration
Your design clearly separates departments (this is strong):

VLAN 10 – IT → 192.168.10.0/24

VLAN 20 – HR → 192.168.20.0/24

VLAN 30 – Sales → 192.168.30.0/24

👉 This shows:

Logical network segmentation

Reduced broadcast domains

Improved organization and security

⚙️ Key Configurations
Created and assigned VLANs on switches

Configured trunk ports between switches for VLAN traffic

Assigned access ports to specific VLANs

Configured router interfaces for inter-VLAN routing (router-on-a-stick)

Assigned IP addressing per VLAN

Verified connectivity across VLANs using ping

🌍 WAN / External Connectivity
Connected internal network to an external router (ISP simulation)

Used a separate network range (200.1.1.x) for WAN communication

Demonstrated understanding of internal vs external routing

🛠️ Technical Skills Demonstrated
VLAN creation and management

Trunking (802.1Q)

Inter-VLAN routing (router-on-a-stick)

Multi-switch network design

IP addressing and subnetting

WAN connectivity basics

Troubleshooting and validation

✅ Results
Devices within VLANs communicate successfully

Inter-VLAN communication enabled through routing

Traffic properly segmented by department

Network supports both internal and external communication

🧠 Challenges & What I Learned
Learned how incorrect VLAN assignments can block communication

Gained hands-on experience configuring trunk vs access ports

Understood how routers route traffic between VLANs

Strengthened troubleshooting using ping and interface checks

🚀 Future Improvements
This is where you can level it up even more:

Implement DHCP per VLAN

Add ACLs to control inter-VLAN traffic

Introduce Layer 3 switch routing instead of router-on-a-stick

Add redundancy (STP tuning or dual links)

📁 How to Use This Project
Open the .pkt file in Cisco Packet Tracer

Review VLAN configurations on switches

Check trunk links between switches

Inspect router subinterfaces

Test connectivity across VLANs and to external network
