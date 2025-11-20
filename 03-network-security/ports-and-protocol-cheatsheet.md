# Ports and Protocols Cheatsheet

## Why This Topic
Any cybersecurity role requires strong familiarity with ports and protocols. Analysts must understand how services communicate, how attackers exploit open ports, and how to identify suspicious behaviour. This cheatsheet serves as a quick reference and demonstrates practical knowledge of network fundamentals.

---

## Common Ports and Their Uses

### Secure Communication
| Port | Protocol | Description |
|------|----------|-------------|
| 22 | SSH | Secure shell for remote administration |
| 443 | HTTPS | Encrypted web traffic |
| 3389 | RDP | Remote Desktop Protocol for Windows systems |

### Web and Application Traffic
| Port | Protocol | Description |
|------|----------|-------------|
| 80 | HTTP | Standard unencrypted web traffic |
| 8080 | HTTP Proxy | Alternative web and proxy port |
| 53 | DNS | Domain name resolution |

### Email Services
| Port | Protocol | Description |
|------|----------|-------------|
| 25 | SMTP | Mail transfer |
| 110 | POP3 | Basic email retrieval |
| 143 | IMAP | Enhanced email retrieval |

### File Transfer and Administration
| Port | Protocol | Description |
|------|----------|-------------|
| 21 | FTP | File transfer (unencrypted) |
| 69 | TFTP | Simple file transfer |
| 23 | Telnet | Remote connection (unencrypted and insecure) |

### Network and Security Services
| Port | Protocol | Description |
|------|----------|-------------|
| 161 | SNMP | Device monitoring |
| 445 | SMB | Windows file sharing |
| 514 | Syslog | Centralised logging |

---

## Why Ports Matter in Cybersecurity
- Attackers scan ports to identify vulnerable services  
- Misconfigured ports often lead to breaches  
- Analysts use port knowledge during threat analysis  
- Firewalls rely on port rules to filter traffic  
- Packet analysis requires understanding of port behaviour  

---

## Reflection
Learning ports and protocols helped me build a strong foundation for both defensive and offensive analysis. This knowledge improved my ability to read packet captures, write firewall rules, and understand attack paths. It also made tools such as Wireshark, Suricata, and tcpdump far easier to use because I could immediately recognise what each packet represented.
