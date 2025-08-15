# PlanetSide ZERO

## Overview
This tool:
- Intercepts network packets in Planetside 2 to capture user IP addresses.
- Exploits server vulnerabilities to access account details from serialized UUIDs obtained using voice communication connections.
- Accesses and reads database SQL data via exploit 0x-- from VoIP communication login packets from server injection.

## Features
- **Packet Sniffing**: Captures and analyzes network packets to extract user IPs.
- **Voice Communication Exploitation**: Retrieves serialized UUIDs linked to user accounts from voice connections.
- **Server Exploitation**: Accesses sensitive account data via server-side vulnerabilities.

## Prerequisites
- Python 3.8+
- Libraries: `scapy`, `requests`, `pyshark`
- A controlled testing environment (e.g., private Planetside 2 server)
- Knowledge of network protocols, UUID serialization, and voice communication systems
