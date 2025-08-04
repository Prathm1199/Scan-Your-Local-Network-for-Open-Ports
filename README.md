# Scan-Your-Local-Network-for-Open-Ports
### Tools Used:
- Nmap
- Wireshark

### IP Range Scanned:
192.168.4.0/24

## Scan Command:
```bash
nmap -sS 192.168.4.0/24
```

Results:
IP Address	Open Ports
192.168.4.120	None
192.168.4.232	53/tcp (domain)
192.168.4.72	None

Analysis:
Port 53/tcp on 192.168.4.232 is open.

This suggests a DNS service is running on that host.

DNS over TCP is typically used for:

Large DNS responses

Zone transfers (AXFR)

If improperly configured, could pose a security risk:

DNS spoofing

Amplification attacks

No other devices showed open ports in this scan.

Additional Notes:
Packet capture was taken using Wireshark during scan.
Verified port function using: SpeedGuide
