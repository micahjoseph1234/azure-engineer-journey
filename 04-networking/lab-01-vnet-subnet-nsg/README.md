# Lab 01 - Virtual Network, Subnet and NSG

## Objective

Create a Virtual Network with multiple subnets and secure it using a Network Security Group.

## Resources Created

* Resource Group: rg-networking-lab01
* Virtual Network: vnet-lab01
* Address Space: 10.0.0.0/16
* Subnet-Web: 10.0.1.0/24
* Subnet-DB: 10.0.2.0/24
* Network Security Group: nsg-web

## Steps Performed

### Step 1 - Create Resource Group

Created a Resource Group named rg-networking-lab01 in Central India.

### Step 2 - Create Virtual Network

Created vnet-lab01 with address space 10.0.0.0/16.

### Step 3 - Create Subnets

Created:

* subnet-web (10.0.1.0/24)
* subnet-db (10.0.2.0/24)

### Step 4 - Create NSG

Created nsg-web.

### Step 5 - Create Inbound Rule

Created Allow-HTTP rule.

Priority: 100

Action: Allow

### Step 6 - Associate NSG

Associated nsg-web with subnet-web.

## Key Learnings

* VNet is Azure's private network.
* Subnets logically divide a VNet.
* NSGs act as virtual firewalls.
* Lower priority number has higher precedence.

## Screenshots

* 01-vnet-overview.png
* 02-subnets-created.png
* 03-nsg-created.png
* 04-http-rule-created.png
* 05-nsg-subnet-association.png

## Cleanup

Deleted Resource Group after completing networking labs.
