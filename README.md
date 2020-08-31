# security

### Private Internet Access VPN for Linux - Exposure of Sensitive Information to an Unauthorized Actor
A vulnerability in the Private Internet Access (PIA) VPN Client for Linux v1.5 through v2.3.1 allows remote attackers to bypass an intended VPN kill switch mechanism and read sensitive information via intercepting network traffic. Since v1.5, PIA has supported a "split tunnel" OpenVPN bypass option. When the kill switch is configured to block all inbound and outbound network traffic, privileged applications can continue sending & receiving network traffic which defeats the purpose of the kill switch. This cannot occur when using the standard OpenVPN configuration (.ovpn) files. For example, a Docker container running on a host with the VPN turned off, and the kill switch turned on, can continue using the internet, leaking the host IP (CWE 200).

**CVE-2020-15590** https://github.com/sickcodes/security/blob/master/advisories/SICK-2020-001.md
