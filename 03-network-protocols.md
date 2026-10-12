# 03 · Network Protocols

## TCP vs UDP
| TCP | UDP |
|-----|-----|
| Connection-oriented | Connectionless |
| Reliable delivery | No delivery guarantee |
| Handshake | No handshake |
| More overhead | Lower overhead |
| HTTP/HTTPS | DNS, DHCP, streaming, VoIP |

**TCP three-way handshake:** SYN → SYN/ACK → ACK. TCP evidence shows connection attempts, failures, suspicious ports, repeated behavior.

**IP:** track source/destination IP, packets, routing, TTL, IPv4/IPv6.

## Application protocols
- **DNS:** names → IPs (A, CNAME, MX, NS). Abused for C2, phishing, exfiltration. Watch for unusual domains and abnormal query volume.
- **Telnet:** unencrypted remote access, so credentials are exposed.
- **FTP:** unencrypted file transfer. Unexpected transfers are an indicator.
- **SSH:** encrypted remote access. Watch for failed logins, brute force, suspicious source IPs, unexpected successes, odd post-login commands.
- **HTTP:** methods `GET/POST/PUT/DELETE`; codes 200, 301/302, 400, 401, 403, 404, 500. Look for suspicious URLs, payloads, auth attempts, odd user agents.
- **DHCP:** IP, mask, gateway, DNS. **DORA:** Discover → Offer → Request → ACK.

## 🔵 Blue Team checkpoint
**Who? → What protocol? → What port? → What was requested? → Was it expected? → What does the traffic show?**
