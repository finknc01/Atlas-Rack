# Mission 05 — What Fails Together?

## Briefing
Northstar management asks whether the rack is redundant. That word means nothing until you name the failure.

## Objective
Identify shared failure domains across power, cooling, switching, management, and compute.

## Tasks
Create a failure-mode table for loss of one feed/PDU, one switch, one uplink, one cooling component, one management path, and one compute node. Mark whether capacity degrades or service is lost.

## Twist
Discover one hidden common dependency in your design—two “redundant” paths using the same upstream component—and redesign it or explicitly accept the risk.

## Evidence
- failure-domain diagram
- N/N+1/A-B assumptions
- degraded-capacity table
- accepted residual risks

## Victory condition
You can answer “redundant against what?” for every duplicated component.
