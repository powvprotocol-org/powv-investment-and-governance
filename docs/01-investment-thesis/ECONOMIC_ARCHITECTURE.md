# ECO-1 — Economic Architecture of PoWV Protocol

**Status:** Public working framework · **Version:** 0.1 · **Date:** 2026-11-20  
**Scope:** PoWV Protocol only · **Decision status:** No economic mechanism is approved by this document.

## Purpose

This document establishes a public framework for studying how PoWV's physical-to-digital evidence infrastructure could support commercially useful services, asset representations, and financial applications.

The work begins with the economic and legal nature of the object represented. Evidence integrity, an asset representation, a contractual entitlement, and a payment obligation are different things. A verified technical record does not independently create ownership, a receivable, a certified environmental benefit, or a claim enforceable against a third party.

This framework is designed for incremental analysis. It records questions and candidate directions without declaring a final token model, product launch, fundraising transaction, or regulatory classification.

## D1 — Nature of evidence, assets, and rights

The first workstream examines **what is represented, by whom, and with what legal and economic consequences**.

| Conceptual layer | Function under examination | Questions to resolve |
| --- | --- | --- |
| Physical-event evidence | Traceable evidence concerning a measured or observed event | What was observed? What controls support admissibility? |
| Lot or process record | Digital record linked to an identifiable lot, process, or outcome | Does it attest to a fact, convey a right, or both? |
| Asset or contractual-right representation | Digital representation of rights concerning goods, services, or claims | Who creates, recognizes, holds, transfers, and extinguishes those rights? |
| Optional network utility mechanism | Possible mechanism for infrastructure fees, guarantees, or network coordination | Is a native token necessary at all, or can services operate through ordinary contractual payments? |

**Candidate direction under examination:** keep evidence, legally recognized asset rights, and infrastructure remuneration conceptually separate. The existence, design, and role of any native token remain open decisions.

### Open D1 questions

- Define the issuer, holder, transferee, and obligated counterparty for each contemplated representation.
- Distinguish a factual certificate from an instrument conveying legal title or a financial claim.
- Establish whether transferability is required and, if so, which rights are transferred.
- Determine supply, issuance, redemption, cancellation, and retirement principles by asset type.
- Establish the applicable legal and regulatory perimeter for each concrete use case.

## D2 — Recognition, authorization, and asset lifecycle

The second workstream examines **when evidence is sufficiently admissible for a downstream economic action**.

An illustrative separation of responsibilities is:

1. A physical or operational event is captured and represented as evidence.
2. The evidence is evaluated under defined technical and operational controls.
3. An authorized party determines whether the evidence supports a specific business or legal action.
4. Where applicable, an asset or right is represented in a controlled digital system.
5. Subsequent transfers, disputes, corrections, redemptions, and retirement events are governed by explicit rules.

No software-only verification result, digital signature, or blockchain entry should be interpreted as an unconditional certification of physical truth or legal ownership.

### Open D2 questions

- What evidence classes and independent checks are sufficient for each type of representation?
- Who has authority to recognize a lot or issue a legally meaningful claim?
- How are disputed measurements, invalidated records, and post-issuance corrections handled?
- What prevents duplicate recognition of the same quantity or environmental outcome across different registries and programs?
- What rules govern expiry, redemption, cancellation, and permanent retirement?
- Which controls require physical field validation before commercial use?

## D3 — Revenues, participant payments, and economic security

The third workstream separates **the business model of the PoWV technology provider** from **cash flows belonging to industrial operators or other parties**.

| Economic flow | Initial analytical treatment |
| --- | --- |
| Sale of physical goods or materials | Revenue of the seller or operator under its commercial arrangements |
| Payment for an environmental or verified service | Contractual revenue whose entitled recipients and allocation must be established |
| Technology, verification, and integration fees | Potential revenue of the relevant PoWV enterprise or authorized network service provider |
| Guarantees, reserves, and dispute-related commitments | Risk controls and funding obligations, not automatically operating revenue |

A distribution mechanism describes *how* entitlements may be settled; it does not establish *where the funds originate* or *who owns them*.

### Open D3 questions

- Identify the payer, beneficiary, contractual obligation, timing, and accounting recognition for each flow.
- Determine whether verification is billed separately or paid from another contractual flow.
- Distinguish funds held on behalf of third parties from revenue earned by the technology provider.
- Establish which participant bears operational losses and the cost of disputed or reversed transactions.
- Evaluate whether economic guarantees are needed, how they are denominated, and who administers them.
- Examine whether independent validators and any associated incentive mechanism are necessary for the target deployment model.

## Enterprise economics versus operator economics

These must be modeled independently.

**Industrial operator:** material or service revenue, direct processing costs, fixed overhead, working capital, contractual allocations, reserves, and expected losses.

**PoWV enterprise:** product and service revenue, direct delivery costs, engineering expenditure, CAPEX, OPEX, gross margin, EBITDA, working capital requirements, and free cash flow.

The early-stage work will identify the right drivers and accounting boundaries before selecting valuation methods or financing structures. A technology valuation is not inferred from the market value or physical quantity of third-party assets represented through the protocol.

## Governance and control

The governance analysis will distinguish:

- **Corporate governance:** ownership, fiduciary authority, intellectual property, budgets, company treasury, contracts, and executive accountability.
- **Protocol governance:** technical standards, admissibility policies, change control, and any future shared network parameters.
- **Independent review:** expert or stakeholder committees that can inform decisions without being assumed to own company assets or legally bind third parties.

Any decentralization proposal must define the legal entity, decision authority, treasury perimeter, liabilities, and limits of delegated powers.

## Parallel validation and diligence

Economic design will advance alongside engineering and field studies:

- Evidence provenance, device identity, and physical measurement reliability.
- Claims of uniqueness and prevention of duplicate recognition.
- Identity and eligibility of economic beneficiaries.
- Integration costs, buyer procurement processes, and contractual demand.
- Regulatory classification of concrete rights and services.
- Operational costs and risk parameters derived from representative data.

## Publication boundary

This page is an **institutional study map**, not a smart-contract specification or a disclosure of unpublished structural tokenomics. It intentionally omits confidential economic parameters, payout rates, guarantee amounts, contract implementation details, and undisclosed internal models. Restricted work should remain within the access controls set by the organization's [Trade Secret and Intellectual Property Protection Policy](https://github.com/powvprotocol-org/powv-governance-and-docs/blob/main/TRADE_SECRET_POLICY.md).

## Public references

- [PoWV Core — architecture and research scope](https://github.com/powvprotocol-org/powv-core)
- [PoWV Lab Status — experimental evidence and limits](https://github.com/powvprotocol-org/powv-lab-status)
- [Governance and documentation policies](https://github.com/powvprotocol-org/powv-governance-and-docs)

**Next:** use the [decision register](DECISION_REGISTER.md) to deepen each question individually, with recorded status and supporting evidence.
