# Lab 03 - NSG Priority Rules

## Objective

Understand how Azure NSG priorities determine which rule is applied.

## Resources Used

* nsg-web

## Steps Performed

### Step 1

Created Allow-SSH rule.

Priority: 200

Action: Allow

### Step 2

Created Deny-SSH rule.

Priority: 300

Action: Deny

### Step 3

Observed that Allow-SSH wins because priority 200 is higher than 300.

### Step 4

Modified Deny-SSH priority to 150.

### Step 5

Observed that Deny-SSH wins because priority 150 is higher than 200.

## Key Learnings

* Lower priority number wins.
* Azure processes NSG rules in priority order.
* Rule conflicts are resolved using priority.

## Screenshots

* 09-allow-ssh-rule.png
* 10-deny-ssh-rule.png
* 11-priority-demo.png

## Interview Questions

### Which rule wins?

Allow SSH 200

Deny SSH 150

Answer: Deny SSH 150
