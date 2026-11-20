# PoWV Technology Development: Engineering Cost Benchmarks, Employment Costs and IP Valuation

**Public methodology note · 20 November 2026 · Version 0.1 · Preliminary and unaudited**

This is the companion methodology to the [2025–2026 Technology Capital Formation Schedule](../06-financial-model/TECHNOLOGY_CAPITAL_FORMATION.md). Its purpose is to make the labor reference, cost-allocation logic, current-money adjustments, asset depreciation and possible intellectual-property value drivers independently inspectable.

**Scope of the present public model:** founder-declared physical inputs, estimated infrastructure allocation and imputed professional effort. None of the calculations below is an audited balance-sheet value, independent appraisal, proof of commercial revenue, or certified market value.

## 1. Five measures of cost and value

| Measurement | What it answers | Appropriate input | Current status |
| --- | --- | --- | --- |
| **A. Historical transaction cost** | What was actually paid, by whom, and when? | Receipts, invoices, payment dates, bank/exchange records | Partial founder-supplied inventory; reconciliation pending |
| **B. Historical-cost restatement** | What is the purchasing-power equivalent at a defined reporting date? | Transaction-dated costs and the IBGE IPCA series | Formula documented; not yet calculated item by item |
| **C. Physical-asset carrying / replacement value** | How much useful equipment value remains, or what would equivalent capacity cost to acquire today? | Acquisition dates, asset classes, useful life/residual value, observable replacement prices | No supported consolidated amount yet |
| **D. Technical reproduction cost** | What would comparable specialized work and infrastructure cost to recreate? | Work-by-deliverable estimates, senior labor benchmarks, applicable burden, current tooling | Illustrative working model available; sensitivity described below |
| **E. Intellectual-property economic value** | What risk-adjusted economic benefit could rights and know-how produce for a specific participant? | Identified rights, use cases, willingness to pay, licensing or cash-flow evidence, implementation and commercialization risks | Research agenda; no independently supportable value concluded |

The first four measures can support a cost-based analysis. The fifth is a distinct valuation exercise. Adding **all** five to one number would double-count overlapping economic contributions.

## 2. Independent salary benchmark and worked reconstruction

The **Robert Half 2026 Brazilian salary guide**, as reproduced with attribution by Serasa Experian, reported the following **national monthly salary** range for a **senior full-stack developer**:

| Salary percentile | Monthly BRL | Illustrative BRL/hour at 160 h/month | 1,185 modeled hours (BRL) |
| --- | ---: | ---: | ---: |
| 25th | 12,450 | 77.8125 | 92,207.81 |
| **50th (reference model)** | **16,250** | **101.5625** | **120,351.56** |
| 75th | 20,950 | 130.9375 | 155,160.94 |

**Source:** [Serasa Experian, “Áreas da tecnologia mais bem pagas em 2026” (reproducing Robert Half, Guia Salarial 2026)](https://www.serasaexperian.com.br/carreiras/blog-carreiras/areas-da-tecnologia-mais-bem-pagas/).

**Calculation:** monthly benchmark / modeled productive-hours denominator × modeled founder hours. The **160 h/month denominator is a modeling choice**, not a Brazilian legal work-hour divisor or an audited founder timecard. At **200 h/month**, the same median monthly salary would imply **BRL 81.25/hour** and **BRL 96,281.25** for 1,185 hours, before any employment burden. The difference between the two estimates reflects the choice of monthly hours.

A full-stack job title is only a **general software-development comparator**, not a definitive market match for all PoWV work. Technical activities may require distinct future benchmarks for embedded software, hardware security, architecture, applied cryptography, data integrity and independent validation. Dated deliverables provide the basis for allocating hours by workstream and selecting a salary benchmark for each task.

The model continues to distinguish **Stage A (525 h, August 2025–March 2026)** from **Stage B (660 h, April–20 November 2026)**. These are assumed hours awaiting activity-level verification; a Git commit, document, signature or test result proves neither the precise human time expended nor a professional qualification.

## 3. Payroll burden: a separate replacement-employment scenario

A monthly salary figure is not automatically the total cost to employ an equivalent engineer. For a **hypothetical Brazilian CLT replacement role**, an explicit scenario may consider:

- **13th salary:** an additional 1/12 of monthly pay per worked year in this simplified annualized model.
- **Vacation third:** an incremental 1/3 of one month of pay, allocated across 12 months. The ordinary paid vacation month is already included in twelve monthly salaries here and is counted once.
- **Employer social-security contribution:** a **20% general employer rate**, **when the regime and employer actually make it applicable**.
- **FGTS:** generally **8%**, subject to the relevant employment rules.
- **RAT/SAT, third-party contributions, benefits, productive-time assumptions, termination provisions, recruitment and actual tax treatment:** the estimate for each component depends on the employer and role.

Authorities: [Federal Revenue — corporate social-security contributions](https://www.gov.br/receitafederal/pt-br/assuntos/orientacao-tributaria/tributos/contribuicoes-previdenciarias-pj); [Ministry of Labor — FGTS](https://www.gov.br/trabalho-e-emprego/pt-br/assuntos/inspecao-do-trabalho/areas-de-atuacao/fgts-fundo-de-garantia-do-tempo-de-servico); [Federal procurement pricing framework, IN 5/2017, Annex VII-D](https://www.gov.br/compras/pt-br/acesso-a-informacao/legislacao/instrucoes-normativas/instrucao-normativa-no-5-de-26-de-maio-de-2017-atualizada). These describe statutory components and contract-cost methodology; they do **not** certify that the founder was employed, paid, or owed those charges.

**Optional, deliberately incomplete CLT sensitivity:**

```text
Annual-pay uplift = 1 + (1/12 for 13th salary) + (1/36 vacation third)
Illustrative employer-tax factor = 1 + 0.20 employer INSS + 0.08 FGTS
Combined illustrative factor = 1.422222...
Median-salary modeled work = BRL 120,351.56 (unrounded model base)
Illustrative burdened work = BRL 171,166.67
Non-labor working-model base = BRL 27,923.55
Illustrative combined replacement scenario = BRL 199,090.22
```

**BRL 148,275.11** is the published historical formation-cost scenario. **BRL 199,090.22** is a separate estimate of the cost of hiring a replacement engineer and covering the modeled non-labor costs. This scenario excludes some potential costs, depends on employment/tax assumptions and is not evidence that statutory charges were paid or are owed. The non-labor base itself contains modeled residential costs and services not yet reconciled.

A separate service-company or independent contractor cost may be more relevant for outsourcing certain specialized activities; in that case it needs its **own sourced rates**, instead of adding CLT charges to consulting quotations.

## 4. Inflation and physical depreciation: different measurements

### 4.1 Purchasing-power restatement

The official Brazilian consumer-price reference is the **IBGE IPCA**. An expense incurred in month `m` may be restated to the last released index month `t` using:

```text
Amount in t-month BRL = nominal historical amount × (IPCA index level at t / IPCA index level at m)
```

The item-level calculation requires the transaction month, nominal BRL amount, IPCA release and series identifier, base month and rounding convention. Each expense has its own adjustment period because the transactions span August 2025 to November 2026.

As of the assessment cutoff **20 November 2026**, the latest published monthly IPCA cited here is **October 2026**, with **0.14% monthly change and 4.63% over the previous 12 months**. These are context figures, **not** a universal factor to multiply all project costs by. Expenses later than the latest available index month require a disclosed cutoff convention.

Official sources: [IBGE, IPCA and its calculator](https://www.ibge.gov.br/explica/inflacao.php); [IBGE October 2026 release](https://ftp.ibge.gov.br/Precos_Indices_de_Precos_ao_Consumidor/IPCA/Fasciculo_Indicadores_IBGE/ipca-inpc_202610caderno.pdf).

The 2026 salary benchmarks enter the comparison at their published amounts. A historical 2025 salary benchmark, if later obtained, could instead be translated explicitly to a common price date.

### 4.2 Depreciation, current replacement and obsolescence

Physical equipment requires an **asset-by-asset** assessment:

- **Accounting carrying amount** depends on recognition, cost, depreciation policy, asset availability for use, useful life, residual value and relevant impairment assessment.
- **Tax-life reference** may be informed by the applicable Federal Revenue depreciation schedule, but it is not itself the accounting useful-life determination.
- **Current replacement cost** requires quotations for functionally equivalent equipment and may differ materially from indexed purchase price or accounting carrying amount.
- Items with research-prototype utility may retain technical usefulness even if their resale value is low. Technical usefulness alone provides no basis for increasing an asset’s carrying amount.

References: [CPC 27 — property, plant and equipment](https://www.cpc.org.br/CPC/Documentos-Emitidos/Pronunciamentos/Pronunciamento?Id=58); [Federal Revenue IN RFB 1,700/2017 — depreciation and useful-life framework](https://normas.receita.fazenda.gov.br/sijut2consulta/link.action?idAto=81268).

A **signed or hashed technical document is not a depreciable physical asset**. Research documents, source code, design rights and know-how require separate intellectual-property and accounting classification.

## 5. Evidence strength and what is actually demonstrated

| Evidence class | What it can support | What it does not independently establish |
| --- | --- | --- |
| Founder-authored historical whitepaper and research documents | Documented descriptions and a claimed chronology of research | Independent novelty assessment, patents granted, verified economic value |
| Signed electronic PDF retained privately | Identity/integrity evidence **subject to successful signature validation**, and correspondence with a specific document version | External certification of technical correctness, commercial maturity or inventorship |
| Git history and dated public engineering records | Observable versions, changes and stated engineering milestones | Full historical hours, exclusivity of authorship or source measurement truth |
| Software CI/testing reports | Tests passed in the stated software environments and tested scope | Independent security certification, production approval or physical hardware validation |
| Scale-to-edge experimental report | Reported limited physical-data acquisition and transmission demonstration | Certified end-to-end hardware attestation, industrial field reliability or audited financial settlement |
| Invoices, bank records and dated time logs (restricted access) | Individual monetary payments and effort reconstruction when reconciled | Market value of associated intellectual property by themselves |
| Customer pilots, contracts and independent outcome measurement | Attributable savings, adoption, willingness to pay and revenue evidence | Automatic extrapolation of pilot outcomes to the entire sector |

No claim is made here that PoWV has received an **independent technology certification**, a completed independent valuation or formal recognition of the cost scenario as an asset. The reported tests document internal validation.

The accompanying [formation-cost schedule](../06-financial-model/TECHNOLOGY_CAPITAL_FORMATION.md) supplies the public evidence IDs and SHA-256 fingerprints of two underlying source revisions. A hash validates a byte-for-byte match; it does not validate the amounts contained in a file.

## 6. Economic value of the intellectual property

The intellectual work is assessed by its **relevant economic contribution**, not merely by multiplying historical development expenditure by an arbitrary innovation premium.

The World Intellectual Property Organization (WIPO) describes established approaches including:

1. **Cost approach:** current cost to recreate/replace comparable capability, with obsolescence, remaining effort and relevant limitations.
2. **Market approach:** observable comparable licenses, transfers or transactions, with adjustments for differences in rights, maturity and market conditions.
3. **Income approach:** present value of incremental attributable cash flows, avoided licensing costs/royalties or measurable operating savings, adjusted for risk.
4. **Real options / scenario methods:** staged decisions and commercial/technical uncertainty for early-stage research.

Sources: [WIPO — Valuing IP Assets](https://www.wipo.int/en/web/business/ip-valuation); [WIPO (2025) — IP Valuation Basics for Technology Transfer Professionals](https://www.wipo.int/web-publications/intellectual-property-valuation-basics-for-technology-transfer-professionals/en/3-ip-valuation-methods.html); [WIPO — Income Approach](https://www.wipo.int/web-publications/intellectual-property-valuation-basics-for-technology-transfer-professionals/en/6-the-income-approach.html).

**PoWV candidate economic benefits to test** include measurement-event traceability, lower reconciliation and fraud-investigation costs, evidence quality for physical-to-digital asset workflows, bounded dispute exposure, lower counterparty verification friction and infrastructure integration. These are **testable value hypotheses**, not yet established customer savings.

An income model for licensing would link operating evidence to estimated cash flows as follows:

```text
Identified customer workflow
  → measured operational problem and current baseline
  → documented PoWV contribution to solving it
  → incremental attributable savings or willingness to pay
  → achievable fee / royalty or licensing model
  → adoption, operating costs, implementation and legal risks
  → appropriately risk-adjusted present value
```

For example, **sector-wide capital flow × hypothetical fee rate** may describe an illustrative addressable revenue *scenario*, but cannot demonstrate current IP value without the fraction of that flow **actually addressable, contracted or credibly obtainable**. The value of underlying waste materials, trade-finance obligations, tokenized rights and PoWV software/services must not be conflated or counted multiple times.

## 7. Sector context — scale of the problem, not project revenue

The [World Bank, *What a Waste 3.0* (2026)](https://www.worldbank.org/en/publication/what-a-waste), estimates that **global municipal solid-waste management costs exceed USD 250 billion per year** and could rise to **USD 426 billion in 2050** under the report's baseline.

These figures concern **global municipal waste-management costs**. They are **not**:

- PoWV revenue, enterprise value, or project cash flow;
- annual revenue of the waste tokenization industry;
- the total value of verified recyclable materials, credits or financial obligations;
- an assessed serviceable market share for PoWV.

Product-level market sizing depends on separate **TAM / SAM / SOM assumptions** and a defined unit of monetization (device, verified event, enterprise license, integration, verification service, or another contractually agreed unit). Only attributable revenue and costs would feed an income-based IP valuation.

## 8. Accounting recognition and independent evaluation

- [CPC 04 (R1) / IAS 38](https://www.cpc.org.br/CPC/Documentos-Emitidos/Pronunciamentos/Pronunciamento?Id=35): research versus development phases, control, probable future benefits and reliable measurement of attributable cost are critical to any intangible recognition analysis.
- [CPC 27 / IAS 16](https://www.cpc.org.br/CPC/Documentos-Emitidos/Pronunciamentos/Pronunciamento?Id=58): tangible asset recognition and depreciation.
- [CPC 46 / IFRS 13](https://www.cpc.org.br/CPC/Documentos-Emitidos/Pronunciamentos/Pronunciamento?Id=78): fair-value measurement framework when such a measurement is required or appropriate.

**Three independent outcomes are possible:** a historically reconciled cost schedule, a current reproduction-cost estimate, and a market-participant economic IP valuation. They have different purposes, assumptions and evidentiary thresholds; they are **not necessarily additive**. Accounting capitalization or formal appraisal must be evaluated for the relevant entity and transaction.

## 9. Project costs and IP value

| Area | Basis for assessment |
| --- | --- |
| Expenses | Payment records establish the project’s share of costs and the period covered in November. October 2026 is the reference month for the proposed IPCA adjustment. |
| Equipment | Replacement estimates use dated prices for equivalent equipment and account for the condition of each item. |
| Engineering | The model estimates 1,185 hours of founder engineering work across two stages (525 + 660). Dividing the monthly salary by 160 or 200 hours gives two hourly cost estimates. Total CLT employment costs and contractor quotes provide alternative benchmarks. |
| Intellectual property | Valuation depends on licensing rights, reproducible pilot results and evidence of future income or comparable transactions. |

Financial records, implementation details, restricted economic assumptions and unpublished IP documents remain confidential.
