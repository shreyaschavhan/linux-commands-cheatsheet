## 𝐧𝐦𝐚𝐩 𝐂𝐡𝐞𝐚𝐭𝐬𝐡𝐞𝐞𝐭:

- Basic scans: 
> - `nmap <hostip>` - Scan Single IPs
> - `nmap <hostip1> <hostip2>` - Scan Specific IPs 
> - `nmap 192.168.1.1-254` - Scan a Range
> - `nmap scanme.domain.name` - Scan a domain
> - `nmap 192.168.1.0/24` - Scan using CIDR notation
> - `nmap -iL targets.txt` - Scan targets from a file
> - `nmap -iR 100` - Scan 100 random hosts
> - `nmap --exclude 192.168.1.1` - Excude listed host

---
- Scan Techniques:
> - `nmap 192.168.1.1 -sS` - TCP SYN port scan
