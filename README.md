# Networking Labs

This repository contains hands-on networking labs aligned with the CCNA syllabus.  
The goal is to build deep, practical understanding of how networks actually work — not just to copy labs or commands.

## What this repository is
- Step-by-step networking labs with clear explanations
- Focus on Layer 2 and Layer 3 fundamentals
- Each lab explains *why* configurations exist, not just the commands

## Topics covered
- Basic LAN design and IP addressing
- Switching fundamentals (MAC learning, VLANs, trunking)
- Spanning Tree Protocol (STP, RSTP)
- EtherChannel
- Routing fundamentals (static routing, inter-VLAN routing)
- Basic troubleshooting scenarios

## Structure
Each lab lives in its **own folder** and is fully self-contained.

networking-labs/
├── lab-01-basic-webserver/
│ ├── README.md
│ └── *.pkt
├── lab-02-how-switches-work/
│ ├── README.md
│ └── *.pkt
└── README.md


Each lab folder contains:
- A `README.md` explaining the goal, topology, and concepts
- A Cisco Packet Tracer (`.pkt`) file with the lab topology

## How to use this repository
1. Open a lab folder (e.g. `lab-01-basic-webserver`)
2. Read the `README.md` to understand the goal and concepts
3. Open the `.pkt` file in Cisco Packet Tracer
4. Explore the topology and test connectivity

