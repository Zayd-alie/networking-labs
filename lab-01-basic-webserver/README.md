# Lab 01 – Basic Network with Web Server

## Lab Goal
The goal of this lab is to demonstrate basic network communication within a single Local Area Network (LAN).  
It shows how end devices communicate through a switch and how a client accesses a web server using an IP address.

This lab focuses on **Layer 2 communication** and does not require routing.

---

## Topology Overview
The network consists of:
- One Layer 2 switch
- Two client PCs
- One web server
- One network printer

All devices are connected to the same layer 3 switch and belong to the same IP subnet.

---

## IP Addressing
All devices are configured in the `192.168.1.0/24` network:

- PC1: `192.168.1.1`
- PC2: `192.168.1.2`
- Web Server: `192.168.1.3`
- Printer: `192.168.1.4`

The web server and printer use **static IP addresses** (manually set IPs) because they provide services on the network, tho i also used static IPs with PCs.

---

## How Communication Works
When PC1 accesses the web server using `http://192.168.1.3`:

1. PC1 checks that the destination IP is in the same subnet.
2. PC1 uses ARP (Address Resolution Protocol) to find the MAC address of the web server.
3. The switch forwards frames based on its MAC address table.
4.The web server receives the HTTP request and responds with the web page.

Because all devices are in the same LAN, **no router or default gateway is required**.

## Verification Steps
- Ping the web server from PC1 and PC2
- Open a web browser on PC1
- Navigate to `http://192.168.1.3`
- Confirm the web page loads successfully

---

## CCNA Concepts Covered
- LAN fundamentals
- Layer 2 switching
- IP addressing and subnetting basics
- ARP operation
- Client-to-server communication
- When routing is NOT required

---

## Notes
This lab builds a foundation for future topics such as VLANs, routing, and inter-VLAN communication.


