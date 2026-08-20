# Final — The Atlas Design Review

## Briefing
The rack faces a review board representing facilities, networking, operations, finance, and the AI platform team. Each group is allowed to challenge a different assumption.

## Required packet
- requirements/assumptions
- rack elevations
- BOM
- power/feed model
- heat/cooling path
- port/cable plan
- network/fabric diagram
- failure-domain analysis
- serviceability notes
- budget and headroom
- unresolved risks

## Red-team review
Have another person/tool issue at least five change requests: lower rack kW, loss of one feed, switch model unavailable, cooling limit changes, required GPU count rises, or maintenance clearance is reduced. For each, state impact and whether you redesign, reject, or negotiate the requirement.

## Victory condition
The final rack is not “perfect.” It is a traceable design whose tradeoffs survive cross-functional questioning.

Operation Atlas is complete when every box in the rack has a reason, every cable has a destination, every watt has somewhere to go, and every major assumption is visible.
