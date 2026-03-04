# 02 - Build Notes (What I Did)

## Hypervisor
- Hypervisor used: (VirtualBox or VMware)
- Host PC: Windows 11
- Lab network: 10.10.10.0/24

## VM List
### DC01 (Windows Server 2022)
- CPU:
- RAM:
- Disk:
- Network adapters:
  - Adapter 1: NAT (internet)
  - Adapter 2: Host-only (lab LAN)

Static IP (Host-only):
- IP: 10.10.10.10
- Mask: 255.255.255.0
- DNS: 10.10.10.10

### CL01 (Windows 11/10 Pro)
- CPU:
- RAM:
- Disk:
- Network adapters:
  - Adapter 1: NAT
  - Adapter 2: Host-only

Static IP (Host-only):
- IP: 10.10.10.20
- Mask: 255.255.255.0
- DNS: 10.10.10.10

## Domain Setup
- Domain name: lab.local
- Roles installed on DC01:
  - Active Directory Domain Services (AD DS)
  - DNS

## Validation (Proof it works)
- Ping tests:
  - CL01 → 10.10.10.10 (DC01)
- Domain join:
  - CL01 successfully joined lab.local
- Login test:
  - Logged into CL01 using LAB\Administrator
