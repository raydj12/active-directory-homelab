# 03 - Troubleshooting / Lessons Learned

## Common issues I ran into (and fixes)
### 1) Domain join fails
- Cause: Client DNS was not pointing to the Domain Controller
- Fix: Set CL01 DNS to 10.10.10.10

### 2) Cannot find DC by name
- Cause: DNS not configured / wrong network adapter used
- Fix: Use the host-only adapter for lab traffic and ensure DNS role is installed

### 3) VM networking confusion
- NAT = internet access
- Host-only = private lab network (AD traffic stays here)
