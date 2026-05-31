# Lab 02 - VNet Peering

## Objective

Establish private communication between two Azure VNets.

## Resources Created

* vnet-lab01
* vnet-dev

## Configuration

### VNet 1

Address Space: 10.0.0.0/16

### VNet 2

Address Space: 10.1.0.0/16

### Subnet

subnet-dev (10.1.1.0/24)

## Steps Performed

### Step 1

Created vnet-dev.

### Step 2

Configured peering from:

vnet-lab01 → vnet-dev

### Step 3

Configured reciprocal peering:

vnet-dev → vnet-lab01

### Step 4

Verified peering status as Connected.

## Key Learnings

* VNets are isolated by default.
* Peering enables private communication.
* Overlapping address spaces are not allowed.
* Peering provides low latency communication.

## Screenshots

* 06-vnet-dev-created.png
* 07-peering-created.png
* 08-peering-reciprocal.png

## Cleanup

Deleted Resource Group after lab completion.
