# OBJECTIVE

To find active hosts in the target network block

# ENVIRONMENT

| Parameter   | Value    |
|--------------- | --------------- |
| Target   | Metasploitable  |
| Target IP   | 192.168.208.128   |
| Attacket IP   | 10.69.11.218   |
| Target Range   | 192.168.208.0/24  |
| Tool  |   Nmap    |

# METHODOLOGY

## ICMP Host Discovery

Command:
> nmap -sn 192.168.208.0/24

Explanation:
- -sn for disabling port scanning and only focusing on Host IP Discovery
- 192.168.208.0/24 for IP range to scan

Observation:
- Discovered an active host in the IP range bearing the Ip address 192.168.208.128

# RESULTS

| IP address | Status |
| -------------- | --------------- |
| 192.168.208.128 | Active |

# MITRE ATTACK MAPPING

| Field | Mapping |
| -------------- | --------------- |
| Tactic | Reconaissance(TA0043) |
| Technique | Active Scanning (T1595) |
| Sub-Technique | Scanning IP Blocks (T1595.001) |

# CONCLUSIONS
- An unknown host is discovered with a reachable IP address
- Further steps including enumerating the target for further information regarding the machine and the its open ports 





