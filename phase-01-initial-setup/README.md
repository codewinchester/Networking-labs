# Phase 1: Initial Office Setup

## 1. Background Story
Senior Partner Harvey has just opened a small law office. Right now, it's a tight team: Harvey, a junior partner, one paralegal, and a receptionist. They bought a few computers and a network printer so they can print out legal briefs. They need a simple local network set up so everyone can talk to each other and print without hassle. 

## 2. Simple Requirements
* **Automatic Setup:** Automatic IP address assignment
* **Reserved Printer IP:** Static IP assignment.
* **Room to Grow:** The setup needs to allow them to add more computers easily later on without having to change the whole network configuration.

## 3. Network Topology
![Phase 1 Topology](./topology.png)

## 4. IP Addressing Scheme

* **Network Range:** 192.168.10.0/24
* **Network ID:** 192.168.10.0
* **Broadcast Address:** 192.168.10.255
* **Subnet Mask:** 255.255.255.0
* **Default Gateway (R2):** 192.168.10.1 (Static)
* **Network Printer (InkPrinter):** 192.168.10.10 (Static)
* **Excluded Range:** 192.168.10.1 to 192.168.10.10 (Reserved for infrastructure)
* **DHCP Pool Scope (STAFF):** 192.168.10.11 to 192.168.10.254 (Dynamic assignment for staff PCs)