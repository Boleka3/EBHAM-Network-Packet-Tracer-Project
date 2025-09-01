📘 EBHAM Network Project
●	Overview
This project documents the complete design, configuration, and security implementation of a network topology built during NTI training. The work focuses on subnetting, routing (OSPF), DHCP, ACLs, AAA authentication, firewall policies, NTP/Syslog integration, and Layer 2 security. The project demonstrates both fundamental networking principles and advanced security practices, ensuring robust connectivity and protection across devices.
________________________________________
📑 Table of Contents
1.	Project Objectives
2.	Network Design
3.	Subnetting & Addressing
4.	Configuration Details
o	Router & Switch Setup
o	DHCP Deployment
o	OSPF Routing
o	Security Features (ACL, AAA, Views, ZPF)
5.	Layer 2 Security
6.	NTP & Syslog
7.	Testing & Verification
8.	Team & Credits
________________________________________
🎯 Project Objectives
•	Implement an enterprise-scale network using Cisco routers and switches.
•	Apply subnetting strategies to optimize IP utilization.
•	Configure dynamic IP allocation via DHCP.
•	Deploy OSPF for efficient dynamic routing.
•	Secure the network with ACLs, AAA authentication, and encrypted routing updates.
•	Enforce Layer 2 security (STP, Portfast, BPDU Guard).
•	Set up Syslog and NTP for monitoring and synchronization.
•	Configure a Zone-Based Firewall for traffic inspection.
________________________________________
🌐 Network Design
•	Topology: Multi-router and multi-switch setup with end devices, servers, and VLANs.
•	Routing Protocol: OSPF with SHA authentication.
•	Security Enhancements: ACLs, ZPF, AAA, encrypted passwords.
•	Services: DHCP, NTP, Syslog, SSH access.
________________________________________
📊 Subnetting & Addressing
The network uses VLSM (Variable Length Subnet Masking) for efficient allocation.
•	Large subnets (/28) for LANs.
•	Point-to-point links using /30 subnets.
•	Address table ensures clear IP ranges, broadcast IDs, and host counts.
(See full addressing table in the documentation for details.)
________________________________________
⚙️ Configuration Details
🔧 Router & Switch Setup
•	Hostnames, enable/console/vty passwords.
•	Password encryption & minimum length enforcement.
•	Logging synchronous for smoother CLI usage.
📡 DHCP Deployment
•	Routers configured with DHCP pools for automatic host assignment.
•	Static IP assignments for servers, DNS, and key devices.
📍 OSPF Routing
•	Enabled across all routers.
•	Passive interfaces for end-device connections.
•	SHA authentication applied to secure OSPF updates.
🔒 Security Features
•	ACLs: Restrict traffic to specific hosts and services.
•	AAA Authentication: Integrated with local and TACACS+/RADIUS methods.
•	Views: Role-based CLI command restrictions.
•	Zone-Based Firewall (ZPF): Allows only HTTPS and ICMP between zones, dropping other traffic.
________________________________________
🔐 Layer 2 Security
•	VLAN segmentation (VLAN 10 & VLAN 20).
•	Trunk connections between switches and router.
•	STP enhancements with Portfast and BPDU Guard.
________________________________________
⏱️ NTP & Syslog
•	NTP hierarchy configured from servers to routers and switches.
•	Syslog server deployed to collect device logs for monitoring and troubleshooting.
________________________________________
🧪 Testing & Verification
•	Ping & connectivity tests between PCs across VLANs and routers.
•	SSH access validated with ACL restrictions.
•	Firewall inspection tested with HTTPS and ICMP sessions.
•	Syslog and NTP successfully synchronized across devices.
________________________________________
👥 Team & Credits
The project was completed collaboratively during NTI Training by the team EBHAM, with contributions in:
•	Subnetting & Addressing
•	Routing & Switching Configuration
•	Security Policies
•	Testing & Documentation
Special thanks to our instructor for guidance and support throughout the project.
________________________________________
🚀 Conclusion
●	This project demonstrates a complete implementation of enterprise networking—from design to configuration and security. By applying advanced routing, subnetting, and security mechanisms, it delivers a highly available and secure environment, suitable for real-world enterprise deployments.

