# 01 - Plan (Active Directory Home Lab)

## Goal (simple)
Build a small Windows Active Directory lab:
- **DC01 (Windows Server 2022)** = domain controller (stores users, passwords, policies)
- **CL01 (Windows 11/10 Pro)** = client PC joined to the domain

## What I will build today
1. Create DC01 VM and install Windows Server 2022
2. Set static IP on the lab network
3. Install AD DS + DNS
4. Create domain: lab.local
5. Create CL01 VM and join it to the domain
6. Create OUs, users, groups
7. Create 1–2 GPOs and test them

## Network plan
- Lab subnet: 10.10.10.0/24 (host-only)
- DC01: 10.10.10.10
- CL01: 10.10.10.20
- DNS for CL01: 10.10.10.10
- NAT adapter used for internet/updates

## Evidence I will capture (screenshots)
- DC01 IP settings (static IP + DNS)
- AD DS + DNS installed
- ADUC showing OUs/users/groups
- DNS zone for lab.local
- CL01 joined to domain
- GPO created + proof it applied
