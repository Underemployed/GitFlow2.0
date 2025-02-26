Exp No: 3
Date:
Study of IPv4 & IPv6 Addresses

Aim: To study IPv4 and IPv6 addressing schemes and subnetting.

Hardware Addressing:
A hardware address uniquely identifies a host within a local network. It functions at the Data-Link layer (Layer-2) of the OSI model. Ethernet uses a 48-bit MAC address, represented in hexadecimal:
00:43:AB:F2:32:13 or 0043.ABF2.3213

Logical Addressing:
Logical addresses operate at the Network layer (Layer-3) and provide a hierarchical structure for networks. Unlike hardware addresses, they are dynamic. A logical address has:
- Network ID: Identifies the network.
- Host ID: Uniquely identifies the host.
IPv4 uses a 32-bit address, e.g., 158.80.164.3

Subnet Mask:
A subnet mask differentiates the network and host portions of an IP address.
Example:
158.80.164.3 255.255.0.0
Binary Representation:
IP Address: 10011110.01010000.10100100.00000011
Subnet Mask: 11111111.11111111.00000000.00000000

IP Address Classes:
IPv4 addresses are structured into classes, determined by the first octet.

CIDR (Classless Inter-Domain Routing):
CIDR notation appends a mask to an IP, e.g., 192.168.1.1/24.

Subnetting:
Subnetting creates subnets by borrowing bits from the host portion.
Example (4 subnets from 192.168.254.0/24):
192.168.254.0 - 192.168.254.63  255.255.255.192
192.168.254.64 - 192.168.254.127  255.255.255.192
192.168.254.128 - 192.168.254.191  255.255.255.192
192.168.254.192 - 192.168.254.255  255.255.255.192

IPv6 Addressing:
IPv6 uses 128-bit addresses, providing an almost unlimited supply.
Features:
- Increased Address Space
- Auto-configuration
- Built-in Security
- IPv4 Compatibility
Example IPv6 Address:
1254:1532:26B1:CC14:0123:1111:2222:3333

IPv6 Address Compression:
Leading zeros can be omitted:
1423:0021:0C13:CC1E:3142:0001:2222:3333 → 1423:21:C13:CC1E:3142:1:2222:3333
Zero fields can be condensed:
F12F:0000:0000:CC1E:2412:1111:2222:3333 → F12F::CC1E:2412:1111:2222:3333

IPv6 Prefix:
Uses CIDR notation:
Full Address: 1254:1532:26B1:CC14:123:1111:2222:3333/64
Prefix ID: 1254:1532:26B1:CC14:
Host ID: 123:1111:2222:3333

Result: The study of IPv4 & IPv6 addressing has been completed.

