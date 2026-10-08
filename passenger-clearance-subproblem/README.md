# Passenger Clearance Subproblem

## Table of Contents
- [The Problem](#the-problem)
- [The Challenge](#the-challenge)
- [Potential Solutions](#potential-solutions)
- [Evaluation](#evaluation)
- [Resources](#resources)

## The Problem
A school group of 32 passengers arrives at the airport to check in for the same flight less than an hour before the check-in deadline. Although the passengers are travelling together, each person has different document requirements, seat assignments and baggage information. Most passengers are cleared immediately, but several require additional document review.

Processing every passenger individually creates a long queue and increases the risk that the group will not complete check-in on time. However, treating the entire group as one unit could cause individual document or baggage issues to be overlooked. Staff need a way to see which passengers are ready, which require attention and what issues remain unsolved. 

## The Challenge
Your challenge is to develop a solution that helps airport staff process passengers efficiently while maintaining accurate clearance information for each individual passenger. The solution should help staff identify who is ready, who requires additional review, and what issues still need to be resolved.

### Inputs and Expected Outputs 
You'll likely be working with passenger lists, bookings, document information, seat assignments, baggage records, check-in status, and schedules. As it is difficult to find perfect datasets, some of it will be missing, late, or contradictory. Design for that instead of around it.

Whatever you build should make passenger clearance status easy to understand at a glance: who is cleared, who requires attention, what issues remain unresolved, and why.

## Potential Solutions
A few possible scopes below. You can extend one or build something else entirely.

| Potential solution | Description | Starting point |
| --- | --- | --- |
| Unified identity gateway | Combine booking lookup, document checks, seat selection, baggage declaration, boarding passes, and agent review. | [Working implementation](unified-identity-gateway/README.md) |
| Document-review assistant | Validate required fields, identify mismatches, and route uncertain cases to an agent. | [Identity-gateway rules](unified-identity-gateway/apps/api/src/rules/) |
| Passenger-clearance dashboard | Show which passengers are cleared, blocked, or awaiting review and explain outstanding issues. | [Unified Identity Gateway](unified-identity-gateway/README.md) |
| Baggage reconciliation tool | Link accepted bags to passengers and explain missing or unexpected scans. | [Baggage Handling System](../baggage-handling-system/README.md) |

### Evaluation

Worth checking your solution against:

| Area | What to look for |
| --- | --- |
| Workflow completeness | Does the process work from input to result? |
| Data modelling | Are passengers, bags, flights, and seats represented clearly? |
| Decision quality | Are recommendations, predictions, and review flags useful? |
| Exception handling | Does the system handle missing, inconsistent data, and edge cases? |
| Dashboard clarity | Can an operator understand readiness and outstanding work from a glance? |
| Privacy and accessibility | Is sensitive data minimized, and is feedback usable by people with different needs? |
| Code quality | Is the implementation modular, readable, and maintainable? |
| Demonstration | Does the demo make the value and limitations clear? |

## Resources
### Challenge Resources

- [Unified Identity Gateway implementation](unified-identity-gateway/README.md)
- [Passenger-processing project ideas](passenger-processing/README.md)
- [Identity-gateway challenge specification](unified-identity-gateway/docs/challenge-spec.md)

### Safety, Privacy, and Industry References

- [ICAO Doc 9303 machine-readable travel documents](https://www.icao.int/publications/pages/publication.aspx?docnum=9303): international specifications for machine-readable passports and identity documents
- [ICAO Annex 9: Facilitation](https://www.icao.int/facilitation-programmes/Annex9): international passenger, border, and document-control context
- [Canadian Aviation Security Regulations, 2012](https://laws-lois.justice.gc.ca/eng/regulations/SOR-2011-318/index.html)
- [Secure Air Travel Regulations](https://laws-lois.justice.gc.ca/eng/regulations/SOR-2015-181/FullText.html)
- [Personal Information Protection and Electronic Documents Act](https://laws-lois.justice.gc.ca/eng/acts/P-8.6/index.html)
- [Accessible Transportation for Persons with Disabilities Regulations](https://laws-lois.justice.gc.ca/eng/regulations/SOR-2019-244/index.html)

