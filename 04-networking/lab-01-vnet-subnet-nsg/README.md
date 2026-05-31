# Lab 01 - VNet, Subnet and NSG

## Objective

Create a Virtual Network with multiple subnets and secure it using a Network Security Group.

---

## Resources Created

- Resource Group: rg-networking-lab01
- Virtual Network: vnet-lab01
- Subnet-Web: 10.0.1.0/24
- Subnet-DB: 10.0.2.0/24
- Network Security Group: nsg-web

---

## Architecture

VNet (10.0.0.0/16)

├── subnet-web (10.0.1.0/24)

└── subnet-db (10.0.2.0/24)

NSG attached to subnet-web

---

## Key Learnings

- VNet is Azure's private network.
- Subnets divide a VNet into smaller logical networks.
- NSGs act as virtual firewalls.
- Lower priority number means higher priority.
- NSGs can be attached to a subnet or NIC.

---

## Interview Questions

### What is a VNet?

A private network in Azure used for secure communication between resources.

### What is a Subnet?

A logical division of a VNet.

### What is an NSG?

A virtual firewall that controls inbound and outbound traffic.

### What happens if two NSG rules conflict?

The rule with the lower priority number wins.

---

## Cleanup

Delete Resource Group after completing the lab.
