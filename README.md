# 🏫 University Campus Network Design
Comprehensive multi-campus network design for a university with 8+ VLANs, OSPF routing, EtherChannel (LACP), and security features including Port Security and ACLs to isolate student traffic. Built with Cisco Packet Tracer.

## 📌 Project Overview
This project simulates a "multi-campus university network" using Cisco Packet Tracer. It includes :VLAN segmentation,Inter-VLAN routing,OSPF,DHCP,EtherChannel,Port Security,and ACLs.


## 🛠 Technologies Used
- **VLANs, Trunking**
- **Inter-VLAN Routing** (Router-on-a-Stick)
- **EtherChannel (LACP)** for link aggregation
- **Static Routing** for external server access
- **OSPF** as dynamic routing protocol
- **DHCP** for automatic IP allocation
- **Port Security** on student labs
- **ACLs** to restrict student access to admin networks


## 📊 IP Addressing Scheme
| VLAN | Department | Network | Gateway |
|------|------------|---------|---------|
| 10 | Admin | 192.168.1.0/24 | 192.168.1.10 |
| 20 | HR | 192.168.2.0/24 | 192.168.2.10 |
| 30 | Finance | 192.168.3.0/24 | 192.168.3.10 |
| 40 | Business | 192.168.4.0/24 | 192.168.4.10 |
| 50 | Engineering | 192.168.5.0/24 | 192.168.5.10 |
| 60 | Art & Design | 192.168.6.0/24 | 192.168.6.10 |
| 70 | Student Labs(Main Campus) | 192.168.7.0/24 | 192.168.7.10 |
| 80 | IT Dept | 192.168.8.0/24 | 192.168.8.10 |
| 90 | Student Labs(Small Campus) | 192.168.9.0/24 | 192.168.9.10 |
| 100 | Science | 192.168.10.0/24 | 192.168.10.10 |


## 🔐 Security Features
- **Port Security**: Max 2 MAC address per port on student VLANs
- **ACLs**: Block student VLAN (60) from accessing Admin/HR/Finance


## 🧪 Testing & Verification
✅ **Inter-VLAN Routing**: PC in VLAN 10 can ping PC in VLAN 30  
✅ **Internet Access**: Internal devices can ping external Mail Server (20.0.0.2)  
✅ **ACL Enforcement**: Student PC cannot ping Admin PC  
✅ **EtherChannel**: Port-channel 1 is up with LACP  

