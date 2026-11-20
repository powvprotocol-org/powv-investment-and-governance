# Investment Thesis

PoWV researches how an enterprise can establish the origin of a physical or operational record, evaluate its integrity and decide whether to accept it, hold it for review or act on it. The commercial hypothesis is that an operator or integrator will pay for verification when it reduces the cost of resolving exceptions or strengthens a consequential authorization decision.

| Proposed product | Decision it could support |
| --- | --- |
| Protocol Suite | Can a receiving system check the evidence accompanying an event before accepting it into an ERP or asset workflow? |
| Secure Capture Node | Which device produced a reading, and under what acquisition conditions? Hardware-backed identity at capture remains a development objective. |
| EdgeGuard | Does the available evidence about an operating environment support authorizing an action or holding it for review? |
| Digital Treasury | Could a treasury operator use EdgeGuard's controls before authorizing a sensitive financial operation? This is a proposed EdgeGuard profile. |

The [product portfolio](https://powv-protocol.gitbook.io/powv-protocol-docs/product-proposals/) describes the architecture and maturity of each proposal.

## Engineering evidence

The [physical bench record](https://github.com/powvprotocol-org/powv-scale-edge-integration/blob/main/docs/integration-module/experimental-record.md) documents a scale reading captured, transmitted and retrieved from an ESP32. The instrument tested the acquisition path. Its use applies no sector restriction to the protocol. The [November software report](https://github.com/powvprotocol-org/powv-lab-status/blob/main/status/2026-11-software-engineering-update.md) records 343 automated cases passing on each of two Python versions and conformance checks across implementations. Hardware-backed attestation and industrial performance still require separate validation.

## Commercial evidence

Potential applications include industrial and agricultural traceability, reconciliation of warehouse records for trade finance, operational security and environmental reporting. A measurement record can support review of an underlying asset. Ownership, financing and settlement depend on the relevant institutional and contractual arrangements. The public materials reviewed here document research and laboratory results. Commercial pricing, paid adoption and recurring revenue remain unsubstantiated in this record.

- [Candidate buyers and pilot measures](../09-commercial-strategy/README.md)
- [Workflow references and market-sizing method](../07-valuation-framework/BENCHMARKS_AND_IP_VALUATION.md#7-workflows-buyers-and-market-sizing)
- [ECO-1 economic architecture](ECONOMIC_ARCHITECTURE.md) and [open decisions](DECISION_REGISTER.md)
