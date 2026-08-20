# Atlas-Rack

> **Operation Atlas — design an AI rack, then keep revising it until power, cooling, cabling, serviceability, redundancy, and cost all agree.**

## Project status

| Field | Current state |
|---|---|
| **Status** | **Planned — requirements/layout in Weeks 9–10; core physical-design work in Weeks 19–20** |
| **Current stage** | Campaign authored; no rack design, BOM, or capacity figure is presented as a completed engineering result |
| **Lab environment** | Design/modeling project using public vendor specifications and explicit assumptions |
| **Evidence rule** | Values must be labeled vendor-specified, calculated, assumed, or modeled; none imply physical deployment |
| **Last plan sync** | 2026-08-19 |

## Purpose

Atlas-Rack is the physical AI-infrastructure design lab. Fictional **Northstar Compute** needs to fit useful GPU capacity into a constrained rack position while facilities, networking, operations, and finance keep adding requirements.

The objective is to answer:

> **Could this design actually be installed, powered, cooled, cabled, maintained, and recovered when something fails?**

The first layout is expected to be wrong. The engineering value comes from exposing assumptions, applying constraints, and documenting why the design changes.

## Skills developed

- rack units, physical layout, and serviceability
- AI server/GPU platform form factors
- power-chain reasoning, A/B feeds, rack PDUs, and headroom
- air vs direct-to-chip liquid-cooling concepts
- CDU/manifold/heat-removal paths
- cable/port planning and redundancy
- weight, maintenance clearances, failure domains, and BOM tradeoffs

## Design campaign

The files in [`missions/`](missions/) are authoritative. Missions 02–05 are the core Weeks 19–20 work; Mission 06 and the final review are stretch work when the Week 20 milestone is secure.

| Mission | Design problem | Primary outcome |
|---|---|---|
| [00 — Requirements](missions/00-requirements.md) | Turn vague business demand into explicit constraints | requirements/assumptions packet |
| [01 — Layout](missions/01-layout.md) | Produce the intentionally naive first rack | initial elevation + questions |
| [02 — Power](missions/02-power.md) | Apply feed, PDU, PSU, and headroom constraints | power budget + redesign |
| [03 — Cooling](missions/03-cooling.md) | Trace heat-removal requirements and cooling limits | cooling path + redesign |
| [04 — Cabling](missions/04-cabling.md) | Map network/power cable paths and service access | port/cable map |
| [05 — Redundancy](missions/05-redundancy.md) | Test failure domains and A/B design assumptions | resilient architecture review |
| [06 — Procurement](missions/06-procurement.md) | Add BOM, availability, and cost tradeoffs | procurement-aware design **(stretch)** |
| [Final — Atlas Design Review](missions/final-design-review.md) | Defend the design against cross-functional change requests | traceable final review **(stretch if needed)** |

## Modeling rule

Use dated public vendor specifications or clearly declared fictional inputs. Separate:

- vendor-specified values
- calculations derived from those values
- planning assumptions
- intentionally simplified models

Never imply that a modeled rack was physically deployed or facility-approved.

## Evidence standard

A strong Atlas packet should include requirements, rack elevation, power/feed model, cooling/heat path, network/fabric diagram, cable/port map, failure-domain analysis, serviceability notes, BOM/cost assumptions, headroom, rejected alternatives, and unresolved risks.

## Completion condition

Operation Atlas is complete when every major component has a reason, every power/network/cooling path is traceable, assumptions are visible, and the design can survive reasonable cross-functional challenge without pretending that the model is a real deployment.
