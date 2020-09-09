# security

### CVE-2020-15590 Private Internet Access VPN for Linux - Exposure of Sensitive Information to an Unauthorized Actor
A vulnerability in the Private Internet Access (PIA) VPN Client for Linux v1.5 through v2.3+ allows remote attackers to bypass an intended VPN kill switch mechanism and read sensitive information via intercepting network traffic. Since v1.5, PIA has supported a "split tunnel" OpenVPN bypass option. The PIA killswitch & associated iptables firewall is designed to protect you while using the Internet. When the kill switch is configured to block all inbound and outbound network traffic, privileged applications can continue sending & receiving network traffic if net.ipv4.ip_forward has been enabled in the system kernel parameters. For example, a Docker container running on a host with the VPN turned off, and the kill switch turned on, can continue using the internet, leaking the host IP (CWE 200). In PIA 2.4.0+, policy-based routing is enabled by default and is used to direct all forwarded packets to the VPN interface automatically.

**CVE-2020-15590** https://github.com/sickcodes/security/blob/master/advisories/SICK-2020-001.md


