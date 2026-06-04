# AZ-104 Networking - Routing, UDRs, NVA and Gateway Transit

## Objective

Learn Azure networking concepts related to routing, traffic flow control, virtual network peering, gateway transit, user-defined routes (UDRs), service chaining, and network virtual appliances (NVAs).

---

## Topics Covered

### Azure DNS

* DNS Zones
* A Records
* CNAME Records
* NS Records
* SOA Records
* DNS Delegation
* Alias Records
* Private DNS Zones

### Virtual Network Peering

* Regional Peering
* Global Peering
* Peering Requirements
* Non-Transitive Peering
* DNS Considerations in Peered VNets

### Gateway Transit

* Hub and Spoke Architecture
* Allow Gateway Transit
* Use Remote Gateway
* Shared VPN Gateway Design

### Azure Routing

* System Routes
* Route Tables
* Route Selection
* Longest Prefix Match
* Route Priority

  * User Defined Routes (UDR)
  * BGP Routes
  * System Routes

### User Defined Routes (UDRs)

* Custom Traffic Routing
* Next Hop Types

  * Virtual Appliance
  * Virtual Network Gateway
  * Virtual Network
  * Internet
  * None

### Service Chaining

* Routing Traffic Through Security Appliances
* Hub-Spoke Security Design

### Network Virtual Appliances (NVA)

* Firewall Appliances
* Traffic Inspection
* IP Forwarding
* Microsegmentation
* DMZ Architecture

### Additional Concepts

* Jumpbox / Bastion Host
* DMZ Networks
* Azure Service Endpoints
* Border Gateway Protocol (BGP)
* Service Tags

---

## Key Learnings

* Azure creates system routes automatically.
* UDRs can override default routing behavior.
* Longest prefix match always wins during route selection.
* If prefixes are equal, Azure prioritizes:

  1. User Defined Routes
  2. BGP Routes
  3. System Routes
* Gateway Transit enables spoke VNets to use a hub VPN Gateway.
* VNet Peering is non-transitive.
* Service Chaining forces traffic through security appliances.
* NVAs require IP Forwarding to route traffic.
* DMZ networks act as security boundaries between public and private resources.
* Jumpboxes provide secure administrative access to private resources.

---

## Lab Progress

### Completed

* Created Route Table
* Created Custom Route
* Created Virtual Network
* Created Public Subnet
* Created Private Subnet
* Created DMZ Subnet
* Associated Route Table with Public Subnet

### In Progress

* NVA Deployment
* IP Forwarding Configuration
* Traffic Routing Validation

---

## AZ-104 Exam Notes

### High-Yield Concepts

* DNS Delegation
* Alias Records
* VNet Peering
* Gateway Transit
* Route Tables
* User Defined Routes
* NVA Architecture
* BGP
* Service Endpoints

### Common Exam Rules

#### Gateway Transit

Hub:

* Allow Gateway Transit

Spoke:

* Use Remote Gateway

#### Route Selection

1. Longest Prefix Match
2. UDR > BGP > System Route

#### NVA Deployment

* Deploy in DMZ Subnet
* Enable IP Forwarding
* Route Traffic Using UDRs

---

## Next Steps

* Complete NVA Deployment Lab
* Validate Routing Using Traceroute
* Continue Networking Module:

  * NSGs
  * Azure Load Balancer
  * Application Gateway
  * Azure Firewall
  * NAT Gateway
