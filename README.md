# PlanetSide ZERO

## Overview
This tool:
- Intercepts network packets in Planetside 2 to capture user IP addresses.
- Exploits server vulnerabilities to access account details from serialized UUIDs obtained through voice communication connections.

## Features
- **Packet Sniffing**: Captures and analyzes network packets to extract user IPs.
- **Voice Communication Exploitation**: Retrieves serialized UUIDs linked to user accounts from voice connections.
- **Server Exploitation**: Accesses sensitive account data via server-side vulnerabilities.

## Prerequisites
- Python 3.8+
- Libraries: `scapy`, `requests`, `pyshark`
- A controlled testing environment (e.g., private Planetside 2 server)
- Knowledge of network protocols, UUID serialization, and voice communication systems

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/SoggyCow/PlanetSide-2.git
   ```
2. Navigate to the project directory:
   ```bash
   cd PlanetSide-2
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
1. Run the packet sniffer to capture IPs and UUIDs from voice communications:
   ```bash
   python packet_sniffer.py --interface eth0 --filter voice
   ```
2. Execute the server exploit script to target vulnerabilities:
   ```bash
   python server_exploit.py --target <server_ip> --port 8080
   ```
3. Review extracted data in the `output/` folder.
