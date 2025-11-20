# Packet Flow Overview

## Why This Topic
Understanding how packets travel across a network is essential for any cybersecurity analyst. Packet flow knowledge allows analysts to identify suspicious behaviour, troubleshoot connectivity issues, and understand where security controls such as firewalls, IDS, and proxies apply. Recruiters look for candidates who can explain packet movement clearly because it demonstrates both network awareness and analytical thinking.

---

# Packet Flow Diagram

flowchart LR

    A[User Device(Laptop / Phone)] --> B[NIC(Network Card)]
    B --> C[Switch(Local Network)]
    C --> D[Router(Gateway / NAT)]
    D --> E[Firewall(Packet Filtering)]
    E --> F[ISP / Public Internet]
    F --> G[Destination Server(Website / API / Cloud)]



---

## Explanation of Packet Flow

### 1. User Device
This is where the packet originates, such as a laptop, desktop, or mobile device.

**Security relevance:**
- Endpoint protection and operating system patching  
- Identity and access management  
- Risk of malware, misconfigurations, or unsafe user behaviour  

---

### 2. Network Interface Card (NIC)
The NIC converts data into frames and prepares it for transmission on the local network.

**Security relevance:**
- Source MAC address identification  
- Useful for packet capture analysis at Layer 2  
- Possible attack surface for MAC spoofing or ARP-based attacks  

---

### 3. Switch
The switch forwards frames based on MAC addresses inside the local network.

**Security relevance:**
- VLAN segmentation to isolate sensitive areas  
- Port security to restrict device access  
- Exposure to switching attacks such as ARP poisoning  

---

### 4. Router
The router directs packets between networks and handles routing decisions.

**Security relevance:**
- Key enforcement point for segmentation  
- Routing tables can be misconfigured or manipulated  
- Critical for filtering and network path control  

---

### 5. Firewall
A firewall evaluates packet headers and sometimes deeper packet content based on a rule set.

**Security relevance:**
- Packet filtering based on IP address, protocol, and port  
- Stateful inspection to track connection state  
- Main control for enforcing network security policy  

---

### 6. Internet Service Provider (ISP)
The ISP transports the packet across wider networks including the public internet.

**Security relevance:**
- Traffic leaves the organisation’s direct control  
- Limited visibility into intermediate hops  
- Depends on the ISP’s routing and infrastructure stability  

---

### 7. Destination Server
This can be a web server, API endpoint, database, or cloud service.

**Security relevance:**
- Server hardening and patching  
- TLS use to encrypt data in transit  
- Logging and monitoring of incoming and outgoing connections  

---

## Why Packet Flow Matters for Cybersecurity

Understanding packet flow helps cybersecurity analysts:

- Identify the correct placement of controls such as firewalls, proxies, and IDS  
- Troubleshoot network issues more effectively  
- Investigate suspicious traffic patterns  
- Analyse logs and packet captures with better context  
- Understand lateral movement during incidents  
- Communicate clearly with network engineers and senior analysts  

---

## Reflection

Building this packet flow overview improved my ability to analyse network behaviour with tools such as Wireshark, Suricata, and tcpdump. Instead of viewing packet data as isolated information, I now understand how each hop shapes the security posture of an organisation. It also highlighted the importance of segmentation, traffic filtering, and endpoint controls because
