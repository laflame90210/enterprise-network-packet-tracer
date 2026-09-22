# Multi-Site Enterprise Network

**Cisco Packet Tracer · Routing & Switching · Network Security**

## Overview

Designed and configured a simulated enterprise network across five sites: Dublin, Cork, Galway, Limerick, and Edinburgh. This Winter 2026 academic project combines departmental segmentation, WAN connectivity, redundancy, wireless access, and centralized services.

**Status:** Completed academic project, documented in the Packet Tracer technical report.

## Network design

| Site | Role and design |
| --- | --- |
| Dublin | Headquarters, departmental VLANs, Layer 3 distribution, access switches, and Internet gateway |
| Cork | Dual-stack IPv4/IPv6 branch |
| Galway | Routed branch connectivity |
| Limerick | Wireless branch with a WLC and three lightweight access points |
| Edinburgh | Large branch network with two routers and HSRP redundancy |

The addressing plan uses VLSM. Dublin separates Accounting, Human Resources, Sales, and IT Support into VLANs.

## Main configurations

- VLANs, VTP v2, inter-VLAN routing, and LACP EtherChannel.
- Multi-area OSPF across the enterprise.
- DHCP for client addressing and DHCPv6 in the dual-stack branch.
- HSRP active/standby gateway redundancy at Edinburgh.
- Serial WAN links with PPP authentication.
- NAT/PAT for Internet access.
- Extended ACLs for departmental and Internet access policies.
- Zone-based firewall configuration on the Dublin router.
- AAA/RADIUS-backed SSH administration.
- Wireless controller and lightweight access points at Limerick.

## Verification recorded in the report

- OSPF neighbors reached FULL and branch routes appeared in routing tables.
- DHCP clients received addressing, gateway, and DNS information.
- Cork clients received IPv4 and IPv6 addressing.
- HSRP showed active and standby routers.
- PPP links showed an operational line protocol.
- SSH access from the IT Support network succeeded.
- A Sales workstation successfully browsed the simulated Internet service.
- The controller reported all three wireless access points up.

## Learning outcomes

This project strengthened my skills in VLSM planning, routing across multiple sites, Layer 2 and gateway redundancy, access controls, and systematic connectivity checks.

## Documentation scope

The portfolio summary is based on the final technical report. A downloadable Packet Tracer file for this specific five-site project is not included in this repository.

Some course configurations use legacy technologies, including WEP and PAP. They are recorded as part of the assignment, not presented as recommended production security settings. VPN connectivity appeared in the project requirements; it is not claimed here as independently validated without a specific supporting test result.

See also my earlier [CCNA and CCNA Security Packet Tracer projects](https://github.com/laflame90210/cisco-networking-labs).


---
[Back to my portfolio](https://github.com/laflame90210)
