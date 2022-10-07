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
- Scans:
> - `nmap -sP 10.7.1.0/24` : ping multiple ips at once
> - `nmap -p <port(s)> <hostaddress` : scan specific ports
> - `nmap -sT <host>` : TCP (full open) scan - using full 3 way handshake
> - `nmap -sS -p <port(s)> <host>` - Stealthy scan (don't let TCP 3 way handshake complete to avoid getting caught.
> - `nmap -O <host>` : OS Detection
> - `nmap -A <host>`: OS Detection + Version Detection + Script Scanning + traceroute 
> - `nmap -sV <host>` : Service version detection
> - `nmap -D <decoy ip> <host>`: Add Decoy
> - `nmap --script ssl-enum-ciphers -p <port> <host>` : Check SSL


Foot notes:
1. https://www.youtube.com/watch?v=4t4kBkMsDbQ

---

## Updates:

- By [Marv](https://www.reddit.com/user/MrK_GER/) 
- Suggestion: [here](https://www.reddit.com/r/oscp/comments/xwgmal/comment/irb9jnz/?utm_source=share&utm_medium=web2x&context=3)
```
nmap -sV -Sc -oA nmap/ <hostip>
```
```
-sV ==> Version detection
-sC ==> Run default scripts
-oA ==> Save the output in all formats
```
