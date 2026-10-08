## Nmap Host Discovery

Kali Linux was connected to the local lab network with the IP address `192.168.100.108`.

Nmap host discovery was performed using:

`nmap -sn 192.168.100.0/24`

The scan discovered 9 active hosts on the local network.

![Nmap Host Discovery](screenshots/01-nmap-host-discovery.png)

## Nmap Basic Port Scan

A basic Nmap TCP port scan was performed against the authorized Windows lab machine at `192.168.100.66`.

The command used was:

`nmap 192.168.100.66`

Nmap confirmed that the host was online, but all 1000 default TCP ports were reported as filtered.

This indicated that the Windows Firewall was filtering the incoming scan traffic and preventing Nmap from receiving normal port responses.

![Nmap Basic Port Scan](screenshots/02-nmap-basic-port-scan-filtered.png)
