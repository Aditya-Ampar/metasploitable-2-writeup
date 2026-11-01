# OBJECTIVE

To find OS , kernel, kernel version and other details of the victim environment 

# ENVIRONMENT

| Parameter   | Value    |
|--------------- | --------------- |
| Target   | Metasploitable  |
| Target IP   | 192.168.208.128   |
| Attacket IP   | 10.69.11.218   |
| Tool  |   Nmap    |

# METHODOLOGY

## Service Version Scanning

Command:
> nmap -O 192.168.208.128

Explanation:
- -O enables OS detection
- 192.168.208.128 to specify the host to be scanned

Observation:
- Returns information regarding the runnign services and its ports
- Host is found to be runnign the Linux kernel of version 2.6.X

# RESULTS

Evidences: Evidence/OSScan.txt

# MITRE ATTACK MAPPING

| Field | Mapping |
| -------------- | --------------- |
| Tactic | Reconaissance(TA0043) |
| Technique | Active Scanning (T1595) |
| Sub-Technique | Scanning IP Blocks (T1595.001) |

# CONCLUSIONS
- Infornation regarding the kernel has been found
- The information provides new avenue for exploitng vulnerabilites this version of the kernel







