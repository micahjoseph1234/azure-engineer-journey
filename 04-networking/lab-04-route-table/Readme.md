# Lab 04 - Route Tables (UDR)

## Objective

Create a Route Table and associate it with a subnet.

## Resources Created

* Route Table: rt-networking-lab01

## Steps Performed

### Step 1

Created Route Table named rt-networking-lab01.

### Step 2

Created Route:

Route Name: route-internet

Address Prefix: 0.0.0.0/0

Next Hop Type: Internet

### Step 3

Associated Route Table with subnet-web.

## Key Learnings

* UDR stands for User Defined Route.
* Route Tables control traffic flow.
* 0.0.0.0/0 represents all traffic.
* Route Tables are associated with subnets.

## Screenshots

* 12-route-table-created.png
* 13-route-added.png
* 14-route-table-associated.png

## Interview Questions

### What does UDR stand for?

User Defined Route

### What does 0.0.0.0/0 represent?

All traffic.

### Can a Route Table be attached directly to a VM?

No. Route Tables are attached to subnets.
