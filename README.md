# security

### CVE-2020-1559
#### Private Internet Access VPN for Linux - Exposure of Sensitive Information to an Unauthorized Actor

A vulnerability in the Private Internet Access (PIA) VPN Client for Linux v1.5 through v2.3+ allows remote attackers to bypass an intended VPN kill switch mechanism and read sensitive information via intercepting network traffic. Since v1.5, PIA has supported a "split tunnel" OpenVPN bypass option. The PIA killswitch & associated iptables firewall is designed to protect you while using the Internet. When the kill switch is configured to block all inbound and outbound network traffic, privileged applications can continue sending & receiving network traffic if net.ipv4.ip_forward has been enabled in the system kernel parameters. For example, a Docker container running on a host with the VPN turned off, and the kill switch turned on, can continue using the internet, leaking the host IP (CWE 200). In PIA 2.4.0+, policy-based routing is enabled by default and is used to direct all forwarded packets to the VPN interface automatically.

**CVE-2020-15590** https://github.com/sickcodes/security/blob/master/advisories/SICK-2020-001.md

### CVE-2020-27402
#### Hindotech HK1 TV Box - Root Privilege Escalation - Improper Access Control

The HK1 Box S905X3 TV Box contains a vulnerability that allows a local unprivileged user, such as a malicious APK, to escalate to root using the /system/xbin/su binary. While connected to the device through the serial port (UART), or while using adb as an unprivileged user, the local attacker can execute the /system/xbin/su binary and execute arbitrary code as root, steal social networking account tokens, WiFi passwords, cookies, saved passwords, user location data, message history, emails, or contacts, etc.

**CVE-2020-27402** https://github.com/sickcodes/security/blob/master/advisories/SICK-2020-004.md

### CVE-2020-8276
#### Exposure of Sensitive Information to an Unauthorized Actor - Brave Browser Potentially Logs The Last Time A Tor Window Was Used.

A vulnerability in the Brave Browser allows an attacker to view the last time a Tor session was used in incognito mode. A local, on-disk attacker could read the Brave Browser's "Local State" json file and identify the last time a Tor session was used, affecting the confidentiality of a user's Tor session.

**CVE-2020-8276** https://github.com/sickcodes/security/blob/master/advisories/SICK-2020-013.md


### CVE-2020-27403
#### Exposure of Information Through Directory Listing - TCL Android TV Filesystem Browsable to Unauthenticated Attackers Over the Adjacent Network on Port 7989

A vulnerability in the TCL Android Smart TV series by TCL Technology Group Corporation allows an attacker on the adjacent network to arbitrarily browse and download sensitive files over an insecure web server running on port 7989 that lists all files & directories.

**CVE-2020-27403** https://github.com/sickcodes/security/blob/master/advisories/SICK-2020-009.md


### CVE-2020-28055
#### Incorrect Permission Assignment for Critical Vendor Resources - TCL Android TV Vendor Configuration & Upgrade Folders World Writable to Local Attacker

A vulnerability in the TCL Android Smart TV series by TCL Technology Group Corporation allows a local unprivileged attacker, such as a malicious App, to read and write to critical vendor resource directories within the Android TV file system, including the vendor upgrades folder.

**CVE-2020-28055** https://github.com/sickcodes/security/blob/master/advisories/SICK-2020-012.md





