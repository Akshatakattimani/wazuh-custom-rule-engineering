# Lab Architecture

## Environment

- Host Machine: Windows Laptop
- Client VM: Windows VM (192.168.56.101)
- Server VM: Kali Linux (192.168.56.102)
- SIEM: Wazuh Manager
- Protocol: SSH

## Workflow

```text
Host Windows Laptop
        │
        ▼
Windows VM (192.168.56.101)
        │
 SSH Authentication Attempt
        │
        ▼
Kali Linux VM (192.168.56.102)
 SSH Server + Wazuh Manager
        │
 Authentication Failure Logged
        │
        ▼
Wazuh Detection Rule (5760)
        │
        ▼
Threat Hunting
        │
        ▼
Wazuh Dashboard
```
