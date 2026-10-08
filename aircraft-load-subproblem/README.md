# Aircraft Load Subproblem
## Table of Contents

- [The Problem](#the-problem)
- [The Challenge](#the-challenge)
- [Potential Solutions](#potential-solutions)
- [Resources](#resources)

## The Problem
A mechanical issue causes the airline to replace the originally scheduled aircraft with a smaller aircraft shortly before departure. The new aircraft has different seating, baggage capacity and weight-and-balance limits. 

Passengers have already checked in, seats have been assigned, and baggage is being prepared for loading. Because the new aircraft has less capacity and different loading constraints, the existing passenger and baggage plan can no longer be used directly. Staff must quickly determine how to reassign passengers and baggage while accounting for the available capacity and avoiding unnecessary delays.

## The Challenge
Your challenge is to develop a solution that quickly adapts the existing passenger and baggage plan to the replacement aircraft while maintaining safe weight-and-balance limits and minimizing operational disruption.  

To do this, you can either create your own solution or build off and improve the existing aircraft load control program. 

## Potential Solutions

A possible scope below. You can extend one or build something else entirely.

| Potential solution | Description | Starting point |
| --- | --- | --- |
| Aircraft load control | Assign passenger and cargo load to aircraft zones while respecting weight and balance limits. | [`load-control/`](load-control/) |
| Aircraft-swap replanning tool | Reassign passengers, seats, baggage, and cargo after an aircraft change. | 
| Weight-and-balance dashboard | Show aircraft loading, zone weights, limits, and potential violations. |
| Load-plan optimization tool | Find a safe loading arrangement while minimizing passenger or baggage disruptions. |

## Resources

- [ICAO Annex 6: Operation of Aircraft](https://store.icao.int/en/annex-6-operation-of-aircraft): international aircraft-operation context, including mass and balance responsibilities
- [IATA Resolution 753 baggage-tracking implementation guide](https://www.iata.org/contentassets/5c4aa8b8b3b1432697d2bf3301450684/reso753-implementation-guide---2023_issue-4.02.pdf): baggage tracking at defined handoff points
- [IATA Weight and Balance Manuals](https://www.iata.org/en/publications/manuals/weight-balance-manuals/): airline load-control procedures and data standards
- [Brock Solutions SmartLoad](https://www.brocksolutions.com/smartload/): An industry solution for cargo tracking, load reconciliation, and real-time weight-and-balance plan validation.

