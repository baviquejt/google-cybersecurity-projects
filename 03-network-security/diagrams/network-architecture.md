# Network Architecture Overview (High-Level)

                          
                          
                          
                          ┌───────────────────────────────┐
                          │          Internet              │
                          └───────────────┬────────────────┘
                                          │
                               (Traffic enters network)
                                          │
                                  ▼ Firewall / IPS ▼
                          ┌───────────────────────────────┐
                          │ FIREWALL / IDS / IPS Layer     │
                          │ - Packet filtering             │
                          │ - Threat detection             │
                          │ - Blocks malicious traffic     │
                          └───────────────┬────────────────┘
                                          │
                       ┌──────────────────┴──────────────────┐
                       │                                     │
                       ▼                                     ▼
        ┌──────────────────────────┐             ┌──────────────────────────┐
        │ DMZ (Public Services)    │             │ Internal Network (LAN)   │
        │ - Web servers            │             │ - Endpoints (PCs, Laptops)│
        │ - Email gateway          │             │ - Printers                │
        │ - Reverse proxies        │             │ - Secure Wi-Fi            │
        └──────────────┬───────────┘             └──────────────┬───────────┘
                       │                                         │
                       │                                         │
                       ▼                                         ▼
        ┌──────────────────────────┐             ┌──────────────────────────┐
        │ Load Balancer            │             │ Core Switch               │
        │ - Distributes traffic    │             │ - VLAN segmentation       │
        │ - High availability      │             │ - Internal routing        │
        └──────────────┬───────────┘             └──────────────┬───────────┘
                       │                                         │
                       ▼                                         ▼
        ┌──────────────────────────┐             ┌──────────────────────────┐
        │ Application Servers       │            │ Database Servers          │
        │ - Backend systems         │            │ - Customer data           │
        │ - Business logic          │            │ - Encrypted at rest       │
        └──────────────┬───────────┘             └──────────────┬───────────┘
                       │                                         │
                       ▼                                         ▼
        ┌──────────────────────────┐             ┌──────────────────────────┐
        │ Logging & Monitoring     │             │ Security Tools            │
        │ - SIEM                   │             │ - Endpoint protection     │
        │ - Syslogs                │             │ - Vulnerability scanner   │
        │ - Suricata IDS logs      │             │ - Asset management        │
        └──────────────────────────┘             └──────────────────────────┘
