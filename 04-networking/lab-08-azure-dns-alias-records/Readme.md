# Lab 08 - Azure DNS Alias Records

## Objective

Understand how Azure DNS Alias Records work and how they can be used to map DNS names directly to Azure resources such as Public IP Addresses, Load Balancers, Application Gateways, and Traffic Manager profiles.

---

## Resources Studied

* Azure DNS Zone
* Alias Record
* Public IP Address
* Azure Load Balancer
* DNS Zone Apex

---

## Concept Overview

Traditional DNS records map directly to IP addresses.

Example:

```text
www.contoso.com
      ↓
20.100.10.5
```

If the IP address changes, the DNS record must be updated manually.

Azure Alias Records solve this problem by pointing directly to Azure resources.

Example:

```text
contoso.com
     ↓
Alias Record
     ↓
Azure Load Balancer
```

Azure automatically updates the DNS mapping if the underlying resource IP changes.

---

## Alias Record Benefits

* Automatic DNS updates
* No manual IP maintenance
* Direct integration with Azure resources
* Improved reliability
* Useful for zone apex records

---

## Supported Azure Resources

Alias records can point to:

* Public IP Addresses
* Azure Load Balancers
* Application Gateways
* Traffic Manager Profiles
* Azure CDN Endpoints

---

## Zone Apex

Zone Apex refers to the root domain.

Example:

```text
contoso.com
```

instead of:

```text
www.contoso.com
```

Alias records are commonly used at the zone apex.

---

## Interview Questions

### What is an Alias Record?

An Alias Record maps a DNS record directly to an Azure resource instead of a fixed IP address.

### Why use Alias Records?

To automatically track Azure resource IP changes and eliminate manual DNS updates.

### What is a Zone Apex?

The root domain of a DNS zone.

Example:

```text
contoso.com
```

### What Azure resources can Alias Records point to?

Public IPs, Load Balancers, Application Gateways, Traffic Manager profiles, and other supported Azure resources.

### Difference between A Record and Alias Record?

A Record points directly to an IP address.

Alias Record points to an Azure resource and automatically updates when the resource IP changes.

---

## Key Learnings

* Alias Records simplify DNS management.
* Alias Records remove dependency on static IP addresses.
* Alias Records are commonly used with Load Balancers.
* Alias Records support zone apex mappings.

---

## Screenshots

* Azure DNS Zone Overview
* DNS Record Sets
* Alias Record Configuration (Theory Reference)

---

## Cleanup

No Azure resources were deployed specifically for this lab.

The concept was studied theoretically to optimize Azure costs and study efficiency.

---

## AZ-104 Exam Relevance

* Azure DNS
* Alias Records
* Zone Apex
* Public DNS Management
* Azure Networking
