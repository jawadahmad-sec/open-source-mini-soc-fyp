# Lab Status - Step 1: Virtual Lab Setup

## Project Information
- **Project:** Open-Source Mini SOC for Automated Threat Detection
- **Student:** Jawad Ahmad
- **Supervisor:** Dr. Fakhrud Din
- **University:** University of Malakand
- **Department:** Computer Science & IT

## Virtual Laboratory Environment
All VMs are configured with **Dual Network Adapters**:
- **Adapter 1:** NAT (for internet access)
- **Adapter 2:** Host-Only Adapter (isolated lab network for attacks and monitoring)

## Host-Only Network IP Mapping

| Virtual Machine | Role | Host-Only IP Address |
|-----------------|------|----------------------|
| Kali Linux 2026.1 | Attacker | 192.168.56.102 |
| Windows Server 2008 | Target (Windows) | 192.168.56.101 |
| Metasploitable 3 (Ubuntu) | Target (Linux) | 192.168.56.103 |

## Connectivity Verification (from Kali Linux)

| Target | Command | Result |
|--------|---------|--------|
| Windows Server 2008 | `ping 192.168.56.101` | ✅ OK |
| Metasploitable 3 (Ubuntu) | `ping 192.168.56.103` | ✅ OK |

## Security Notes for Lab
- Firewalls disabled on target machines for initial testing.
- Network is isolated (Host-Only) with no external access during attack simulation.
- All attacks are authorized and strictly within the lab environment.

## Next Steps
- Step 2: Perform first Nmap scan from Kali to both targets.
- Step 3: Install and configure Suricata IDS.
