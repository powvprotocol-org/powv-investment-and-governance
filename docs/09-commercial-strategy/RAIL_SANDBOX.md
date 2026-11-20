# Rail evidence sandbox and field pilot

**Planning case updated 20 November 2026 · One application of PoWV’s evidence architecture**

The June concept combined a 16-week engineering sandbox, a railway field pilot and revenue at network scale. These are three distinct decisions. The September [bench record](https://github.com/powvprotocol-org/powv-scale-edge-integration/blob/main/docs/integration-module/experimental-record.md) already documents a real scale reading reaching an embedded receiver over a local network. A rail sandbox would build on that result by testing device-backed signing, live satellite delivery and independent verification of the received record. The [November software tests](https://github.com/powvprotocol-org/powv-lab-status/blob/main/status/2026-11-software-engineering-update.md) have a separate, software-only scope.

## Sandbox budget

One bench, an existing compatible scale, one prototype path and access to a live satellite messaging service are assumed. The 16 weeks are a planning window from equipment availability and service activation. Parallel or part-time roles account for different person-month totals. These are estimates of the economic cost of delivery, in nominal BRL. Existing equipment or contributed founder time can reduce the cash request when documented.

| Budget line (BRL) | Lean | Working case | Extended |
| --- | ---: | ---: | ---: |
| Software and evidence integration at 16,250 per person-month | 32,500 (2 months) | 48,750 (3 months) | 65,000 (4 months) |
| Controls and instrument integration at 12,500 per person-month | 18,750 (1.5 months) | 25,000 (2 months) | 37,500 (3 months) |
| Planning allowance for employment costs, 30% of salary base | 15,375 | 22,125 | 30,750 |
| Incremental devices, interfaces, antenna, spares and procurement | 4,500 | 8,000 | 12,000 |
| Test airtime and infrastructure | 1,000 | 2,500 | 5,000 |
| External test review and reporting | 5,000 | 10,000 | 18,000 |
| Contingency on subtotal | 7,713 (10%) | 17,456 (15%) | 33,650 (20%) |
| **Estimated total, rounded to BRL** | **84,838** | **133,831** | **201,900** |

The lean case assumes an available interface and limited test traffic. The working case includes additional integration time and external review. The extended case allows another integration iteration, spares and a larger test campaign. The reviewer’s scope, engineering hours, overhead, hardware bundle and contingency are planning inputs. The 30% allowance represents a sensitivity assumption. Employment or contractor quotes would replace the corresponding salary and overhead lines together.

**Price anchors.** The software proxy is the 2026 national median for senior full-stack development. The controls proxy rounds the November 2026 Brazilian average of BRL 12,494 per month for control and automation engineers. A satellite development module was publicly listed at USD 302 before accessories, freight, taxes and service. It benchmarks one component. A rugged field terminal and local support require their own quote. Development airtime can include monthly rental and credits per 50 bytes or fraction, including certain mailbox checks. The airtime budget depends on actual message size, retries and traffic. [Software salary reference](https://www.serasaexperian.com.br/carreiras/blog-carreiras/areas-da-tecnologia-mais-bem-pagas/) · [Brazilian controls salary data](https://www.salario.com.br/profissao/engenheiro-de-controle-e-automacao-cbo-202110/) · [Module price](https://store.groundcontrol.com/products/rockblock-9603) · [Development airtime terms](https://docs.groundcontrol.com/iot/rockblock/web-services/iridium-contract-costs)

At BRL 67,000, the June allowance would fall below the working case's BRL 73,750 in base labor alone. It could cover a narrower cash-funded scope if a partner supplies equipment or personnel. The working estimate is compatible in scale with [illustrative Round A](../06-financial-model/VENTURE_FUNDING_SCENARIOS.md). The two figures overlap: a sponsor payment, grant or in-kind contribution for the same work reduces the remaining financing need.

## Sandbox budget in US dollars

The 19 November 2026 closing PTAX selling rate was **BRL 5.8889 per USD**, the latest closing reference available on 20 November. The two stress rates are rounded assumptions roughly 10% either side of that reference. Amounts use the same BRL scope throughout, rounded to the nearest dollar. [Central Bank of Brazil closing PTAX](https://ptax.bcb.gov.br/ptax_internet/consultarUltimaCotacaoDolar.do).

| Sandbox scope | Budget (BRL) | USD at 5.8889 | USD at 5.30 | USD at 6.48 |
| --- | ---: | ---: | ---: | ---: |
| Lean | 84,838 | 14,406 | 16,007 | 13,092 |
| Working case | 133,831 | 22,726 | 25,251 | 20,653 |
| Extended | 201,900 | 34,285 | 38,094 | 31,157 |

The working case is about **USD 22,726** at the reference rate. Imported hardware and satellite service priced in USD have a different exposure: their BRL cost rises when the dollar strengthens. A procurement budget would retain those items in their invoice currency and translate only the BRL-priced remainder. The site pilot still requires its own quote. [Twelve-month FX assumptions and installment example](../06-financial-model/VENTURE_FUNDING_SCENARIOS.md#us-dollar-view-and-12-month-currency-sensitivity).

## Milestones and acceptance

| Indicative window | Sandbox output | Evidence for acceptance |
| --- | --- | --- |
| Weeks 1–4 | Repeatable acquisition on the existing bench | Dated baseline, identified instrument and a comparison between its reading and the captured record. |
| Weeks 5–8 | Prototype signing at capture and independent verification | A separate verifier checks attribution to the enrolled prototype and records results for original and altered samples. |
| Weeks 9–12 | Live satellite delivery | Send and receive logs identify delivered, delayed, repeated and missing events. Billed usage is reconciled to the test traffic. Simulated transmissions have a separate label. |
| Weeks 13–16 | Repeat run and external review | A reviewer records equipment, versions, test conditions, exceptions and results against thresholds agreed before testing. Field readiness is a separate decision. |

## One-site field pilot

Field work starts with written site access, an agreed instrument interface, a responsible operator, baseline data and a budget for that location. The pilot would run alongside existing procedures, compare records for the same movements and measure completeness, end-to-end delay, exception handling time and cost per accepted event. The operator and reviewer would define the observation window and acceptance thresholds before deployment.

A field quote adds site survey and access, installation, rugged hardware, field connectivity, operator integration, travel, testing and support. Procurement must establish whether an existing scale and its data can be used and whether any metrology or site approvals apply. An industrial scale purchase or track work would change the scope materially. A site pilot price remains open until those inputs are known. The price of that service and the company's equity funding are separate negotiations.

## Commercial unit after a pilot

A buyer could pay a one-time integration fee, a recurring per-site service fee and a usage fee for accepted evidence. One candidate usage unit is 1,000 verified net tonne-kilometres. For an eligible movement, the calculation is accepted net tonnes × recognized distance in kilometres. A signed weight alone establishes neither distance nor entitlement to bill. The contract would specify the distance source, duplicates, corrections, disputes and the person authorized to accept the movement. [Official rail production measures](https://saff.antt.gov.br/Manual/mnusiade_consulta_producao.htm)

**Usage revenue = accepted, billable tonne-kilometres ÷ 1,000 × negotiated unit fee.** Where a minimum-volume commitment applies, only the excess above the included volume is billed again. Traffic on an entire network, freight tariffs and the value of insured cargo do not determine PoWV revenue. Field pricing and gross margin depend on measured delivery cost, customer benefit and agreed terms. This case names no commercial partner and assumes no contracted traffic.
