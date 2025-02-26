# Exp No: 3
**Date:**

## Study of IPv4 & IPv6 Addresses

### Aim:
To study IPv4 and IPv6 addressing schemes and subnetting.

### Hardware Addressing
A MAC address uniquely identifies a host in a local network (Layer-2). It is a 48-bit hexadecimal address:
- 00:43:AB:F2:32:13
- 0043.ABF2.3213

### Logical Addressing
Logical addresses (Layer-3) provide hierarchical structuring. An IPv4 address consists of:
- **Network ID** – Identifies the network.
- **Host ID** – Identifies the host.

IPv4 uses a 32-bit address (e.g., 158.80.164.3).

### Subnet Mask
Separates network and host parts of an IP address:
- Example: 158.80.164.3 255.255.0.0
- Binary format:
  - **IP Address:** 10011110.01010000.10100100.00000011
  - **Subnet Mask:** 11111111.11111111.00000000.00000000

### IP Address Classes & CIDR
IPv4 addresses are classified based on the first octet. CIDR notation represents subnet masks, e.g.,
- **192.168.1.1/24** (Subnet mask: 255.255.255.0)

### Subnetting
Dividing networks into smaller subnets:
- Example: **192.168.254.0/26**
  - 192.168.254.0 - 192.168.254.63
  - 192.168.254.64 - 192.168.254.127
  - 192.168.254.128 - 192.168.254.191
  - 192.168.254.192 - 192.168.254.255

### IPv6 Addressing
IPv6 uses 128-bit addresses, providing a vast address space. Features:
- **Auto-configuration**
- **Built-in security**
- **IPv4 compatibility**

Example:
- **Full:** 1254:1532:26B1:CC14:0123:1111:2222:3333
- **Condensed:** 1254:1532:26B1:CC14:123:1111:2222:3333
- **Further compressed:** F12F::CC1E:2412:1111:2222:3333

### IPv6 Prefix
Uses CIDR notation, e.g.,
- **Full Address:** 1254:1532:26B1:CC14:123:1111:2222:3333/64
- **Prefix ID:** 1254:1532:26B1:CC14
- **Host ID:** 123:1111:2222:3333

### Result
The study of IPv4 & IPv6 addressing has been completed.
