# 01 · Networking Fundamentals

## Network types
- **LAN:** small area (home, office, building)
- **WAN:** connects networks across large distances
- **MAN:** city or large campus
- **PAN:** around one person (e.g. Bluetooth)

## Topologies
Bus · Star · Ring · Mesh. Topology affects **reliability, scalability, and the impact of failures**.

## Models
**OSI (7 layers):** Physical → Data Link → Network → Transport → Session → Presentation → Application.
**TCP/IP (4 layers):** Application, Transport, Internet, Network Access. TCP/IP reflects real networks; OSI is useful for explaining and troubleshooting.

## Devices
| Device | Role |
|--------|------|
| Hub | Broadcasts traffic to all ports |
| Switch | Forwards frames by MAC address |
| Router | Connects networks, forwards packets by IP |
| Firewall | Allows/blocks traffic by rules |
| Access point | Wireless connectivity |

## Addressing & traffic
- **IPv4** (32-bit) / **IPv6** (128-bit)
- **NAT:** translates private ↔ public addresses; conserves IPv4, hides internal addressing
- **VLAN:** logical separation; smaller broadcast domains, isolates sensitive systems
- **VPN:** encrypted tunnel; attackers can abuse legitimate remote access, so investigate carefully
- **MAC:** Data Link identifier for local communication
- **ARP:** maps IPv4 → MAC; no strong authentication, so **ARP spoofing/poisoning** can intercept traffic
- **ICMP:** diagnostics (`ping`); also used in recon or tunneling
- **Routing:** routing tables, default gateway, static/dynamic routes, next hop

## 🔵 Blue Team checkpoint
Look for unexpected connections, unfamiliar IPs, unusual ports, abnormal traffic patterns, repeated connection attempts.
**Source → Protocol → Destination → Route → Network segment → Expected or not?**
