# Lab 02 – How Switches Work (MAC Learning & Frame Forwarding)

## Lab Goal

The goal of this lab is to demonstrate how Layer 2 switches learn MAC addresses
and forward Ethernet frames within a local area network (LAN).

This lab focuses on **switch behavior before VLANs**, including:
- MAC address table learning
- Frame flooding vs unicast forwarding
- Traffic flow across multiple switches

No routing or VLAN configuration is used.

---

## Topology Overview

The network consists of:
- Two Layer 2 switches connected together
- Multiple end devices (PCs, laptops, printer, server)
- A single IP subnet: `192.168.0.0/24`

All devices are connected to switches and communicate using Ethernet frames.

---

## Initial State

- Both switches start with **empty MAC address tables**
- No device MAC addresses are known
- Any unknown destination traffic must be flooded

---

## Simulation Task

Using **Simulation Mode** in Packet Tracer:

1. Send a ping from **PC1** to **PC3**
2. Observe how frames move through the switches
3. Answer the questions below based on what you see

---

## Questions to Answer

1. Which MAC address does each switch learn first, and on which port?
2. Why is the first frame flooded across multiple ports?
3. After the first ping, how does the forwarding behavior change?
4. Why does the return traffic no longer get flooded?

---

## Key Observations

- Switches learn MAC addresses from the **source MAC** of incoming frames
- Unknown destination MACs cause **flooding**
- Known destination MACs result in **unicast forwarding**
- MAC tables are built dynamically based on traffic flow

---

## Why This Matters (Real World)

Understanding MAC learning is critical because:
- VLANs, trunking, and STP all build on this behavior
- Misunderstanding flooding leads to poor network design
- Switch efficiency depends on accurate MAC tables

This is foundational knowledge for CCNA and real enterprise networks.
