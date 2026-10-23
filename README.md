# BRACU Network Design — CSE421

A Cisco Packet Tracer networking project that models a multi-department BRAC University network. The project includes a Packet Tracer topology, an IP addressing plan, and router configuration commands.

## Project Overview

The network connects six departmental LANs:

- CSE — `17.16.1.0/24`
- BBS — `17.16.2.0/24`
- MNS — `17.16.3.0/24`
- BIL — `17.16.4.0/24`
- EEE — `17.16.5.0/24`
- LAW — `17.16.6.0/24`

The design uses a central CSE router, a core network, and point-to-point links to connect departmental networks. The project report documents device addressing and router configurations.

## Project Files

- `cse421project.pkt` — Cisco Packet Tracer network simulation.
- `2206_CSE421 Project.pdf` — Project report with the topology, IP address table, and router configuration commands.
- `image.webp` — Network topology screenshot.
- `83adef93-3452-4261-94e0-1e2ad6572121.jpg` — Hand-drawn planning/topology diagram.

## Technologies and Concepts

- Cisco Packet Tracer
- IPv4 addressing and subnet masks
- LAN design and router interconnection
- DHCP configuration
- Static routing
- RIP version 2
- Network services such as DNS, web, and email servers
- Network troubleshooting and connectivity testing

## IP Addressing Summary

| Department / Link | Network |
|---|---|
| CSE LAN | `17.16.1.0/24` |
| BBS LAN | `17.16.2.0/24` |
| MNS LAN | `17.16.3.0/24` |
| BIL LAN | `17.16.4.0/24` |
| EEE LAN | `17.16.5.0/24` |
| LAW LAN | `17.16.6.0/24` |
| CSE–MNS point-to-point link | `17.16.10.0/30` |
| CSE–LAW point-to-point link | `17.16.10.4/30` |
| CSE–BIL point-to-point link | `17.16.10.8/30` |
| Core network shown in report | `17.16.20.0/24` |

Refer to the PDF report for the full device-by-device IP address table and configuration commands.

## How to Open the Project

1. Install Cisco Packet Tracer.
2. Clone or download this GitHub repository.
3. Open `cse421project.pkt` in Cisco Packet Tracer.
4. Inspect the topology, routers, switches, PCs, printers, and servers.
5. Open router CLI windows to review the configurations.
6. Test connectivity with `ping` between devices on different LANs.
7. Verify DHCP, DNS, web, and email services where configured.

## Validation Checklist

Use these checks when reviewing or demonstrating the simulation:

- [ ] Router and switch interfaces are connected and enabled.
- [ ] PCs receive the expected IP settings where DHCP is configured.
- [ ] Default gateways match the router LAN interfaces.
- [ ] Routing tables contain routes to remote departmental networks.
- [ ] PCs can ping their default gateway.
- [ ] Devices in different departments can communicate where routing is intended.
- [ ] Configured DNS, web, and email services work as expected.

## Notes

This repository documents an academic network simulation. The actual behavior should be verified by opening the `.pkt` file in Cisco Packet Tracer and testing connectivity. The report and configuration excerpts may contain inconsistencies; confirm interface addressing, DHCP pools, routing, and the topology before treating the design as fully validated.

## Contributors

The original project report lists the project group. If publishing this repository publicly, consider whether you want to include student IDs and other personal details in the report.

## License

No license has been specified. Add a license if you want to define how others may reuse or modify the project.
