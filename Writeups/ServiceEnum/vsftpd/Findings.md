# Findings
- Found to have a backdoor vulnerability that provides access to root shell

# Exploit Methodology
- Backdoor shell opens at port 6200 on login to ftp with any username that ends with ":)"
- connect to the shell with nc or telnet


# CVE Mapping

| CVE | Description | CVSS | Affected Services |
| --------------- | --------------- | --------------- | --------------- |
| CVE-2011-2523 | A backdoor execution vulnerability | 9.8 | vsftpd 2.3.4 |

