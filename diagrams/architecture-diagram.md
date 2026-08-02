# Wazuh Lab Architecture

The following diagram illustrates the communication flow used in this project.

```text
                 Host Windows Laptop
                        │
        ┌───────────────┴───────────────┐
        │                               │
        ▼                               ▼
 Windows VM                     Kali Linux VM
192.168.56.101                 192.168.56.102
 SSH Client                 SSH Server + Wazuh Manager
        │                               │
        └──────── SSH Login ───────────►│
                                        │
                              Authentication Failure
                                        │
                                        ▼
                               Wazuh Detection Engine
                                        │
                                        ▼
                                Threat Hunting Module
                                        │
                                        ▼
                                Wazuh Dashboard
```

## Components

- **Host:** Windows Laptop
- **Client VM:** Windows VM (192.168.56.101)
- **Server VM:** Kali Linux (192.168.56.102)
- **Monitoring Platform:** Wazuh Manager
- **Protocol:** SSH
