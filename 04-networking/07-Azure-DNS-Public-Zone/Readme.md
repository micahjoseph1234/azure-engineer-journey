# Lab 07 - Azure DNS Public Zone and A Record

## Objective

Learn how Azure DNS works by creating a public DNS zone, adding an A record, and verifying DNS name resolution.

---

## Resources Created

* Resource Group: rg-dns-lab01
* Azure DNS Zone: micahdns12345.com
* A Record: www
* IP Address: 10.10.10.10

---

## Steps Performed

### Step 1 - Create Resource Group

Created a new resource group:

```text
rg-dns-lab01
```

### Step 2 - Create Azure DNS Zone

Created a public DNS zone:

```text
micahdns12345.com
```

Azure automatically created:

* NS Record
* SOA Record

### Step 3 - Review Default Records

Verified the default DNS records created by Azure:

* NS (Name Server)
* SOA (Start of Authority)

### Step 4 - Create A Record

Created an A record with the following configuration:

```text
Name: www
Type: A
TTL: 1 Hour
IP Address: 10.10.10.10
```

### Step 5 - Verify Name Resolution

Copied one of the Azure DNS name servers and verified DNS resolution using:

```bash
nslookup www.micahdns12345.com <name-server>
```

Expected result:

```text
10.10.10.10
```

---

## Key Learnings

* Azure DNS hosts DNS zones in Azure.
* DNS Zones contain DNS records.
* NS records identify authoritative name servers.
* SOA records define DNS zone authority.
* A records map domain names to IPv4 addresses.
* TTL controls how long DNS responses are cached.
* Azure automatically creates NS and SOA records when a DNS zone is created.

---

## Interview Questions

### What is Azure DNS?

Azure DNS is a hosting service for DNS domains that provides name resolution using Azure infrastructure.

### What is an A Record?

An A Record maps a hostname to an IPv4 address.

### What is the purpose of an NS Record?

NS records specify the authoritative name servers responsible for a DNS zone.

### What is the purpose of TTL?

TTL (Time To Live) determines how long DNS records are cached before being refreshed.

### Difference between Public DNS and Private DNS?

Public DNS is accessible from the internet.

Private DNS is accessible only from linked Azure VNets.

---

## Screenshots

1. 01-rg-created.png
2. 02-dns-zone-created.png
3. 03-default-recordsets.png
4. 04-a-record-created.png
5. 05-nameservers.png
6. 06-nslookup-success.png

---

## Cleanup

Deleted:

```text
rg-dns-lab01
```

to avoid unnecessary Azure charges.

---

## AZ-104 Exam Relevance

* Azure DNS
* DNS Zones
* Record Sets
* A Records
* NS Records
* DNS Resolution
* Public DNS Services
